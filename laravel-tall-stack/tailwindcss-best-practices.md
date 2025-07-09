---
trigger: glob
description: Tailwind CSS usage guidelines and UI best practices for Laravel, Vue, and React projects
globs: ["**/*.blade.php"]
---

# Tailwind CSS Best Practices

- Use utility-first classes consistently; avoid custom CSS unless absolutely necessary.
- Group utility classes logically and consistently for readability (position, spacing, typography).
- Extract repeating UI patterns into Blade components to avoid class repetition.
- Use Tailwind’s built-in responsive classes (`sm:`, `md:`, `lg:`) rather than media queries.
- Use `@apply` sparingly and only for repeated complex patterns.
- Avoid overriding Tailwind defaults directly; use `tailwind.config.js` instead.
- Keep the CSS bundle size optimized using Tailwind's PurgeCSS (Just-In-Time mode enabled).
- Always document customizations made in `tailwind.config.js`.
- Maintain consistency in spacing, typography, colors, and shadow scales.
- Leverage Tailwind’s built-in accessibility classes (`sr-only`, focus indicators, etc.).