Portable Canon Drift Control — Reconciliation Checklist

This checklist helps reconcile "portable canon / drift-control" primitive artifacts and restore a single canonical source of truth.

1) Confirm canonical sources
   - Locate and list the canonical primitive file(s) and any linked deliverables or evidence anchors.
   - Confirm canonical README/registry entries (movement-primitives-library-v0.md, docs/targets/README.md).

2) Inventory drift points
   - List files/paths that diverge from canonical language or behavior (code, docs, artifact paths).
   - Record who last edited each divergent file and the edit timestamp.

3) Decide canonical interpretation
   - For each drift point, choose: (A) adopt drift as new canonical, (B) merge/alias into canonical, or (C) revert to prior canonical.
   - Record rationale and acceptance criteria for the chosen option.

4) Create concrete reconciliation tasks
   - For each adopted/merged decision, create a small task with file-scope, owner, and acceptance criteria (unit: 1–3 files).
   - Schedule follow-up: review PR + smoke test + update primitive registry.

5) Implement and test
   - Apply code/doc edits in a single scoped PR per reconciliation decision.
   - Add minimal tests or a documentation smoke check where applicable.

6) Verify and close
   - Confirm PR merged, artifacts updated, and movement-primitives-library reflects the final path.
   - Update deliverable and task notes with the reconciliation outcome.

7) Post-mortem (optional)
   - Record why the drift occurred and add a short mitigation bullet to prevent recurrence (guardrails, cadence, or ownership change).

Next step: expand this checklist into a primitive-card-friendly template and register it in the movement-primitives library as a reconciliation pattern.