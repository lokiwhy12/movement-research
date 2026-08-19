# Primitive: Portable canon / drift-control architecture

What it is

A compact pattern for preserving an authoritative, portable subset of doctrine (the "canon") while allowing the broader body of doctrine, examples, and paraphernalia to evolve. The primitive supplies a minimal, stable kernel that operators can distribute and reference, plus a drift-control policy that ensures local variants remain interoperable with the canonical core.

Mechanics

- Canon kernel: a 1–3 paragraph statement of core rules, commitments, and non-negotiables that define the practice's identity.
- Translation map: a tiny mapping table that ties canonical terms to local-language synonyms and permitted local ritual variations.
- Versioned release cadence: canonical patches (minor/major) and an explicit compatibility window that limits how long a local variant may diverge without explicit re-alignment.
- Drift-control triggers: agreed signals (e.g., >3 local edits to core ritual, new admission scripts, or monetization changes) that prompt a reconciliation event with an authoritative operator or review committee.

Examples

- A coaching method publishes a one-page "Foundational Rules" document (the kernel) and a FAQ mapping common local phrasing back to canonical terms. Local chapters may add examples but must run a quarterly compatibility check with HQ.
- A community ritual keeps the canonical script in a single short file; any local edits must be tagged and submitted for review when they exceed the documented deviation threshold.

Risks / Misuse

- Canon capture: a small canon can be weaponized to lock in exploitative defaults (e.g., mandatory fees) if governance is weak.
- False-stability illusion: having a canon does not guarantee ethical practice; minimal canon may hide harmful processes in ancillary materials.
- Overcentralization: excessive re-alignment demands can stifle local agency and lead to fragmentation.

Safe-translation / Guardrails

- Publish the canon under a clear license and include an explicit ethical constraint clause (Section G-style mitigations) that forbids predatory monetization or coercive escalation paths.
- Keep the kernel minimal and focused on structural invariants (roles, consent rules, escalation gates) rather than procedural minutiae.
- Define a lightweight, time-bounded reconciliation protocol: local operator files a drift report, a 7-day window opens for automated/peer review, and only then does a formal decision require higher-level signoff.

Next steps

- Anchor the primitive in the movement-primitives library (`shared/docs/targets/movement-primitives-library-v0.md`) with a one-line registry entry.
- Create an example reconciliation checklist and a one-page canonical kernel file to use as a template for future target packets.

---

artifact: shared/docs/targets/primitives/portable-canon-drift-control-architecture.md
