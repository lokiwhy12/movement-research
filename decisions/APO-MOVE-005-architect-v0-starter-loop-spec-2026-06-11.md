# APO-MOVE-005 — Architect v0 Starter Loop Spec

Prepared by: Architect  
Prepared on: 2026-06-11  
Approval source: `APO-MOVE-005-exec-memo-2026-05-28-founder-approval-2026-06-11.yaml` (`branch: approve-pair`, `source_reply: "rec approved. do it."`)

## Purpose
Convert the approved `pull-factor onboarding + ritual map` recommendation into the **smallest shippable build packet** for Apotheosis.

## Scope freeze
Ship only the approved v0 outcome bundle:
1. onboarding ends with one personalized **Clarity Card**
2. that card is saved as a **Day 0 Snapshot**
3. the user can complete one **session-driven Day 1 check-in**

Out of scope: streaks, rankings, social loops, deep memory graphing, pressure mechanics, push-notification strategy, community features, council/routing rewrites.

---

## Frozen product decisions

### 1) Exact onboarding questions for v0
Use the **existing onboarding seed questions verbatim** as the Clarity Card input set. This is the smallest build because the questions, validation, and persistence already exist in the live onboarding flow.

Required input set for the starter loop:
- `display_name`
- `q1-stress` — "Think of the last few times you were under real pressure (money, work, relationship conflict, major problems). In roughly the first 60 minutes, what do you tend to do most often?"
- `q2-conflict` — "This is about conflict with people who matter most to you (partner, close friend, cofounder, family) — where your emotions and identity are actually involved. Think of the last few times you had real conflict with someone in that category. In the first 24 hours, what do you tend to do most often?"
- `q3-validation` — "When you’re unsure you’re ‘enough’ or did well (work, dating, creative output), what do you usually do in the next day or two?"
- `q4-stability` — "Look at the last 1–2 years. When your life becomes reasonably stable (money, schedule, relationships), what tends to happen next most of the time?"
- `q5-pursuit` — "When you really want something (a person, opportunity, project, or lifestyle change), how do you usually pursue it over the first days/weeks?"
- `q6-decision` — "When you have to make an important decision and you don’t have enough information to be sure — the data is incomplete, the outcome is uncertain, people are giving you conflicting advice — what do you actually do?"
- `q7-protection` — "When someone consistently crosses a line with you — disrespect, broken agreements, bad fit — and it’s not a one-time thing, what do you tend to do over the next days and weeks?"

Rules:
- Use the current answer options and validation exactly as implemented.
- Do **not** add new onboarding questions in this milestone.
- Existing context capture (`location`, `relationship_status`, `world_notes`) may remain in onboarding state, but the v0 Clarity Card must **not depend** on them.

### 2) Where the Day 0 Snapshot lives
The **Day 0 Snapshot lives on `/app` Home** as the first real product card above the existing dashboard grid.

Why:
- `/app` is already the Home surface in the shell.
- This is smaller than inventing a new timeline surface.
- It gives the user one obvious place to revisit the artifact after onboarding.

v0 UI rule:
- Home shows at most one active starter-loop card: the latest Day 0 Snapshot with its current Day 1 status.

### 3) Day 1 update model
**Day 1 updates the same card**, not a new linked Day 1 entry.

Why:
- It is the smallest clean implementation.
- It preserves the Day 0 artifact as the anchor object.
- It avoids building a second artifact list/timeline model in v0.

Non-destructive update rule:
- Keep the original Day 0 fields unchanged.
- Add Day 1 fields onto the same record (`day1_status`, `day1_reflection`, `day1_next_move`, `day1_completed_at`).

### 4) Smallest milestone split that gets this to Forge cleanly
Split into **two bounded Forge slices**:

#### Slice A — Day 0 vertical slice
Deliver:
- Clarity Card generation at onboarding completion
- Day 0 Snapshot persistence
- Home surface rendering of the saved snapshot
- instrumentation for onboarding complete, card delivered, snapshot viewed

