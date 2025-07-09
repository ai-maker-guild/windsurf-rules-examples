---
trigger: glob
description: Tailwind CSS usage guidelines and UI best practices for Laravel, Vue, and React projects
globs: ["**/*.tsx"]
---

# Tailwind CSS Best Practices

- Stick strictly to utility-first Tailwind CSS principles; minimize custom CSS.
- Consistently group utility classes logically (display, position, spacing, typography).
- Use responsive classes (`sm:`, `md:`, `lg:`) rather than manual media queries.
- Extract repeating UI patterns into reusable React components instead of repeating class sets.
- Utilize Tailwind’s built-in theme system; avoid arbitrary values.
- Minimize `@apply` usage; prefer direct utility classes unless complex repetition is frequent.
- Configure theme customizations explicitly in `tailwind.config.js`.
- Enable JIT compilation mode and purging for optimal performance and bundle size.
- Regularly audit CSS bundle size; keep Tailwind configuration lean and documented.
- Utilize Tailwind’s built-in accessibility helpers (`focus-visible`, `sr-only`).