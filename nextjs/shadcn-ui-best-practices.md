---
trigger: glob
description: Best practices for using shadcn/ui components
globs: ["**/components/ui/**/*.tsx"]
---

# shadcn/ui Best Practices

- Always import components explicitly (`import { Button } from "@/components/ui/button"`).
- Avoid direct modifications of shadcn/ui component internals.
- Customize components via props and Tailwind utility classes rather than arbitrary CSS.
- Extract reusable UI patterns into clear wrapper components when necessary.
- Maintain consistency in styling across the app (spacing, rounding, shadows).
- Regularly update shadcn/ui components to leverage latest improvements.
- Clearly document customizations and extensions built around shadcn/ui.
- Consistently use built-in accessibility features provided by shadcn/ui components.