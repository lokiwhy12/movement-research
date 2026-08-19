# APO-MOVE-005 Executive Memo — Decision Sheet

Task: `APO-MOVE-005-MEMO-20260528`
Project: `monolith`
Prepared by: Gaia
Prepared on: 2026-06-02

## Purpose
Reduce founder review to one concrete decision: which primitive should become the first Apotheosis product experiment.

## Scoring lens
- **Activation speed** — how quickly this can improve day-0 / week-1 user response
- **Retention lift** — how strongly this should affect repeat use
- **Build complexity** — lower is better for the first experiment
- **Measurement clarity** — how easy it is to tell whether it worked
- **Brand safety** — how safely this translates into outward product behavior

Scale: 1-5 where **5 = best first-experiment fit**.

| Primitive | Activation speed | Retention lift | Build simplicity | Measurement clarity | Brand safety | First-pass take |
|---|---:|---:|---:|---:|---:|---|
| Pull-factor onboarding | 5 | 4 | 4 | 5 | 5 | Excellent immediate test candidate |
| Ritual map | 4 | 5 | 4 | 4 | 5 | Excellent paired candidate with onboarding |
| Compact doctrine | 3 | 3 | 5 | 3 | 5 | Strong support asset, weaker first standalone test |
| Felt alignment | 4 | 4 | 3 | 3 | 4 | Useful, but slightly softer to measure first |
| Container + portability | 2 | 4 | 2 | 3 | 5 | Important later-system design question, not first test |
| Transparency + room legibility | 3 | 3 | 4 | 3 | 5 | Strong trust layer, better as parallel governance copy |

## Recommendation
**Start with a combined experiment:**
1. **Pull-factor onboarding** as the front-door mechanic
2. **Ritual map** as the repeat-use mechanic

Why this pair wins:
- It hits the two earliest leverage points: activation and return behavior.
- It is easy to explain in plain English: “show value fast, then give the user a repeatable daily loop.”
- It is measurable without a heavy analytics rewrite.
- It stays safely inside mainstream product behavior.

## Proposed v0 experiment brief
**Experiment name:** 24-hour starter loop

**User promise:** In the first 24 hours, the user gets one visible win, one saved trace of progress, and one clear next action.

**Flow:**
1. User finishes onboarding
2. Product delivers one fast personalized insight or action
3. Product saves a visible artifact (checkpoint, score, reflection, or commitment)
4. Product schedules one lightweight follow-up ritual for the next day

## Success signals
- Higher onboarding completion rate
- More users returning on day 1 / day 2
- More users completing the first repeat ritual

## Founder decision options
- **Approve pair** — move to downstream translation of onboarding + ritual experiment
- **Approve single primitive** — choose one primitive only for the first build
- **Re-rank** — keep the six, but change the starting order
- **Hold** — keep as reference only, no immediate translation
