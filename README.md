# ZipVerse SDK

**Public integration contracts, examples, and mock surfaces for governed AI-agent execution.**

ZipVerse is being developed as a deterministic governance layer for teams of AI agents. It is designed to turn operator intent into bounded task packets, apply explicit permissions and approvals, coordinate governed roles, and return structured, auditable results.

This repository is the **public integration layer**. It does not contain the private ZipVerse engine, internal orchestration logic, production dictionaries, provider-routing logic, private validation evidence, or proprietary runtime code.

## Core ideas

- **Locked intent** — the requested task is represented as a stable task packet.
- **Bounded authority** — tools, scope, permissions, and approval requirements are explicit.
- **Governed roles** — agents operate through defined responsibilities rather than unrestricted autonomy.
- **Structured handoffs** — work moves between roles through machine-readable packets.
- **Auditable outcomes** — results carry status, evidence references, and execution metadata.

## Public repository map

```text
docs/             Public concepts, boundaries, and roadmap
examples/         Illustrative task packets and governed-run examples
public_schemas/   Draft public JSON Schemas
mock_runtime/     Description of the planned local mock surface
sdk/              Future client-library surface
```

## Illustrative flow

```text
Operator intent
  -> task packet
  -> policy and approval checks
  -> governed execution
  -> structured result envelope
```

Start with:

- [What is ZipVerse?](docs/what-is-zipverse.md)
- [Governance model](docs/governance-model.md)
- [Public integration boundary](docs/integration-boundary.md)
- [Example task packet](examples/basic-task-packet.json)

## Status

This is an early public contract repository. The schemas and examples are intentionally implementation-neutral and may change before a versioned SDK release.

## Licence

A public-source licence has not yet been selected. Until a licence file is added, publication of this repository does not itself grant permission to copy, modify, or redistribute its contents.
