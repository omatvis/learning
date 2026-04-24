# sp-05 — Auth Mini

> **Goal:** Add JWT authentication to a Controllers-based API and protect React routes.

## Project folder

`projects/small/sp-05-auth-mini/`

## What to build

Extend the Tasks domain from sp-03 with authentication:

### Backend

- `POST /auth/register` — create a user account.
- `POST /auth/login` — return a JWT access token.
- Protect `POST`, `PUT`, `DELETE /tasks` with `[Authorize]`.
- `GET /tasks` remains public.

### Frontend

- Login and register pages.
- Store JWT in memory (not localStorage); refresh on page load via a `/auth/me` endpoint or similar.
- Redirect unauthenticated users to the login page.

## Acceptance criteria

- [ ] Passwords are hashed (use ASP.NET Core `IPasswordHasher<T>` or BCrypt).
- [ ] JWT secret loaded from configuration (not hard-coded).
- [ ] Protected endpoints return `401` when token is missing or invalid.
- [ ] Frontend handles token expiry gracefully.
- [ ] Follows `docs/conventions/dotnet-simple-controllers.md`.

## Branch convention

`exercise/sp-05-<feature>`
