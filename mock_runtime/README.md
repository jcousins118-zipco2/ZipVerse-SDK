# Mock runtime

The planned mock runtime will provide a local, non-production implementation of the public ZipVerse contracts.

It is intended to help integrators:

- validate task packets;
- test approval-required and rejected states;
- parse result envelopes;
- build adapters without access to the private engine.

The mock runtime will not contain production policies, private orchestration logic, provider routing, or execution authority.

## Planned behaviour

Given a public task packet, the mock may return deterministic sample states such as:

- `accepted`
- `rejected`
- `approval_required`
- `completed`
- `held`

No code has been published here yet. The first implementation will be added only after the public contracts are reviewed and versioned.
