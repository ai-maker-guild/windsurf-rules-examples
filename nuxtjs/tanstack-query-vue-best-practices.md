---
trigger: glob
description: Best practices for data fetching with Tanstack Query (Vue Query)
globs: ["**/*.vue", "**/composables/use*.ts"]
---

# Tanstack Query (Vue Query) Best Practices

- Clearly define custom composables (`useUsersQuery`, `useCreateOrderMutation`) for queries and mutations.
- Explicitly structure query keys (`['users', userId]`, `['orders']`) consistently.
- Leverage caching and stale data settings explicitly (`staleTime`, `cacheTime`).
- Always handle query states (`isLoading`, `isError`, `data`) explicitly and clearly.
- Prefetch commonly accessed queries explicitly.
- Use Vue Query Devtools during development for debugging purposes.
- Optimize mutations with optimistic updates clearly (`onMutate`, `onSuccess`, `onError`).
- Regularly invalidate query cache explicitly after mutations.