---
trigger: glob
description: Tailwind CSS usage and styling best practices
globs: ["**/*.tsx", "**/*.module.css", "**/*.css"]
---

# Tailwind CSS Best Practices

- Strictly adhere to utility-first principles; avoid custom CSS unless essential.
- Group utility classes logically for readability and maintainability.
- Prefer responsive utility classes (`sm:`, `md:`, `lg:`) rather than manual media queries.
- Extract repetitive UI patterns into React components to reduce class repetition.
- Limit the usage of `@apply`; prefer direct usage of utility classes.
- Explicitly configure customizations in `tailwind.config.js`.
- Enable Tailwind JIT mode to optimize bundle size and performance.
- Use built-in accessibility utilities (`sr-only`, `focus-visible`) consistently.