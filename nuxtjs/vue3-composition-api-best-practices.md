---
trigger: glob
description: Best practices for Vue 3 Composition API in Nuxt.js
globs: ["**/*.vue", "**/composables/*.ts"]
---

# Vue 3 Composition API Best Practices

- Use `<script setup>` exclusively for concise syntax and automatic imports.
- Clearly separate UI presentation from business logic within composables (`useAuth`, `useProducts`).
- Always use reactive state (`ref`, `reactive`) explicitly for clarity.
- Avoid deep nesting of components; prefer modular composition.
- Extract reusable logic into composables; avoid complex logic inside components.
- Always explicitly declare emitted events (`defineEmits`) and props (`defineProps`) clearly.
- Handle side effects clearly with lifecycle hooks (`onMounted`, `watch`, `watchEffect`).
- Consistently optimize performance with computed properties and cached reactive data.
- Always use TypeScript explicitly in components and composables.
- Maintain consistent component naming conventions using PascalCase (`UserCard`, `OrderForm`).