---
trigger: glob
description: Best practices for data validation using Zod in Nuxt.js
globs: ["**/schemas/*.ts", "**/*.schema.ts"]
---

# Zod Validation Best Practices

- Centralize validation schemas clearly within dedicated files (`schemas/`).
- Explicitly infer types from schemas (`z.infer<typeof schema>`) for strong TypeScript integration.
- Utilize Zod’s `.safeParse()` consistently for robust error handling.
- Clearly use `.refine()` for complex validations; document intent clearly.
- Reuse schemas consistently for client-side and server-side validations.
- Structure validation error responses explicitly for clear UI handling.
- Regularly unit-test schemas to ensure data integrity and consistency.