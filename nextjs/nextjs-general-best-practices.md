---
trigger: always_on
description: General best practices for Next.js 15 projects
globs: ["**/*.tsx", "**/*.ts", "**/app/**"]
---

# Next.js 15 General Best Practices

- Strictly use App Router for all new Next.js 15 projects.
- Use server components (`.server.tsx`) by default; client components only if interactivity is needed (`"use client"`).
- Organize files clearly within `/app`, with dedicated folders for routes and nested layouts.
- Clearly separate layout (`layout.tsx`) and page components (`page.tsx`).
- Leverage route groups (`(auth)`, `(dashboard)`) for logically grouping related routes.
- Explicitly define metadata (`generateMetadata`) per page for better SEO.
- Always use Next.js Image (`next/image`) and Link (`next/link`) components instead of native elements.
- Keep dynamic routes (`[id]`) clean and well-documented.
- Consistently handle errors using Next.js error boundaries (`error.tsx`) within route segments.
- Utilize Next.js built-in middleware (`middleware.ts`) for authentication or redirects.
- Keep bundle optimized by minimizing unnecessary client-side code.
- Always prefer dynamic imports (`next/dynamic`) for heavy client-side libraries or components.
- Strictly enforce TypeScript usage across the entire codebase.
- Configure ESLint, Prettier, and TypeScript settings consistently for code quality.
- Run Next.js built-in optimizations regularly (`next build`, analyze bundle size).