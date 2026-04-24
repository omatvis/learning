# m4 — API Layer

> Implement the Application use-cases and expose them through the API.

## Goals

- Add CQRS commands and queries in `Capstone.Application`.
- Expose them via controllers or endpoint groups in `Capstone.Api`.
- Add input validation, error handling, and OpenAPI documentation.

## Tasks

- [ ] Implement CRUD use-cases (commands + queries) in `Application`.
- [ ] Wire up controllers/endpoints in `Api`.
- [ ] Add `FluentValidation` for input validation.
- [ ] Return `ProblemDetails` for all errors.
- [ ] Configure Swagger / OpenAPI.
- [ ] Add JWT authentication (extend from sp-05 learnings).
- [ ] Write integration tests covering all endpoints.

## Acceptance criteria

- [ ] All endpoints documented in Swagger.
- [ ] Unauthenticated requests to protected endpoints return 401.
- [ ] Validation errors return structured `ProblemDetails`.
- [ ] Integration tests pass.
