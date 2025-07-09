---
trigger: glob
description: General best practices for Laravel projects using the TALL stack (Tailwind, Alpine.js, Laravel, Livewire)
globs: ["**/*.php", "**/*.blade.php"]
---

# Laravel 12 General Best Practices

- Follow Laravel 12’s default directory structure strictly.‡
- Always define named routes; never hard-code URLs.
- Keep controllers lean; delegate heavy logic to dedicated services or actions.
- Utilize Laravel Form Requests for validating inputs.
- Clearly define Eloquent relationships explicitly in models.
- Implement Laravel policies and gates for authorization consistently.
- Store sensitive environment data securely within `.env`.
- Always adhere to Laravel’s middleware conventions.
- Optimize database queries using eager-loading (`with()`) to avoid N+1 issues.
- Manage scheduled tasks explicitly in Laravel’s `Console/Kernel.php`.
- Use Laravel’s built-in authentication scaffolding when appropriate.
- Utilize queues (Redis, Database driver) for long-running or background jobs.
- Prefer Laravel’s built-in storage drivers for handling file uploads (S3, R2).
- Stick to PSR-12 coding standards consistently.