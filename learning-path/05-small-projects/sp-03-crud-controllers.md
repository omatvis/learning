# sp-03 — CRUD API (Controllers)

> **Goal:** Rebuild the same Tasks domain using MVC Controllers to compare the two styles.

## Project folder

`projects/small/sp-03-crud-controllers/`

## Domain

Same as sp-02: **Tasks** (`Id`, `Title`, `Description`, `IsCompleted`, `CreatedAt`).

## What to build

Same endpoints as sp-02, implemented with a `TasksController`.

## Acceptance criteria

- [ ] `[ApiController]` attribute is applied; model-state validation is automatic.
- [ ] Controller is thin — all logic is in `TaskService`.
- [ ] Returns `ActionResult<T>` (not `object`).
- [ ] Returns `Problem(...)` for errors; 404 for not-found.
- [ ] At least one integration test using `WebApplicationFactory`.
- [ ] Follows `docs/conventions/dotnet-simple-controllers.md`.

## Template

Copy from `projects/templates/dotnet-controllers/`.

## Reflection exercise

After completing sp-02 and sp-03, write a short note in each project's `README.md`:
- What was easier/harder with Minimal APIs vs Controllers?
- When would you choose each?

## Branch convention

`exercise/sp-03-<feature>`
