---
trigger: glob
description: Best practices for using shadcn-vue components
globs: ["**/components/ui/**/*.vue"]
---

# shadcn-vue Best Practices

- Import components explicitly and consistently (`import { Button } from '@/components/ui/button'`).
- Avoid modifying shadcn-vue internal component files directly.
- Customize components via wrapper components, props, or utility classes.
- Ensure consistent UI/UX patterns by strictly using shadcn-vue components across your app.
- Group Tailwind utility classes logically and consistently when customizing components.
- Document clearly any custom component wrappers or extensions created around shadcn-vue.
- Regularly update shadcn-vue components via official methods to benefit from improvements.
- Use accessibility attributes and roles consistently provided by shadcn-vue.
- Avoid mixing multiple UI libraries; keep the UI consistent using shadcn-vue exclusively.