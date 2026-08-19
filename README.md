# Movement / Monolith — Research Archive

**Rescued from the loki-core server on 2026-08-19, before it is decommissioned.**

This is the complete, merged archive of the movement research program (internally tagged **APO-MOVE**, feeding a downstream product called **Monolith**). It studies why intensely loyal movements work — the mechanics that make people join, stay, climb, and identify — and distills those mechanics into reusable, ethically-annotated "pattern cards."

---

## ⚠️ Read this before anything else

**There are 74 pattern cards, not 18.**

The research existed in two copies on the server, and *neither one was complete*:

| Copy | Location | Cards | Backed up? |
|---|---|---|---|
| "Official" | the shared repo | 18 | ✅ pushed to GitHub + mirrored |
| Gaia's working copy | her private agent folder | 73 | ❌ **no remote, untracked, one machine** |

Only **17 cards overlapped**. That meant **56 cards — the majority of the work — existed in exactly one folder, on one machine, with no backup of any kind.** They were also invisible: the project's own index (preserved at `_misc/ORIGINAL-INDEX-superseded.md`) still lists cards as "to be written" that had in fact been finished months earlier. Anyone opening this project cold would have read that index, believed there were 18 cards, and never found the other 56.

**This archive is the union of both copies.** That is why it supersedes the original index.

Two specific cards the old index claimed were never written — and which are fully written:
- `primitives/protected-disclosure-chamber.md`
- `primitives/self-stabilizing-service-loop.md`

**Eight cards exist in two genuinely different versions.** Gaia's version is fuller for six of them; the official version is fuller for two (notably `testimony-loop-narrative-proof`, where the official copy is nearly double the length). Rather than pick a winner and silently destroy content, **both are preserved**: the primary file in `primitives/` is Gaia's, and the official version sits alongside in `primitives/_official-variants/`. Compare the two before you build on any of these eight.

---

## What's here

```
movement-monolith/                       173 files · 1.5 MB
├── primitives/            74 cards      The reusable mechanics — the core asset
│   └── _official-variants/  8 cards     Alternate versions of 8 cards (see above)
├── cases/                 18 dossiers   The movements studied, one file each
│   ├── analysis/          10 files      Per-case analyses + the cross-case master synthesis
│   └── sources/            4 files      Raw source extracts the dossiers were built from
├── method/                 9 files      How to dissect a movement: extraction checklist,
│                                        taxonomy, mechanic rating system, target roster,
│                                        naming/lexicon ledger, blank card template
├── doctrine/               3 files      "Doctrine Without Doctrine" (the closest thing to
│                                        actual Monolith doctrine) + early blueprints v0/v1
├── decisions/             46 files      The decision trail: audits, the executive memo
│                                        package, the founder approval, the build spec,
│                                        sprint plans, checkpoints, activity ledger
└── _misc/                               The superseded original index, kept for provenance
```

**Movements studied (18 dossiers):** Alcoholics Anonymous · Scientology · NXIVM/ESP · Landmark Forum (plus a deep-dive: essence + 51-term glossary & protocol reconstruction) · CrossFit · 75 Hard · OneTaste · QAnon · LDS/Mormon · Tony Robbins · Peloton · Burning Man · The Secret · Apple marketing · ALA Austin — plus a cross-case "unfiltered re-audit."

> Note: `qanon.target-packet.md` also existed **only** in Gaia's copy. It was not in the backed-up set either.

## The four layers

1. **Method** — how to dissect any movement: an intake checklist, a taxonomy of analytical dimensions, and a scoring system for rating mechanics against each other.
2. **Cases** — full dossiers, one per movement, plus per-case analyses and a cross-case synthesis.
3. **Primitives** — the payoff. Each card isolates one reusable mechanic (e.g. *threshold ritual*, *visible ladder / status economy*, *costly proof / seriousness filter*), with real examples, risk notes, an explicit ethical warning, and guidance on translating it into a product safely. The later cards are written as **contrasting pairs** (e.g. *voluntary affiliation vs. exit-friction ratchet*), which is a more advanced generation than the original set.
4. **Decisions** — what was approved, by whom, and what got built.

## Ethical framing

The project's own governing documents are emphatic that this is **research and pattern-collection, not movement-building** — studying how loyalty mechanics work in order to build honestly, and to recognize them when they're used on you. Individual cards carry their own harm-mitigation notes. Keep that framing attached to this material; out of context it reads very differently than it was written.

## Known gaps (this project is unfinished)

- The **naming/lexicon ledger** covers only about 5 of ~15 catalogued cases.
- The **target roster** explicitly flags that the case mix skewed toward transformation seminars, and plans an expansion into religion, recovery, digitally-native conspiracy movements, failed/decayed movements, and control groups. Some landed; much did not.
- **"Doctrine Without Doctrine"** is small (2.7 KB) but disproportionately important — it proposes *"agency is the root technology"* as the core claim, with a four-layer arc, a draft credo and a ritual cadence. It ends on open questions and is explicitly marked unfinished.
- One approved feature was **never built** — see below.

## The approved-but-unbuilt feature

On **2026-06-11** the founder approved two mechanics for a build: a personalized **"Clarity Card"** at the end of onboarding, saved as a **"Day 0 Snapshot"**, with a **"Day 1 check-in"** ritual. A full build specification was written and frozen the same day (`decisions/APO-MOVE-005-architect-v0-starter-loop-spec-2026-06-11.md`). It was checked against every copy of the app repository: **it was never built.**

The approval and the specification were stored in *different* folders — take only one and you lose half the story. Both are here.

## Provenance

Merged from two locations on loki-core:
- `~/.openclaw/families/loki/shared/docs/targets/` (official, backed up)
- `~/.openclaw/families/loki/workspaces/gaia/shared/docs/targets/` (Gaia's working copy, unbacked)
- Decision trail from both `shared/state/gaia/mission-control/` and `workspaces/gaia/shared/state/gaia/mission-control/`

See `FOUNDER_DIRECTION.md` for the human guidance that produced this work.
