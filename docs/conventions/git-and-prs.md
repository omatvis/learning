# Conventions — Git and PRs

## Branch naming

| Pattern | Use |
|---------|-----|
| `exercise/<module>-<n>` | Exercise submission (e.g. `exercise/01-csharp-03`) |
| `feature/<topic>` | New feature in a project |
| `fix/<topic>` | Bug fix |
| `chore/<topic>` | Tooling, config, documentation |

## Commit messages

Use the imperative mood: `Add`, `Fix`, `Update`, `Remove`.  
Keep the subject line ≤ 72 characters.  
Reference an issue or exercise number when relevant: `Add CRUD endpoints (exercise/02-01)`.

## PR rules

- One logical change per PR; keep diffs small and focused.
- Fill in every section of `.github/pull_request_template.md`.
- Add Copilot as a reviewer on every exercise PR.
- Do not merge until all coaching comments are addressed (or explicitly deferred).
- Squash or rebase before merging to keep `main` history clean.

## Review etiquette

- Respond to every review comment — even if just "done" or "acknowledged".
- If you disagree with a suggestion, say why — it is a learning opportunity.
