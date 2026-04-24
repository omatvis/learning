# Conventions — .NET Clean Architecture (capstone)

> Rules for the capstone project (`projects/capstone/capstone-app/backend`).

## Layer responsibilities

| Layer | Allowed dependencies | Responsibilities |
|-------|---------------------|-----------------|
| `Domain` | None | Entities, value objects, domain events, interfaces |
| `Application` | Domain | Use-cases / commands / queries (CQRS), ports (interfaces) |
| `Infrastructure` | Application (→ Domain via transitive ref for entity mapping) | EF Core, SQL, external services, adapters |
| `Api` | Application | HTTP controllers/endpoints, DI wiring, middleware |

## Rules

- `Domain` must have **zero** references to frameworks (no EF Core, no ASP.NET).
- `Application` defines interfaces; `Infrastructure` implements them.
- Use CQRS: separate `Commands/` and `Queries/` folders in `Application`.
- Validation lives in `Application` (not in controllers).
- `Api` layer is thin: validate → dispatch → return.
- Async all the way — no `.Result` / `.Wait()`.
- Parameterize all queries; avoid raw string-concatenated SQL.
- Return `ProblemDetails` for all error responses.
- Every use-case has a corresponding unit test in `Capstone.UnitTests`.
- Integration tests in `Capstone.IntegrationTests` use a real (test) database.
