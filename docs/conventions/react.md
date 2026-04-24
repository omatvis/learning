# Conventions — React

> Rules for React projects in this repo (small projects + capstone frontend).

## Rules

- Use **functional components** only — no class components.
- Prefer **TypeScript**; see `typescript.md` for typing rules.
- Co-locate component, styles, and tests: `MyComponent/MyComponent.tsx`, `MyComponent.test.tsx`.
- Use **React Query** (or SWR) for server state; avoid `useEffect` + `useState` for data fetching.
- **Accessibility**: use semantic HTML elements; add ARIA labels where needed.
- Handle **loading** and **error** states explicitly in every data-fetching component.
- Avoid unnecessary re-renders; use `useMemo`/`useCallback` only with profiler evidence.
- Keep components small and focused (single responsibility).
- Avoid prop-drilling more than two levels — lift state or use Context / a state library.
- Do not hard-code API base URLs — use environment variables (`import.meta.env.VITE_API_URL`).
