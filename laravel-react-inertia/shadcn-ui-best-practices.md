---
trigger: glob
description: Best practices for using shadcn/ui components
globs: ["**/components/ui/**/*.tsx"]
---

# Shadcn/ui Best Practices

- Always import Shadcn components explicitly (`import { Button } from '@/components/ui/button'`).
- Avoid direct modification of component files; use wrapper components or utility classes for customization.
- Extend Shadcn components via props and classNames rather than direct internal modifications.
- Clearly document custom wrapper components built around Shadcn.
- Use Shadcn components consistently for UI elements; avoid mixing with other UI libraries.
- Apply consistent spacing (`p-`, `m-`), rounding, and shadows as recommended by Shadcn/ui guidelines.
- Always leverage Shadcn’s built-in accessibility attributes (ARIA, roles).
- Avoid overriding styles with arbitrary CSS; use Tailwind classes first.
- Organize custom UI extensions clearly in `components/ui/custom` if necessary.
- Regularly update Shadcn components via CLI to incorporate latest best practices.