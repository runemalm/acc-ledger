# acc-ledger

`acc-ledger` is an accounting ledger semantic module.

The repository is intended to grow into a ledger module that can later compose with adjacent modules such as VAT, reporting, and other institutional accounting capabilities.

## Architecture

The solution separates the institutional ontology from its software realization:

- `ACC.Ledger.Ontology` contains the semantic ledger reality: acts, continuities, facts, invariants, observations, and primitives.
- `ACC.Ledger.Realization` contains operational/materialized structures such as projections.

## Current Scope

This repository currently contains semantic scaffolding only. It intentionally does not implement business logic, persistence, APIs, event sourcing, projection runners, or infrastructure concerns.
