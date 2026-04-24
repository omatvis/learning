# sp-04 — Full-Stack Mini

> **Goal:** Connect a React/TypeScript frontend to a .NET Minimal API backed by SQL Server.

## Project folder

`projects/small/sp-04-fullstack-mini/`

## What to build

Extend the Tasks domain from sp-02 with a React UI:

- Task list page: list tasks, filter by status, mark complete.
- Task form: create / edit a task.
- Delete task with confirmation.

## Acceptance criteria

### Backend

- [ ] Same sp-02 endpoints (extend if needed).
- [ ] CORS configured for the frontend dev server.

### Frontend

- [ ] TypeScript strict mode enabled.
- [ ] React Query used for data fetching.
- [ ] Loading and error states handled for every data-fetching component.
- [ ] No hard-coded API URL (use `import.meta.env.VITE_API_URL`).
- [ ] Follows `docs/conventions/react.md`.

### General

- [ ] `docker-compose.yml` (or README instructions) to run the full stack locally.

## Branch convention

`exercise/sp-04-<feature>`
