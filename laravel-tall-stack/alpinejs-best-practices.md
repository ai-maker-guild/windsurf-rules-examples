---
trigger: glob
description: Best practices for Alpine.js usage in Laravel Blade templates
globs: ["**/*.blade.php"]
---

# Alpine.js Best Practices

- Use Alpine.js strictly for simple client-side interactivity; delegate complex logic to Livewire.
- Always scope Alpine components explicitly with `x-data`.
- Limit nested Alpine.js directives for readability and maintainability.
- Use `x-show` with transitions for UI animations instead of CSS-only solutions.
- Avoid inline JavaScript logic inside Blade; prefer Alpine directives.
- Keep state management simple; if complexity increases, delegate to Livewire.
- Use event-driven architecture (`@click`, `@input`) clearly and consistently.
- Always initialize default Alpine state to avoid undefined behaviors.
- Keep DOM manipulations minimal and performant.
- Avoid excessive polling or intervals; use event-driven or reactive patterns instead.