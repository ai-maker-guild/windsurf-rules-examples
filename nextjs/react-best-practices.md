---
trigger: always_on
description: React component and hook best practices for Next.js
globs: ["**/*.tsx", "**/*.ts"]
---

# React Best Practices for Next.js

- Use React functional components exclusively with hooks (`useState`, `useEffect`, `useMemo`, `useCallback`).
- Clearly separate logic from presentation; avoid mixing UI with complex logic.
- Extract reusable logic into custom hooks (`useAuth`, `useFetchUser`).
- Always name components clearly using PascalCase (`UserProfileCard`, `DashboardLayout`).
- Utilize error boundaries at critical UI points.
- Keep state management simple; use Zustand for global state if needed, avoid unnecessary Redux usage.
- Minimize prop drilling; leverage React Context cautiously and explicitly.
- Always use React Server Components (RSC) unless interactivity explicitly requires a client component.
- Optimize re-renders using `React.memo`, `useMemo`, `useCallback` when justified.
- Maintain clear component hierarchy to improve readability and maintainability.