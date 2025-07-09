---
trigger: always_on
description: General best practices for Nuxt.js 3 projects
globs: ["**/*.vue", "**/*.ts", "**/app.vue", "**/pages/**"]
---

# Nuxt.js 3 General Best Practices

- Always use Nuxt’s file-based routing strictly within the `pages/` directory.
- Clearly separate components (`components/`), layouts (`layouts/`), and composables (`composables/`).
- Use Nuxt layouts (`<NuxtLayout>`) consistently to maintain uniformity across pages.
- Leverage Nuxt middleware explicitly for authentication and redirections (`defineNuxtRouteMiddleware`).
- Use `<NuxtLink>` instead of native anchor tags for internal navigation.
- Strictly adhere to Nuxt’s server-side rendering patterns (SSG/SSR/ISG).
- Optimize page metadata (`useSeoMeta`, `definePageMeta`) explicitly for better SEO and social sharing.
- Use `useAsyncData` for server-side fetching and hydration clearly and consistently.
- Enable auto-imports (`composables`, `utils`) only when project size justifies it; otherwise, prefer explicit imports for clarity.
- Configure ESLint, Prettier, and TypeScript consistently.
- Regularly optimize and audit the Nuxt bundle (`nuxi build`).
- Keep components small, reusable, and strictly single-purpose.
- Clearly document usage of plugins and modules (`modules/`, `plugins/`) in Nuxt config.