Done when:
- a new user completes onboarding
- sees one Clarity Card before exit
- lands on `/app` and can see the saved Day 0 Snapshot later

#### Slice B — Day 1 ritual slice
Deliver:
- session-driven 2-minute Day 1 check-in on the same snapshot
- same-record update path for progress / revised next move
- instrumentation for Day 1 started/completed

Done when:
- returning user can open the saved snapshot
- answer the 3 Day 1 prompts
- complete the ritual in under 2 minutes
- see the updated state on the same card

This is the smallest clean split because Slice A is independently testable and Slice B layers on the exact saved artifact from Slice A.

---

## Recommended implementation seam

### Data model
Create one narrow persistence seam for the starter loop instead of overloading `user_onboarding_state`:
- new table: `starter_loop_snapshots`

Minimum columns:
- `id`
- `user_id`
- `source_calibration_snapshot_id`
- `source_conversation_id`
- `title`
- `pattern_label`
- `insight_text`
- `next_action_text`
- `generated_at`
- `day1_status` (`pending` | `completed` | `skipped`)
- `day1_reflection`
- `day1_next_move_text`
- `day1_completed_at`
- `created_at`
- `updated_at`

Rationale:
- clean boundary
- single retrieval object for Home + Day 1
- avoids entangling starter-loop state with onboarding resume state

### Generation rule
For v0, the Clarity Card may be generated by a **deterministic mapper** from the existing seed-answer construct tags plus a small template layer.

v0 output format:
- `title` = short named pattern / friction point
- `insight_text` = one-sentence leverage insight in plain English
- `next_action_text` = one concrete 24-hour move

Rule:
- Do **not** widen this milestone into a new council/orchestration feature.
- If LLM polish is used, it must stay behind the same narrow output contract.

### Surfaces / file scope
Primary file scope:
- `apps/web/src/app/api/onboarding/complete/route.ts`
- `apps/web/src/app/app/page.tsx`
- new starter-loop API/helpers under `apps/web/src/app/api/starter-loop/*` and/or `apps/web/src/lib/starter-loop/*`
- one Supabase migration for `starter_loop_snapshots`

Do not pull in:
- council routing files
- deep calibration flow
- weekly pulse surfaces
- My World surfaces
- notification infrastructure

---

## Acceptance criteria

### Slice A
- onboarding completion returns one Clarity Card before exit
- Clarity Card is persisted as a Day 0 Snapshot
- `/app` Home renders the saved snapshot for the authenticated user
- telemetry fires for:
  - onboarding completed
  - Clarity Card delivered
  - Day 0 Snapshot viewed

### Slice B
- returning user can start a Day 1 check-in from the Home snapshot
- Day 1 asks exactly:
  1. "Did yesterday’s next move happen?"
  2. "What changed?"
  3. "What is today’s smallest next move?"
- submit updates the same snapshot record
- telemetry fires for:
  - Day 1 check-in started
  - Day 1 check-in completed

---

## Recommended Forge handoff boundary
Hand off **Slice A first** as the initial Forge task.

Why:
- it establishes the new persistence seam and visible artifact
- it validates the Day 0 promise before adding the ritual layer
- it reduces review surface if the first pass needs tightening

Immediately queue **Slice B** as the follow-on task using the same spec packet once Slice A is accepted.

---

## Immediate blocker check
**No blocker prevents spec freeze now.**

Operational note only:
- the routed note referenced `shared/state/gaia/mission-control/deliverables/...`, but the source memo bundle was actually present under `workspaces/gaia/shared/state/gaia/mission-control/deliverables/...`. That path mismatch was resolved during spec assembly and does not block build freeze.

## Source bundle used
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-decision-sheet.md`
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-first-experiment-brief.md`
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-architect-handoff-seed.md`
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-v0-scope-freeze.md`
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-starter-loop-defaults.md`
- `/home/ubuntu/.openclaw/families/loki/workspaces/gaia/shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-founder-approval-2026-06-11.yaml`
