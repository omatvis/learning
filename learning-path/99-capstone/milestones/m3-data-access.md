# m3 — Data Access

> Implement the Infrastructure layer: EF Core, repositories, and database migrations.

## Goals

- Implement `IRepository<T>` using EF Core in `Capstone.Infrastructure`.
- Create and apply the first migration.
- Seed development data.

## Tasks

- [ ] Add EF Core DbContext in `Infrastructure`.
- [ ] Implement repository interfaces defined in `Domain`.
- [ ] Create and apply initial migration (`dotnet ef migrations add Initial`).
- [ ] Add seed data script in `database/seed/`.
- [ ] Write integration tests using a real (or containerized) SQL Server database.

## Acceptance criteria

- [ ] `dotnet ef database update` applies migrations cleanly.
- [ ] Repository integration tests pass against a real database.
- [ ] No raw string-concatenated SQL anywhere.
