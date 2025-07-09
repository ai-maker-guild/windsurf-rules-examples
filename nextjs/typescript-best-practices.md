---
trigger: glob
description: TypeScript usage and configuration best practices
globs: ["**/*.ts", "**/*.tsx"]
---

# TypeScript Best Practices

- Always enforce strict TypeScript configurations (`strict: true`, `noImplicitAny: true`).
- Use explicit typing rather than implicit inference in complex components and functions.
- Centralize type definitions and interfaces clearly (`types/` folder).
- Prefer utility types (`Pick`, `Omit`, `Partial`) over duplicating interfaces.
- Regularly run type-checking (`tsc --noEmit`) during development and CI.
- Strictly type props and state in React components explicitly.
- Avoid usage of `any`; if unavoidable, explicitly document reasoning.
- Ensure all external APIs and data sources have explicitly defined types.