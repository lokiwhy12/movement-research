# APO-MOVE-008 — OneTaste packet docs-side sync

Timestamp: 2026-06-25T19:00:00Z (UTC)

Summary
- Reconciled the canonical `docs/targets/onetaste.target-packet.md` copy from the substantive shared packet so the active OneTaste lane no longer points at a stale skeleton.

Work completed (atomic)
- Replaced the stale skeleton at `docs/targets/onetaste.target-packet.md` with the full packet content already present in `shared/docs/targets/onetaste.target-packet.md`.
- Updated the docs-side header timestamp to `2026-06-25T19:00:00Z` and added a sync note documenting the reconciliation.

Verification
- `diff -u shared/docs/targets/onetaste.target-packet.md docs/targets/onetaste.target-packet.md` now shows only the intentional docs-side timestamp + sync-note header changes.

Next logical step
- Continue the OneTaste finishing pass by tightening either the pull-factor matrix or the protocol map directly inside the docs-side canonical packet.
