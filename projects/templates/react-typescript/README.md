# Template — React + TypeScript

> Copy this template when starting a new React frontend project.

## How to use

1. Copy this directory to `projects/small/sp-XX-<name>/frontend/` or `projects/capstone/capstone-app/frontend/`.
2. Scaffold with Vite: `npm create vite@latest . -- --template react-ts`.
3. Follow `docs/conventions/react.md` and `docs/conventions/typescript.md`.

## Directory layout (after scaffolding)

```
frontend/
├── src/
│   ├── api/           # API client functions / React Query hooks
│   ├── components/    # shared / reusable components
│   ├── features/      # feature folders (each feature has its own components + hooks)
│   ├── pages/         # top-level route components
│   ├── types/         # shared TypeScript types
│   └── main.tsx
└── tests/             # Vitest / Testing Library tests
```

## TODO

- [ ] Run `npm create vite@latest . -- --template react-ts`.
- [ ] Enable `strict: true` in `tsconfig.json`.
- [ ] Add React Query: `npm install @tanstack/react-query`.
- [ ] Configure `VITE_API_URL` environment variable.
- [ ] Implement features per the project spec.
