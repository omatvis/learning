# m6 — Hardening

> Improve reliability, observability, security, and test coverage.

## Goals

- Increase test coverage.
- Add structured logging and basic observability.
- Address security concerns.
- Prepare for a "production-like" deployment.

## Tasks

- [ ] Achieve ≥ 80% unit test coverage in `Application` and `Domain`.
- [ ] Add structured logging with Serilog (or `Microsoft.Extensions.Logging`).
- [ ] Add a global exception handler middleware.
- [ ] Validate all configuration values at startup (fail fast).
- [ ] Rate-limit sensitive endpoints (auth, registration).
- [ ] Review and document any known security trade-offs.
- [ ] Add a `CHANGELOG.md` and tag `v1.0.0`.

## Acceptance criteria

- [ ] CI passes with all tests green.
- [ ] No secrets committed.
- [ ] Security review checklist in `README.md` is filled in.
- [ ] `v1.0.0` tag is pushed.
