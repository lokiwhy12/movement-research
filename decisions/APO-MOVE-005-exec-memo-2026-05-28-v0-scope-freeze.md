# APO-MOVE-005 Executive Memo — 24-Hour Starter Loop v0 Scope Freeze

Task: `APO-MOVE-005-MEMO-20260528`
Project: `monolith`
Prepared by: Gaia
Prepared on: 2026-06-08

## Purpose
Freeze the recommended starter-loop experiment into a sharp **v0 in/out boundary** so founder approval can convert into Architect scoping without immediate scope creep.

## Approval gate
Use this only if Loki approves the current recommendation:
- **pull-factor onboarding** + **ritual map**
- shipped as the **24-hour starter loop**

## v0 outcome
A first-time user should be able to:
1. finish onboarding
2. receive one personalized **Clarity Card**
3. find the saved **Day 0 Snapshot** later
4. complete one sub-2-minute Day 1 check-in

If those four things work, v0 succeeded.

## In scope for v0
### 1) Onboarding inputs
Capture only the minimum inputs needed to generate a useful Clarity Card.

Allowed:
- a small set of founder-approved intake prompts
- one lightweight pattern inference
- one immediate next move

Not required in v0:
- full profile depth
- long narrative memory capture
- multi-session calibration

### 2) Clarity Card output
Return exactly one visible win at the end of onboarding.

Required fields:
- named pattern or friction point
- one-sentence leverage insight
- one 24-hour next move

### 3) Day 0 Snapshot
Persist the Clarity Card as a saved artifact the user can revisit.

Required fields:
- title
- insight
- next action
- timestamp

### 4) Day 1 ritual
Provide one session-driven follow-up check-in.

Required prompts:
- did yesterday's next move happen?
- what changed?
- what is today's smallest next move?

Required output:
- either a small progress trace or a revised next move attached to the Day 0 Snapshot

### 5) Basic instrumentation
Track only the signals needed to judge activation and repeatability.

Required events:
- onboarding completed
- Clarity Card delivered
- Day 0 Snapshot viewed
- Day 1 check-in started
- Day 1 check-in completed

## Explicitly out of scope for v0
Do **not** pull these into the first build:
- streak systems
- push notification strategy beyond optional placeholders
- social sharing loops
- community or multiplayer mechanics
- deep memory graphing
- comparative scoring/rankings
- advisor/council orchestration layers
- gamified progression ladders
- any shame/urgency pressure mechanic

## Default product rule
If a feature does not directly improve one of the four v0 outcomes above, it waits.

## Architect decisions that still matter
Architect should still decide:
1. the exact onboarding questions
2. where the Day 0 Snapshot lives in the interface
3. whether Day 1 updates the same card or creates a linked entry
4. the smallest milestone split that gets this spec to Forge cleanly

## Why this exists
The memo packet already answers **why** this experiment matters. The handoff seed answers **what** to build first. This scope freeze answers **what not to build yet**, which is the fastest way to keep the first approved version small, legible, and shippable.

## Source bundle
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-first-experiment-brief.md`
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-starter-loop-defaults.md`
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-architect-handoff-seed.md`
