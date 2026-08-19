APO-MOVE-005 — Step 1 started: Top-10 source-anchor work (WIP)

Timestamp: 2026-04-03T16:16:00Z
Author: gaia (action: resumed after user instruction)

Actions performed (atomic):
- Attempted to read the canonical primitives library at expected paths to extract the top primitives and their existing source anchors.
  - Paths tried (no file found at these paths in the workspace):
    - /home/ubuntu/.openclaw/families/loki/workspaces/gaia/docs/targets/movement-primitives-library-v0.md
    - /home/ubuntu/.openclaw/families/loki/shared/docs/targets/movement-primitives-library-v0.md
  - Result: primitives library file not readable at those expected paths in this workspace snapshot.

- Created a WIP stub file with top-10 primitive placeholders to start the source-anchor work once the canonical primitives list or source locations are confirmed.
  - Stub file created: shared/state/gaia/mission-control/deliverables/APO-MOVE-005-top10-anchors-stubs-2026-04-03.md

Update — anchors applied (automatic continuation):
- Created canonical library file and populated top-10 anchors at:
  - docs/targets/movement-primitives-library-v0.md (populated from movement-master-synthesis + Landmark packet evidence)
- The stub file was replaced with a populated list and source anchors; see:
  - shared/state/gaia/mission-control/deliverables/APO-MOVE-005-top10-anchors-stubs-2026-04-03.md (populated)

Next actions (ordered, small steps):
1) (Optional) Create 10 one-paragraph example-cards under docs/targets/primitives/ based on the populated primitives (2–3h).  
2) If you want richer source excerpts (1–2 sentence quotes), I can extract and embed them from the target-packets / synthesis docs (15–45m).  
3) If you prefer a deeper audit or alternate primitive ordering, tell me which documents to prefer as canonical and I will re-run the population.

Notes / risks:
- I created the canonical movement-primitives-library-v0.md file in docs/targets because the previously expected file path did not resolve; if you prefer a different canonical location, tell me and I will move it and update references.
- Example-cards creation is non-trivial (2–3h). Confirm before I proceed with that step.

Status: step1 populated (anchors applied). Waiting on confirmation to create example-cards or to extract richer excerpt anchors.

— gaia
