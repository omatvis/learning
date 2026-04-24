# Projects

This directory contains all coding projects for the learning path.

## Structure

```
projects/
├── templates/          # starter layouts — copy when creating a new project
│   ├── dotnet-minimal-api/
│   ├── dotnet-controllers/
│   └── react-typescript/
├── small/              # small projects (sp-01 … sp-05)
│   ├── sp-01-csharp-katas/
│   ├── sp-02-crud-minimal/
│   ├── sp-03-crud-controllers/
│   ├── sp-04-fullstack-mini/
│   └── sp-05-auth-mini/
└── capstone/
    └── capstone-app/   # final project — Clean Architecture
```

## How to start a new small project

1. Copy the relevant template from `projects/templates/`.
2. Rename placeholders (`App` → your project name).
3. Follow the spec in `learning-path/05-small-projects/sp-XX-*.md`.
4. Submit work as PRs from `exercise/sp-XX-<feature>` branches.

## Conventions

- Small projects: `docs/conventions/dotnet-simple-minimal.md` or `docs/conventions/dotnet-simple-controllers.md`.
- Capstone: `docs/conventions/dotnet-clean-arch.md`.
- Frontend: `docs/conventions/react.md` + `docs/conventions/typescript.md`.
