---
trigger: glob
description: Best practices for database schema, migrations, and Eloquent model usage in Laravel
globs: ["**/*.php"]
---

# Database & Eloquent Best Practices

- Define migrations with clear and explicit naming conventions.
- Never alter past migrations once deployed; always create incremental migrations.
- Strictly prefer using Eloquent ORM over raw SQL queries.
- Utilize Eloquent scopes to encapsulate query logic clearly.
- Regularly use eager loading (`with()`) to avoid performance issues.
- Ensure transaction safety by using Laravel’s built-in transaction methods (`DB::transaction()`).
- Clearly define and document Eloquent model attributes, relationships, and casts.
- Keep complex query logic separated into clearly defined repository or query classes.
- Consistently use factories and seeders for populating databases during tests and development.
- Regularly review and optimize database indices based on actual query patterns.