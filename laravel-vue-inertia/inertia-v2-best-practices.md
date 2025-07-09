---
trigger: glob
description: Best practices for using Inertia.js v2 with Laravel, Vue, or React
globs: ["**/*.vue", "**/*.php"]
---

# Inertia v2 Best Practices

- Clearly organize Inertia pages and layouts (`Pages/`, `Layouts/`).
- Minimize props passed from Laravel to frontend; fetch extra data asynchronously if needed.
- Use Inertia’s form helpers (`useForm()`) consistently for handling forms.
- Leverage persistent layouts via `<slot />` and layout components to avoid repetition.
- Use Inertia links (`<Link>`) exclusively for internal navigation.
- Define shared data (user details, flash messages) via Laravel middleware.
- Utilize partial reloads (`only`) to optimize component rendering.
- Implement graceful loading states and error handling consistently.
- Always ensure validation errors are clearly displayed to the user.
- Keep controller responses concise; offload complex state management to the frontend.