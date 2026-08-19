# APO-MOVE-005 Executive Memo — Architect Handoff Seed

Task: `APO-MOVE-005-MEMO-20260528`
Project: `monolith`
Prepared by: Gaia
Prepared on: 2026-06-05

## Purpose
Pre-package the recommended first experiment so founder approval can convert into an Architect kickoff without another translation pass.

## Approval gate
This packet is **conditional**.
Use it only if Loki approves the current recommendation:
- **pull-factor onboarding** + **ritual map**
- shipped as the **24-hour starter loop**

## Product outcome
A new user should leave the first session with:
1. one visible win
2. one saved artifact
3. one obvious next action for the next day

## Recommended v0 shape
### 1) Day 0 visible win
Return one personalized **Clarity Card** at the end of onboarding.

Minimum payload:
- one named pattern or friction point
- one leverage insight in plain English
- one specific next move for the next 24 hours

### 2) Saved artifact
Persist that card as a **Day 0 Snapshot** on the user's home/timeline surface.

Minimum fields:
- title
- one-sentence insight
- one next action
- timestamp

### 3) Day 1 return loop
Offer a **2-minute session-driven check-in** the next day.

Prompt set:
- did yesterday's next move happen?
- what changed?
- what is today's smallest next move?

Output:
- progress trace or revised next move attached to the original snapshot

## Acceptance criteria
A v0 build is successful when a new user can:
1. finish onboarding
2. receive one Clarity Card before exit
3. find the Day 0 Snapshot later
4. complete the next-day check-in in under 2 minutes

## Instrumentation minimum
Track:
- onboarding completion
- Clarity Card delivered
- Day 0 Snapshot viewed later
- day-1 return rate
- next-day ritual completion rate
- median completion time for the ritual

## Safe-translation constraints
Keep:
- clarity
- momentum
- visible progress
- repeatability

Avoid:
- shame loops
- coercive streaks
- exclusivity signaling
- intensity escalation as retention glue
- manipulative pressure mechanics

## What Architect should decide next
1. what exact inputs generate the Clarity Card in v0
2. where the Day 0 Snapshot lives in the product surface
3. whether the day-1 ritual updates the same card or creates a linked Day 1 card
4. what smallest milestone split gets this into a buildable spec fastest

## Suggested downstream split
### Architect
- convert this seed into a milestone/spec packet
- define the user flow and product states
- choose the minimal data model for Day 0 / Day 1 artifacts

### Forge
- implement once Architect freezes the flow
- instrument the metrics above from the first build

## Source bundle
This handoff seed depends on:
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28.md`
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-decision-sheet.md`
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-first-experiment-brief.md`
- `shared/state/gaia/mission-control/deliverables/APO-MOVE-005-exec-memo-2026-05-28-starter-loop-defaults.md`

## Why this exists
Founder approval is still the gate. This file removes the post-approval stall by turning the memo recommendation into a ready-to-route implementation seed.