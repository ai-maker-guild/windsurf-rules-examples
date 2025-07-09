---
trigger: glob
description: Best practices for Vue 3 with Laravel & Inertia V2
globs: ["**/*.vue", "**/composables/*.ts"]
---

# Vue.js Best Practices (with Inertia)

- Use Composition API consistently with `<script setup>`.
- Structure Vue components clearly by responsibility (Atomic design: Atoms, Molecules, Organisms).
- Clearly name components in PascalCase (`UserCard.vue`, `OrderTable.vue`).
- Avoid deep nesting of components; prefer shallow and modular composition.
- Always use reactive state (`ref()`, `reactive()`) clearly and explicitly.
- Extract reusable logic into composables (`useAuth()`, `useOrders()`, `usePagination()`).
- Handle side effects clearly with `watch()` and `onMounted()` lifecycle hooks.
- Always use key attributes (`:key`) in `v-for` loops.
- Keep templates clear and concise; delegate complex logic to computed properties or composables.
- Optimize performance using Vue’s built-in optimization tools (computed caching, `v-memo` directive).
- Clearly handle and document emitted events (`defineEmits`).
- Strictly enforce ESLint and Prettier configuration for consistency.
- Use TypeScript consistently to enhance maintainability and readability.