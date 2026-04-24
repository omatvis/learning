# Template — .NET Minimal API

> Copy this template when starting a new Minimal API small project.

## How to use

1. Copy this directory to `projects/small/sp-XX-<name>/`.
2. Rename `App` to your project name throughout (solution, project files, namespaces).
3. Follow `docs/conventions/dotnet-simple-minimal.md`.

## Directory layout

```
backend/
├── App.sln
├── src/
│   └── App.Api/
│       ├── Program.cs
│       ├── Endpoints/       # route groups — one file per resource
│       ├── Contracts/       # request / response DTOs (records)
│       ├── Domain/          # entities + domain rules (no framework refs)
│       ├── Data/            # DbContext or SQL access / repositories
│       ├── Services/        # business logic
│       └── Common/          # error types, helpers, mapping
└── tests/
    ├── App.UnitTests/
    └── App.IntegrationTests/
```

## TODO

- [ ] Rename `App` to your project name.
- [ ] Add NuGet packages (`dotnet add package ...`).
- [ ] Implement `Program.cs` (DI + routing).
- [ ] Implement endpoints, services, and data access.
- [ ] Add tests.
