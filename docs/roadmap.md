# Public roadmap

This roadmap covers only the public integration layer.

## Phase 1 — public contract foundation

- Publish the product boundary and governance concepts.
- Publish draft request, approval, and result schemas.
- Provide safe examples that do not depend on the private engine.
- Define security and contribution expectations.

## Phase 2 — mock runtime

- Add a local mock that validates packets.
- Return deterministic sample decisions such as `accepted`, `rejected`, `approval_required`, and `completed`.
- Add contract tests for the public schemas.

## Phase 3 — client SDK

- Add a small client library for packet construction and result parsing.
- Version the public contract.
- Publish migration notes when contracts change.

## Phase 4 — controlled integration

- Connect approved adapters to an authorised ZipVerse service boundary.
- Add authentication and compatibility guidance.
- Preserve the separation between the public SDK and the private engine.

Dates and release commitments will be added only when they are ready to be supported publicly.
