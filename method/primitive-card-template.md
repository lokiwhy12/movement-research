# Primitive Card Template

Title: <primitive-name>
One-line summary: <one-sentence explanation of the primitive and its role>

Mechanic:
- Short description of how the primitive operates (mechanics, actors, and visible signals)

Lifecycle slot:
- e.g. pre-start / active / post-end / recurring / onboarding / retention

Evidence anchors:
- Source 1 (URL / doc path / quote)
- Source 2

Examples (short):
- Example 1 — short, concrete instance
- Example 2

Use cases / translation notes:
- When to apply this primitive safely
- What it looks like in product/content/context

Shadow risks:
- Risk 1 (what can go wrong / abusive translation)
- Risk 2

Safe-translation checklist:
- [ ] Evidence anchors verified and cited
- [ ] Small mitigations for top shadow risks documented
- [ ] Explicit human review required for any live deployment

Reconciliation checklist (for APO-MOVE reconciliation pass):
- [ ] Confirm canonical shared/docs/targets/primitives/<primitive-name>.md exists
- [ ] Populate "Evidence anchors" with at least 2 public-source excerpts
- [ ] Fill "Examples" with at least 2 concrete cases and one minimal mitigation
- [ ] Run small-risk audit and add mitigation notes under "Shadow risks"
- [ ] Mark library entry complete and update movement-primitives-library-v0.md index

Notes:
- Use this template to standardize primitive cards before merging into the movement-primitives library.
- Keep language factual and source-anchored; avoid persuasive amplification.
