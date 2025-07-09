---
trigger: glob
description: General best practices for Laravel projects using the TALL stack (Tailwind, Alpine.js, Laravel, Livewire)
globs: ["**/*.php", "**/*.blade.php"]
---

# Laravel 12 General Best Practices

- Always adhere strictly to Laravel 12 conventions and file structure.
- Prefer route names over hard-coded URLs.
- Keep controllers lean; delegate logic to action classes or service layers.
- Enforce validation using dedicated Form Requests.
- Always define Eloquent relationships explicitly in models.
- Use Laravel’s built-in authentication scaffolding when possible.
- Maintain Laravel’s default middleware structure for consistency.
- Clearly separate business logic from controllers; avoid inline logic.
- Leverage Laravel policies and gates for authorization.
- Keep sensitive information strictly within `.env` files.
- Store assets using Laravel’s storage filesystem (S3, Cloudflare R2).
- Utilize Laravel Mix or Vite for asset bundling consistently.
- Implement queues for time-consuming tasks (using Redis or database driver).
- Always define scheduled tasks explicitly in Laravel’s `Kernel.php`.
- Strictly follow PSR-12 coding standards.