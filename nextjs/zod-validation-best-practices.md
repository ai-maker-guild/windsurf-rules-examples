---
trigger: glob
description: Best practices for data validation using Zod
globs: ["**/schemas/*.ts", "**/*.schema.ts"]
---

# Zod Validation Best Practices

- Clearly define validation schemas separately within dedicated schema files.
- Strictly enforce schema naming conventions (`userSchema`, `loginFormSchema`).
- Utilize Zod's `.safeParse()` method for graceful error handling.
- Explicitly type schemas (`z.infer<typeof schema>`) for better TypeScript integration.
- Leverage `.refine()` for complex validation logic clearly and explicitly.
- Consistently use schemas both for client-side validation and server-side type safety.
- Always centralize schemas to avoid duplication; reuse across frontend and backend code.
- Clearly structure error messages returned from Zod validation for easy UI display.
- Regularly unit-test validation schemas to ensure data integrity.