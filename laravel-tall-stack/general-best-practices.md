---
trigger: glob
description: General best practices for Laravel projects using the TALL stack (Tailwind, Alpine.js, Laravel, Livewire)
globs: ["**/*.php", "**/*.blade.php"]
---

# General Best Practices (Laravel TALL Stack)

- Use Laravel conventions strictly for file structure.
- Maintain Laravel's default naming conventions for controllers, models, views, and components.
- Always use route names instead of hard-coded URLs.
- Follow PSR-12 coding standards consistently.
- Prefer Laravel Blade components over partial views for reusable UI.
- Keep controllers thin: delegate complex logic to service classes or action classes.
- Adhere to Laravel’s MVC pattern; avoid heavy logic in Blade views.
- Utilize Laravel’s built-in authentication scaffolding when applicable.
- Explicitly declare fillable attributes in all Eloquent models.
- Use Laravel policies for authorization logic.
- Enforce validation using Laravel Form Requests rather than inline validation.
- Always define relationships clearly and explicitly in Eloquent models.
- Use Laravel Mix or Vite for asset compilation.
- Configure and use Laravel’s logging channels appropriately (avoid direct use of PHP `error_log()`).
- Store sensitive configuration securely in `.env`, never in source code.
- Keep Laravel version up-to-date; leverage Laravel Shift if needed.