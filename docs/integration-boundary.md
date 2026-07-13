# Public integration boundary

This repository describes the safe boundary between external tools and the private ZipVerse product.

## Public side

The public side may expose:

- versioned request and response schemas;
- client libraries;
- examples;
- mock behaviour;
- compatibility guidance;
- public error and status definitions.

## Private side

The following remain outside this repository:

- runtime implementation;
- internal policy and command dictionaries;
- provider-selection and routing logic;
- private role contracts and orchestration internals;
- production prompts and internal context;
- private tests, evidence packs, audit records, and operational configuration;
- secrets, credentials, customer data, and deployment details.

## Intended contract

An external integration should be able to:

1. construct a valid task packet;
2. submit it to an authorised ZipVerse endpoint or adapter;
3. receive an explicit acceptance, rejection, hold, or approval-required response;
4. receive a structured result envelope after authorised execution.

The external integration should not need access to the engine's internal folder structure or execution logic.

## Draft status

The schemas in `public_schemas/` are illustrative version `0.1` drafts. They are not yet a promise of production API compatibility.
