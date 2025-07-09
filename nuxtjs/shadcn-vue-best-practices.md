---
trigger: glob
description: Best practices for using shadcn-vue components
globs: ["**/components/ui/**/*.vue"]
---

# Shadcn-vue Best Practices

- Import components explicitly (`import { Button } from '@/components/ui/button'`).
- Avoid directly modifying internal Shadcn-vue component files.
- Customize components explicitly through props or utility classes.
- Extract reusable UI patterns into wrapper components clearly.
- Maintain consistent UI design (spacing, shadows, rounding).
- Regularly update Shadcn-vue components for the latest improvements.
- Use built-in accessibility features (`aria-`, roles) consistently.
- Document custom wrappers or extensions built around Shadcn-vue explicitly.