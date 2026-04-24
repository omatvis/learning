# Conventions — TypeScript

> TypeScript rules for all projects in this repo.

## Rules

- Enable `strict: true` in `tsconfig.json` — no exceptions.
- Avoid `any`; use `unknown` + type guards where the shape is truly unknown.
- Prefer `interface` for object shapes that may be extended; `type` for unions and aliases.
- Use **readonly** for data that should not be mutated.
- Export types and interfaces from a barrel file (`types/index.ts`) per feature.
- Use **generics** instead of duplicating typed logic.
- Prefer **discriminated unions** over optional properties for variant types.
- Use utility types (`Partial`, `Required`, `Pick`, `Omit`, `ReturnType`, etc.) to avoid repetition.
- Never assert `as X` without a comment explaining why the assertion is safe.
- Co-locate types with the code that uses them; only move to `types/` when shared across features.
