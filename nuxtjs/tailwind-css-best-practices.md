---
trigger: glob
description: Tailwind CSS styling best practices for Nuxt.js
globs: ["**/*.vue", "**/*.css", "**/*.module.css"]
---

# Tailwind CSS Best Practices

- Strictly adhere to Tailwind’s utility-first approach; minimize custom CSS.
- Clearly group utility classes logically and consistently.
- Prefer responsive utilities (`sm:`, `md:`, `lg:`) explicitly over custom media queries.
- Limit the use of `@apply`; prefer direct utility classes for clarity.
- Configure customizations explicitly in `tailwind.config.js`.
- Enable Tailwind’s JIT mode to optimize CSS bundle size and performance.
- Utilize built-in accessibility utilities (`sr-only`, `focus-visible`) consistently.
- Document clearly any customizations or extensions made to Tailwind configuration.