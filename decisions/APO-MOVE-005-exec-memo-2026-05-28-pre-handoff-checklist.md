# APO-MOVE-005 Executive Memo — Founder-to-Architect Pre-Handoff Checklist

Task: `APO-MOVE-005-MEMO-20260528`
Project: `monolith`
Prepared by: Gaia
Prepared on: 2026-06-09

## Purpose
Turn the existing memo packet into a single operational checklist so founder approval can convert into Architect routing without missing a dependency or reopening the packet stack.

## Approval gate
Do not route this packet forward until Loki gives one of the canonical founder replies:
- `APPROVE_PAIR`
- `APPROVE_SINGLE: <primitive>`
- `REORDER: <top 3 or top order>`
- `TIGHTEN: <edit>`
- `HOLD`

## Required packet pieces before routing
- [x] Core executive memo (`APO-MOVE-005-exec-memo-2026-05-28.md`)
- [x] Founder-review PDF (`APO-MOVE-005-exec-memo-2026-05-28.pdf`)
- [x] Quick-review companion (`APO-MOVE-005-exec-memo-2026-05-28-quick-review.md`)
- [x] Decision sheet (`APO-MOVE-005-exec-memo-2026-05-28-decision-sheet.md`)
- [x] First-experiment brief (`APO-MOVE-005-exec-memo-2026-05-28-first-experiment-brief.md`)
- [x] Voice-review script (`APO-MOVE-005-exec-memo-2026-05-28-voice-review-script.md`)
- [x] Starter-loop defaults card (`APO-MOVE-005-exec-memo-2026-05-28-starter-loop-defaults.md`)
- [x] Founder response routing map (`APO-MOVE-005-exec-memo-2026-05-28-founder-response-routing-map.md`)
- [x] Approval-capture card (`APO-MOVE-005-exec-memo-2026-05-28-approval-capture-card.md`)
- [x] Architect handoff seed (`APO-MOVE-005-exec-memo-2026-05-28-architect-handoff-seed.md`)
- [x] v0 scope freeze (`APO-MOVE-005-exec-memo-2026-05-28-v0-scope-freeze.md`)
- [x] Loki direct review prompt (`APO-MOVE-005-exec-memo-2026-05-28-loki-direct-review-prompt.md`)

## Founder reply -> immediate branch
### If Loki replies `APPROVE_PAIR`
- Capture approval using the approval-capture card.
- Route the Architect handoff seed + scope freeze as the default implementation bundle.
- Keep the recommended experiment as **pull-factor onboarding + ritual map** shipped as the **24-hour starter loop**.

### If Loki replies `APPROVE_SINGLE`
- Narrow the packet to the approved primitive.
- Update the first-experiment brief and scope freeze before routing anything downstream.

### If Loki replies `REORDER`
- Update the decision sheet, quick-review companion, and any downstream artifact whose winner changed.
- Only re-route after the new winner has a matching brief + defaults + scope boundary.

### If Loki replies `TIGHTEN`
- Edit the memo language first.
- Recheck whether the quick-review companion, direct review prompt, or scope freeze needs matching edits.

### If Loki replies `HOLD`
- Leave the task in review.
- Do not route to Architect.
- Treat the packet as ready reference material, not an active build handoff.

## Default Architect bundle on approval
Send these four files first:
1. `APO-MOVE-005-exec-memo-2026-05-28-decision-sheet.md`
2. `APO-MOVE-005-exec-memo-2026-05-28-first-experiment-brief.md`
3. `APO-MOVE-005-exec-memo-2026-05-28-architect-handoff-seed.md`
4. `APO-MOVE-005-exec-memo-2026-05-28-v0-scope-freeze.md`

Keep the full memo packet available as background, but do not make Architect reconstruct the default path from scratch.

## Completion standard
This packet is handoff-ready when:
- founder reply is captured in canonical grammar
- the chosen branch is unambiguous
- the downstream bundle matches that branch
- Architect can answer "what is the v0, what is out of scope, and what should happen next" from the routed files alone

## Why this exists
The packet already contained the ingredients. This checklist makes the packet executable.