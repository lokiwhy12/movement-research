# APO-MOVE-005 Executive Memo — Approval Capture Card

Task: `APO-MOVE-005-MEMO-20260528`
Project: `monolith`
Prepared by: Gaia
Prepared on: 2026-06-06

## Purpose
Turn a short founder voice/text reply into a structured record that Gaia can act on immediately without a second interpretation pass.

## Founder reply shortcut
If Loki wants the shortest possible answer path, he can reply with one of these:

- **APPROVE_PAIR** — use pull-factor onboarding + ritual map as the first experiment
- **APPROVE_SINGLE: <primitive>** — start with one primitive only
- **REORDER: <top order or top 3>** — keep the six, change the priority stack
- **TIGHTEN: <what to sharpen>** — keep the structure, revise claim/example/tone
- **HOLD** — keep the packet as reference only for now

Voice-safe equivalents are already covered by the voice review script; this card is the capture grammar behind that surface.

## Canonical capture fields
Record these fields after the founder reply:
1. `branch`
2. `approved_primitives`
3. `starter_loop_survives_unchanged`
4. `route_architect_now`
5. `requested_edits`
6. `source_reply`

## Copy/paste capture template
```yaml
branch: approve-pair | approve-single | re-rank | tighten | hold
approved_primitives:
  -
starter_loop_survives_unchanged: yes | no
route_architect_now: yes | no
requested_edits: ""
source_reply: ""
```

## Branch-to-action map

### 1) approve-pair
- `approved_primitives`: `pull-factor onboarding`, `ritual map`
- `starter_loop_survives_unchanged`: `yes`
- `route_architect_now`: `yes`
- immediate action: route `APO-MOVE-005-exec-memo-2026-05-28-architect-handoff-seed.md`

### 2) approve-single
- `approved_primitives`: exactly one primitive
- `starter_loop_survives_unchanged`: usually `no`
- `route_architect_now`: `no` until a single-primitive variant is created
- immediate action: clone and narrow the experiment brief/defaults/handoff seed

### 3) re-rank
- `approved_primitives`: top-ranked set after reordering
- `starter_loop_survives_unchanged`: `yes` only if onboarding+ritual still wins
- `route_architect_now`: `yes` only if the existing recommendation survives
- immediate action: update quick-review + decision sheet, then regenerate downstream artifacts if the top experiment changes

### 4) tighten
- `approved_primitives`: current set unchanged unless founder says otherwise
- `starter_loop_survives_unchanged`: usually `yes`
- `route_architect_now`: `no` until edits are applied
- immediate action: edit the source memo first, then propagate wording changes into companion artifacts

### 5) hold
- `approved_primitives`: none newly approved
- `starter_loop_survives_unchanged`: `n/a`
- `route_architect_now`: `no`
- immediate action: leave task in review and preserve the packet as dormant reference material

## What this unblocks
This card closes the last operational gap between founder feedback and action logging: Gaia now has a single, explicit structure for capturing approval and deciding whether Architect can be routed immediately.