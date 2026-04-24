# Conventions — .NET Minimal API (small projects)

> Rules for small projects that use Minimal APIs (`projects/templates/dotnet-minimal-api`).

## Project layout

```
App.Api/
├── Program.cs          # DI registration + app.Build() + MapGroup calls
├── Endpoints/          # One file per resource group (e.g. TaskEndpoints.cs)
├── Contracts/          # Request / response DTOs (records preferred)
├── Domain/             # Entities + domain rules (no framework references)
├── Data/               # DbContext or SQL access helpers / repositories
├── Services/           # Business logic orchestration
└── Common/             # Error types, helpers, mapping extensions
```

## Rules

- Use `app.MapGroup("/<resource>")` to group related endpoints.
- Return typed `Results<T1, T2>` for OpenAPI-friendly responses.
- Validate with `FluentValidation` filters or Data Annotations + `IEndpointFilter`.
- No business logic in `Program.cs` or endpoint lambdas — delegate to services.
- Use constructor injection; register services in `Program.cs`.
- Async all the way — no `.Result` / `.Wait()`.
- Parameterize all queries — no string-concatenated SQL.
- Return `ProblemDetails` for error responses.
