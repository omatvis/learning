# Exercises — Submission Rules

Each exercise submission lives in its own branch and is submitted as a PR.

## Folder structure

Submissions are organised by module under `exercises/submissions/<module>/`.  
Each submission is a folder named after the exercise, e.g.:

```
exercises/submissions/01-csharp-dotnet-basics/ex-01-types-nullability/
exercises/submissions/02-web-api-basics/ex-01-minimal-api/
```

## Submission workflow

1. Create a branch: `exercise/<module>-<exercise-number>` (e.g. `exercise/01-csharp-03`).
2. Add your code to the appropriate `exercises/submissions/<module>/` folder **and/or** the relevant `projects/` folder.
3. Open a PR and fill in `.github/pull_request_template.md`.
4. Add Copilot as a reviewer.
5. Apply feedback → push → merge when approved.

## Rules

- One PR per exercise (or per small logical piece of a larger exercise).
- Do not commit secrets, credentials, or large binary files.
- Tests are encouraged; see the exercise spec for requirements.
