# Capstone App

> Full-stack application built using Clean Architecture (.NET 10 + SQL Server + React/TypeScript).

## Architecture

```
capstone-app/
├── backend/
│   ├── Capstone.sln
│   ├── src/
│   │   ├── Capstone.Api/            # HTTP layer (thin controllers or endpoints)
│   │   ├── Capstone.Application/   # CQRS use-cases, interfaces
│   │   ├── Capstone.Domain/        # Entities, value objects (no framework deps)
│   │   └── Capstone.Infrastructure/ # EF Core, SQL, external services
│   └── tests/
│       ├── Capstone.UnitTests/
│       └── Capstone.IntegrationTests/
├── frontend/                        # React + TypeScript (Vite)
├── database/
│   ├── schema/
│   ├── migrations/
│   └── seed/
└── ops/
    ├── docker/
    └── scripts/
```

## Milestones

See `learning-path/99-capstone/milestones/` for detailed specs.

## How to run

```bash
# TODO: fill in once milestone m1 is complete
docker-compose -f ops/docker/docker-compose.yml up
```

## Conventions

- Backend: `docs/conventions/dotnet-clean-arch.md`
- Frontend: `docs/conventions/react.md`, `docs/conventions/typescript.md`
- Database: `docs/conventions/sql-server.md`
