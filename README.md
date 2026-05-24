# acc-ledger

`acc-ledger` is a reusable accounting ledger semantic module/kernel.

The repository is intended to grow into a ledger module that can later compose with adjacent modules such as VAT, reporting, and other institutional accounting capabilities.

## Architectural Direction

- Semantic module first, technical concerns second.
- Separate the ledger ontology/kernel from application and infrastructure concerns.
- Keep kernel semantics focused on ontological objects and institutional concepts.
- Keep infrastructure, policies, persistence, APIs, CQRS handlers, projections, and accounting behavior outside the kernel until they have explicit architectural shape.

## Repository Structure

```text
src/
  ACC.Ledger.Kernel/
  ACC.Ledger.Application/
  ACC.Ledger.Projections/

tests/
  ACC.Ledger.Kernel.Tests/
  ACC.Ledger.Application.Tests/

docs/
  ontology/
  invariants/
  decisions/
  diagrams/
```

## Current Scope

This repository currently contains only semantic and architectural scaffolding. It intentionally does not implement business logic, persistence, APIs, CQRS handlers, event sourcing, projections, or accounting behavior.
