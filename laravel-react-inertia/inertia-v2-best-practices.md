---
trigger: glob
description: Best practices for using Inertia.js v2 with Laravel, Vue, or React
globs: [ "**/*.tsx"]
---

# Inertia v2 Best Practices

- Always structure pages and layouts clearly in separate folders (`Pages/`, `Layouts/`).
- Pass minimal data via Inertia props; fetch extra data asynchronously when necessary.
- Use Inertia’s built-in methods (`useForm()`, `router`) consistently for forms and navigation.
- Utilize persistent layouts (`<Layout>` components) for consistent UI across pages.
- Always handle loading states gracefully with Inertia's built-in indicators.
- Prefer Inertia links (`<Link>`) over regular anchor tags for SPA navigation.
- Leverage Inertia middleware for shared props (user, permissions, flash messages).
- Always define explicit error handling in frontend components.
- Optimize payload sizes sent from Laravel controllers; use pagination or lazy loading when possible.
- Leverage Inertia’s partial reloads (`only`) for targeted updates.