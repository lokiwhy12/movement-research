# APO-MOVE Document Map (canonical entrypoint)

Status: active as of 2026-03-16.

Purpose: make the APO-MOVE / movement-DNA folder readable as a system instead of a pile of artifacts.

## What APO-MOVE is

APO-MOVE is a **movement-DNA research program**.
It exists to:
- build a database of movement cases
- extract and compare the mechanics that make movements work
- separate useful mechanics from coercive/pathological ones
- produce analytical tools that can later inspire Monolith

It is **not** currently a direct movement-design project.

Canonical scope doc:
- `movement-dna-program-scope-v1.md`

---

## Recommended reading order

If you are orienting fresh, read in this order:

1. **`movement-dna-program-scope-v1.md`**
   - governing scope and boundary doc
   - defines current mission and Monolith downstream-use rule

2. **`../MOVEMENT_EXTRACTION_CHECKLIST.md`**
   - per-target intake form
   - use this to dissect a single movement cleanly

3. **`movement-mechanic-rating-system-v0.md`**
   - post-extraction scoring / comparison framework
   - use this to profile mechanics across potency, risk, durability, etc.

4. **`../MOVEMENT_LEXICON_AND_NAMING_LOG.md`**
   - language-system DNA ledger
   - use this to track naming, slogans, role labels, compressed vocabulary, and in-group language across cases

5. **`movement-dna-taxonomy-v0.md`**
   - full extraction schema / concept map
   - use this as the master list of analytical dimensions

6. **`movement-primitives-library-v0.md`**
   - canonical registry of reusable mechanics + current example-card coverage
   - use this when you want the cross-case primitive layer instead of a single target packet

7. **`movement-unfiltered-reaudit-v1.md`**
   - comparative synthesis sweep across the current corpus
   - useful for seeing the big patterns before diving into individual target packets

8. **`movement-target-roster-v1.md`**
   - active corpus-planning roster
   - tells you what has already been covered and what should be added next

---

## Current live work surfaces

**Canonical path note:** treat `docs/targets/` as the primary readable corpus. `shared/docs/targets/` may contain legacy mirrors for Mission Control / backfill-card compatibility, but the docs-side packet should never be allowed to drift into a weaker placeholder than its shared mirror.

### APO-MOVE-002 — Landmark deep pass
Primary working docs:
- `landmark-forum.target-packet.md`
- `landmark-forum.glossary-and-protocol-v0.md`
- `landmark-forum.essence.md`

### APO-MOVE-005 — movement-DNA synthesis
Primary working docs:
- `movement-dna-program-scope-v1.md`
- `movement-dna-taxonomy-v0.md`
- `movement-primitives-library-v0.md`
- `movement-unfiltered-reaudit-v1.md`
- `movement-mechanic-rating-system-v0.md`
- `movement-target-roster-v1.md`

### APO-MOVE-007 — language / naming-pattern analysis
Primary working doc:
- `../MOVEMENT_LEXICON_AND_NAMING_LOG.md`

---

## Folder structure by role

### 1) Governance / scope
These define what the project is and is not.
- `movement-dna-program-scope-v1.md`
- `README.md` (this file)

### 2) Core analytical infrastructure
These are the reusable frameworks.
- `../MOVEMENT_EXTRACTION_CHECKLIST.md`
- `movement-mechanic-rating-system-v0.md`
- `../MOVEMENT_LEXICON_AND_NAMING_LOG.md`
- `movement-dna-taxonomy-v0.md`
- `movement-primitives-library-v0.md`

### 3) Corpus planning / comparative synthesis
These help decide what to study and what patterns are emerging.
- `movement-target-roster-v1.md`
- `movement-unfiltered-reaudit-v1.md`

### 4) Case files / target packets
These are the main database entries per movement.
- `75-hard.target-packet.md`
- `ala-austin.target-packet.md`
- `alcoholics-anonymous.target-packet.md`
- `apple-marketing.target-packet.md`
- `crossfit.target-packet.md`
- `landmark-forum.target-packet.md`
- `nxivm-esp.target-packet.md`
- `onetaste.target-packet.md`
- `qanon.target-packet.md`
- `scientology.target-packet.md`
- `the-secret.target-packet.md`
- `tony-robbins.target-packet.md`
- `peloton.target-packet.md`
- `burning-man.target-packet.md`
- `lds-mormon.target-packet.md`

### 5) Deep-dive / case-specific supporting analysis
These deepen a specific target beyond the packet level.
- `landmark-forum.glossary-and-protocol-v0.md`
- `landmark-forum.essence.md`

### 6) Primitive example cards
These make a single mechanic concrete with examples, risk notes, and safe-translation guidance.
- `primitives/compact-doctrine.md`
- `primitives/threshold-ritual.md`
- `primitives/rehearsal-assignments-that-leave-the-room.md`
- `primitives/daily-micro-rituals-measurable-trace.md`
- `primitives/micro-ritual-persistence.md`
- `primitives/public-commitment-witness.md`
- `primitives/ritual-signature-compact.md`
- `primitives/testimony-loop-narrative-proof.md`
- `primitives/confessional-inventory-loop.md`
- `primitives/program-over-personality.md`
- `primitives/dyadic-operator-channels.md`
- `primitives/distributed-node-architecture.md`
- `primitives/visible-ladder-status-economy.md`
- `primitives/compressed-timebox-flagship-event.md`
- `primitives/branded-distinctions-cognitive-handles.md`
- `primitives/member-to-operator-pipeline.md`

### 7) Supporting extracts / source distillations
These are not first-class target packets; they are supporting analytical inputs.
- `boodaism-lgat-extract-v0.md`
- `crimereads-cult-steps-extract-v0.md`
- `how-to-become-a-cult-leader-series-extract-v0.md`
- `how-to-become-a-cult-leader-transcript-paths-v0.md`

Use these for additional mechanics signal, not as the main database backbone.

### 8) Historical / superseded framing
These are preserved for traceability, but they are **not** the governing frame now.
- `movement-blueprint-v0.md`
- `movement-blueprint-v1.md`
- `movement-target-roster-v0.md`

Important note:
- those blueprint docs may still contain useful extracted thinking
- they should be treated as historical artifacts from the earlier, now-superseded movement-design framing

---

## Monolith downstream-use rule

The database built here is meant to become an inspiration/input layer for **Monolith** later.
That means the research should stay focused on:
- observed mechanics
- comparative analysis
- mechanism/risk tradeoffs
- reusable primitives

Not on:
- directly naming Monolith elements inside every research file
- prematurely drafting Monolith doctrine
- turning every analytical file into a design brainstorm

The translation layer comes later.
The database comes first.

---

## Naming convention / interpretation guide

### `*.target-packet.md`
A first-class case entry for the database.

### `*-extract-v0.md`
A supporting extract from a source/article/show. Useful, but not the main record.

### `*-taxonomy-*`, `*-rating-*`, `*-scope-*`
Framework docs: reusable analytical infrastructure.

### `*-roster-*`
Corpus planning docs.

### `*-blueprint-*`
Historical artifacts from the older movement-design framing.

---

## If you only read three files

Read these:
1. `movement-dna-program-scope-v1.md`
2. `movement-dna-taxonomy-v0.md`
3. `movement-target-roster-v1.md`

That gives you:
- the mission
- the schema
- the current corpus plan

---

## Bottom line

This folder is now organized around one workflow:

**extract -> rate -> compare -> synthesize -> later translate into Monolith inspiration**

If a file does not clearly support one step in that chain, it should be treated as secondary or historical.
