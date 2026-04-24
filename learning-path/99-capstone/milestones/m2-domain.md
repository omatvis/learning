# m2 — Domain Model

> Define the core domain entities, value objects, and business rules.

## Goals

- Model the core domain in `Capstone.Domain` with zero framework dependencies.
- Write unit tests for domain logic.

## Tasks

- [ ] Define primary entities (e.g. `Task`, `User`, `Project` — finalise with Copilot).
- [ ] Add value objects where appropriate (e.g. `Email`, `TaskStatus`).
- [ ] Define domain interfaces (e.g. `ITaskRepository`).
- [ ] Add domain events if needed.
- [ ] Write unit tests in `Capstone.UnitTests` for all domain rules.

## Acceptance criteria

- [ ] `Capstone.Domain` has **no** NuGet references to frameworks.
- [ ] All domain rules are unit-tested.
- [ ] Entity invariants are enforced in constructors / factory methods.
