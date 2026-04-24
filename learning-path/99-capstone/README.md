# 99 — Capstone

> **Goal:** Build a production-quality full-stack application from scratch using Clean Architecture.

## What to build

A **task-management / productivity app** (or a topic of your choice — discuss with Copilot).  
The exact domain will be refined in milestone m2; what matters is completing all six milestones.

## Architecture

- Backend: .NET 8, Clean Architecture (Api / Application / Domain / Infrastructure).
- Database: SQL Server with EF Core migrations.
- Frontend: React + TypeScript (Vite).
- Auth: JWT.
- Ops: Docker Compose for local development.

## Milestones

| # | Name | Spec |
|---|------|------|
| m1 | Skeleton | [milestones/m1-skeleton.md](milestones/m1-skeleton.md) |
| m2 | Domain model | [milestones/m2-domain.md](milestones/m2-domain.md) |
| m3 | Data access | [milestones/m3-data-access.md](milestones/m3-data-access.md) |
| m4 | API layer | [milestones/m4-api.md](milestones/m4-api.md) |
| m5 | React frontend | [milestones/m5-frontend.md](milestones/m5-frontend.md) |
| m6 | Hardening | [milestones/m6-hardening.md](milestones/m6-hardening.md) |

## Conventions

Follow `docs/conventions/dotnet-clean-arch.md`, `docs/conventions/react.md`, `docs/conventions/sql-server.md`.
