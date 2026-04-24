# Conventions — SQL Server

> Rules for SQL Server usage in all projects.

## Rules

- **Always parameterize** queries — never concatenate user input into SQL strings.
- Use **stored procedures** only for complex, performance-critical queries; prefer ORM or parameterised SQL otherwise.
- Name tables in **PascalCase singular** (e.g. `Task`, `User`).
- Name columns in **PascalCase** (e.g. `CreatedAt`, `IsDeleted`).
- Every table must have a surrogate primary key (`Id INT IDENTITY` or `Id UNIQUEIDENTIFIER`).
- Use **soft deletes** (`IsDeleted BIT`) where audit trails matter; use hard deletes otherwise.
- Add a `CreatedAt DATETIME2` column to every table.
- Keep transactions **intentional and short**; avoid long-running transactions.
- Consider indexes on foreign keys and frequently filtered columns.
- Avoid `N+1` patterns — use JOINs or batch queries.
- Store schema scripts in `database/schema/` and seed data in `database/seed/`.
- EF Core migrations (if used) live in `database/migrations/`.
