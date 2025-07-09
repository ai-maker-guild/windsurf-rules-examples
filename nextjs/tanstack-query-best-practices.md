---
trigger: glob
description: Best practices for data fetching with Tanstack Query (React Query)
globs: ["**/*.tsx", "**/hooks/use*.ts"]
---

# Tanstack Query Best Practices

- Use dedicated custom hooks (`useUsers`, `useOrders`) for queries/mutations.
- Clearly name queries (`queryKey`) consistently (`["users", userId]`, `["orders"]`).
- Leverage caching and stale-while-revalidate settings explicitly.
- Utilize Tanstack Query DevTools during development for debugging and insights.
- Always handle loading, error, and data states clearly and explicitly.
- Consistently use optimistic updates (`onMutate`, `onError`) for mutations.
- Prefetch frequently accessed data explicitly (`queryClient.prefetchQuery`).
- Centralize query client configuration (`QueryClientProvider`) globally at app root.
- Keep queries small and focused; avoid overly broad or complex queries.
- Explicitly manage cache invalidation (`queryClient.invalidateQueries`) upon data mutations.