---
trigger: glob
description: Best practices for building React components and hooks in modern web applications
globs: ["**/*.tsx"]
---

# React Best Practices (with Inertia)

- Use functional components exclusively with Hooks (`useState`, `useEffect`, `useMemo`).
- Structure React components clearly into atomic, reusable units.
- Follow clear naming conventions (`UserProfileCard`, `OrderListItem`).
- Separate business logic into custom hooks (`useOrders`, `useAuth`, `useForm`).
- Minimize prop drilling; utilize context or state management libraries (Zustand, Redux Toolkit) only if complexity justifies.
- Clearly handle side-effects in `useEffect()` hooks; clean up properly.
- Optimize React rendering using `React.memo()`, `useCallback()`, and `useMemo()` when justified.
- Avoid excessive use of inline callbacks; prefer named handlers.
- Maintain consistent folder structure (`Components/`, `Hooks/`, `Utils/`, `Pages/`).
- Ensure error boundaries are defined for better UI reliability.
- Always use TypeScript for better reliability and maintainability.
- Clearly separate presentational components from logic-based components.
- Maintain consistent code style with ESLint and Prettier configured.