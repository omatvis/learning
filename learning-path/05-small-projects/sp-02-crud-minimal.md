# sp-02 — CRUD API (Minimal API)

> **Goal:** Build a simple CRUD REST API using ASP.NET Core Minimal APIs.

## Project folder

`projects/small/sp-02-crud-minimal/`

## Domain

**Tasks** — a simple to-do item: `Id`, `Title`, `Description`, `IsCompleted`, `CreatedAt`.

## What to build

1. `GET /tasks` — list all tasks (with optional `?completed=true/false` filter).
2. `POST /tasks` — create a task (validate: title required, max 200 chars).
3. `GET /tasks/{id}` — get one task (return 404 if not found).
4. `PUT /tasks/{id}` — update a task.
5. `DELETE /tasks/{id}` — delete a task.

## Acceptance criteria

- [ ] All endpoints return appropriate HTTP status codes.
- [ ] Input validation returns `ProblemDetails` with field-level errors.
- [ ] Endpoints are grouped under `app.MapGroup("/tasks")` in an `Endpoints/` file.
- [ ] Business logic lives in a `TaskService`, not in endpoint lambdas.
- [ ] At least one integration test using `WebApplicationFactory`.
- [ ] Follows `docs/conventions/dotnet-simple-minimal.md`.

## Template

Copy from `projects/templates/dotnet-minimal-api/`.

## Branch convention

`exercise/sp-02-<feature>`
