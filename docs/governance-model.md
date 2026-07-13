# Governance model

ZipVerse treats an AI-agent team as a set of governed roles operating inside an explicit authority boundary.

## Governed roles

A role is defined by responsibility, permitted capabilities, expected inputs, and required outputs. A role is not granted unrestricted authority simply because the underlying model is capable of more.

Illustrative roles include:

- **Supervisor** — routes approved work and enforces the execution boundary.
- **Builder** — produces an implementation or artefact within the approved scope.
- **Reviewer** — independently checks the builder output against the task and validation requirements.
- **Researcher** — gathers bounded evidence without changing the target system.
- **Handoff role** — packages state and evidence for the next governed step.

These names are illustrative public concepts, not a disclosure of private runtime configuration.

## Governance sequence

1. Capture operator intent.
2. Compile it into a task packet.
3. Lock the scope and permissions.
4. Resolve required approvals.
5. Route the packet to permitted roles.
6. Record structured handoffs and outcomes.
7. Return a result envelope with status and evidence references.

## Separation of duties

Where practical, the role generating work should not be the only role validating it. Independent review reduces self-confirming errors and makes acceptance criteria visible.

## Determinism

In this context, deterministic governance means that the same locked packet, policy state, and approval state should lead to the same authority decision: allow, reject, hold, or require approval. It does not claim that language-model prose will always be byte-for-byte identical.

## Human authority

Human approval remains explicit at configured boundaries. The public schemas represent approval as a separate object so that approval is not confused with a model's recommendation.
