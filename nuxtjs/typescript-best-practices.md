---
trigger: glob
description: TypeScript best practices for Nuxt.js projects
globs: ["**/*.vue", "**/*.ts"]
---

# TypeScript Best Practices

- Strictly configure TypeScript (`strict: true`, `noImplicitAny: true`) consistently.
- Explicitly type component props, state, and emitted events (`defineProps`, `defineEmits`).
- Clearly define types and interfaces within a centralized folder (`types/`).
- Prefer utility types (`Pick`, `Omit`, `Partial`) explicitly over duplicating interfaces.
- Regularly perform type checks (`vue-tsc --noEmit`) during development and CI.
- Avoid `any` usage; document clearly if unavoidable.
- Ensure external APIs and data sources have explicitly defined types.