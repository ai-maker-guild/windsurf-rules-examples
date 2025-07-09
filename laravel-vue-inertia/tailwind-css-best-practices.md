---
trigger: glob
description: Tailwind CSS usage guidelines and UI best practices for Laravel, Vue, and React projects
globs: ["**/*.vue"]
---

# Tailwind CSS Best Practices

- Strictly follow utility-first principles; minimize custom CSS.
- Group classes logically (layout, spacing, typography) for readability.
- Consistently use responsive classes (`sm:`, `md:`, `lg:`) provided by Tailwind.
- Extract recurring UI elements into reusable Vue components rather than repeating class sets.
- Limit the usage of `@apply`; prefer direct use of utility classes for clarity.
- Configure theme adjustments explicitly in `tailwind.config.js`; avoid inline arbitrary values.
- Enable JIT mode and use purging to keep the bundle optimized.
- Use Tailwind’s built-in accessibility utilities (`focus-visible`, `sr-only`) regularly.
- Document clearly any Tailwind config customizations for easy maintenance.
- Audit and optimize CSS bundle size regularly.