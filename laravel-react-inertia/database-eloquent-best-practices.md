---
trigger: glob
description: Best practices for database schema, migrations, and Eloquent model usage in Laravel
globs: ["app/Models/*.php"]
---

# Database & Eloquent Best Practices

- Clearly define migrations with explicit names and comments.
- Keep migrations incremental; never edit past migrations after deployment.
- Always use Eloquent ORM for database interactions; avoid raw SQL unless necessary.
- Use Eloquent scopes extensively to encapsulate query logic.
- Eager-load relationships (`with()`) to prevent N+1 queries.
- Leverage Laravel factories and seeders consistently for testing/development.
- Clearly document relationships and database structure in models.
- Keep transactions atomic using Laravel’s DB transactions (`DB::transaction()`).
- Maintain clear and concise Eloquent model methods (`getActiveUsers()`, `isExpired()`).
- Regularly optimize database indices based on common query patterns.
- Enforce consistent primary and foreign key conventions across all tables.
- Clearly document complex queries or raw SQL logic when unavoidable.