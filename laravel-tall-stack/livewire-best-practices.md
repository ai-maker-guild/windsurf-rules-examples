---
trigger: glob
description: Best practices for building dynamic interfaces using Laravel Livewire
globs: ["**/Livewire/**/*.php", "**/*.blade.php"]
---

# Livewire Best Practices

- Keep Livewire components small and focused (single responsibility principle).
- Name Livewire components descriptively (e.g., `UsersTable`, `EditProfileForm`).
- Validate input data within Livewire components explicitly.
- Always use Livewire’s built-in validation methods (`$this->validate()`).
- Leverage Livewire’s lifecycle hooks (`mount()`, `updated()`, `render()`) correctly.
- Emit clear and descriptive events (avoid ambiguous naming).
- Prefer public properties for inputs and private/protected for internal state.
- Utilize pagination with Livewire’s built-in methods rather than custom implementations.
- Be cautious with `wire:model.lazy` to reduce unnecessary network requests.
- Keep `render()` methods clean; delegate heavy lifting to methods or services.
- Utilize `wire:key` whenever looping through items to optimize DOM updates.
- Avoid nesting too many Livewire components deeply; favor clear component boundaries.
- Properly handle exceptions and validation errors gracefully in the UI.