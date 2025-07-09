---
trigger: glob
description: Best practices for database schema, migrations, and Eloquent model usage in Laravel
globs: ["app/Models/*.php"]
---

# Database & Eloquent Best Practices

- Define migrations clearly and use descriptive naming conventions.
- Maintain separate migration files per table change for clear rollback capabilities.
- Use Eloquent scopes to encapsulate common query logic.
- Eager-load relationships to prevent N+1 issues (`with()`, `load()`).
- Avoid direct queries (`DB::table()`); prefer using Eloquent ORM.
- Use database seeders and factories consistently for testing/development.
- Keep database transactions atomic using Laravel’s DB transaction helpers.
- Avoid logic-heavy queries; delegate complex logic to services or repositories.
- Clearly document database schema changes using comments or markdown files.
- Regularly run Laravel’s optimization commands (`artisan optimize`, `artisan migrate:fresh --seed` for local development).