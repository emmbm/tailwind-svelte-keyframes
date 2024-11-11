# Reproduction of broken svelte + tailwind global keyframes behavior

Tailwind's vite plugin version `4.0.0-alpha.32` breaks svelte's handling of global animation keyframes defined using the `-global-` prefix.
Revert to `4.0.0-alpha.31` or a prior version to observe the behavior working as expected.

```bash
# Install
pnpm install

# Run dev to observe broken behavior
pnpm dev
```
