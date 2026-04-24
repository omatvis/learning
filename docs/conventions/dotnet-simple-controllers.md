# Conventions — .NET Controllers (small projects)

> Rules for small projects that use MVC Controllers (`projects/templates/dotnet-controllers`).

## Project layout

```
App.Api/
├── Program.cs          # DI registration + app.Build()
├── Controllers/        # One controller per resource (e.g. TasksController.cs)
├── Contracts/          # Request / response DTOs (records preferred)
├── Domain/             # Entities + domain rules (no framework references)
├── Data/               # DbContext or SQL access helpers / repositories
├── Services/           # Business logic orchestration
└── Common/             # Error types, helpers, mapping extensions
```

## Rules

- Decorate controllers with `[ApiController]` — enables automatic model-state validation.
- Keep controllers thin: one action per HTTP verb, delegate all logic to services.
- Return `ActionResult<T>` or `IActionResult`; avoid returning `object`.
- Use constructor injection; register services in `Program.cs`.
- Async all the way — no `.Result` / `.Wait()`.
- Parameterize all queries — no string-concatenated SQL.
- Return `ProblemDetails` for error responses (use `Problem()` helper).
- Validate inputs via Data Annotations or `FluentValidation` with `AddFluentValidationAutoValidation()`.
