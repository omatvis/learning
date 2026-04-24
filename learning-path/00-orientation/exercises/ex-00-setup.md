# ex-00 — Environment Setup

> **Goal:** Verify your development environment is ready for all subsequent exercises.

## Tasks

1. Confirm .NET 10 SDK is installed: `dotnet --version` (should show `10.x.x`).
2. Confirm Node.js LTS is installed: `node --version`.
3. Confirm Git is installed: `git --version`.
4. Clone this repo (if not already done) and create a test branch: `exercise/00-setup`.
5. Create a tiny "Hello, World" console app:
   ```bash
   mkdir -p exercises/submissions/00-orientation/ex-00-setup
   cd exercises/submissions/00-orientation/ex-00-setup
   dotnet new console -n HelloWorld
   cd HelloWorld && dotnet run
   ```
6. Open a PR from `exercise/00-setup` and verify the CI workflow passes.

## Acceptance criteria

- [ ] `dotnet run` prints "Hello, World!".
- [ ] CI workflow passes on the PR.
- [ ] PR description is filled in using the template.

## Branch

`exercise/00-setup`
