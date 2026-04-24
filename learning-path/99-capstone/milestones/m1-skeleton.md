# m1 — Skeleton

> Set up the repo structure, CI pipeline, and local development environment.

## Goals

- Create the solution and project structure in `projects/capstone/capstone-app/backend/`.
- Add Docker Compose for SQL Server.
- Verify the empty app builds and the CI workflow passes.

## Tasks

- [ ] Create `Capstone.sln` with four projects: Api, Application, Domain, Infrastructure.
- [ ] Set project references: Api → Application → Domain; Infrastructure → Application + Domain.
- [ ] Add `docker-compose.yml` with SQL Server service.
- [ ] Add a health-check endpoint (`GET /health`) that returns 200.
- [ ] CI passes (`dotnet build` + `dotnet test`).

## Acceptance criteria

- [ ] `dotnet build` succeeds with no warnings.
- [ ] `docker-compose up` starts SQL Server successfully.
- [ ] `GET /health` returns 200.
- [ ] Project references enforce the Clean Architecture dependency rules.
