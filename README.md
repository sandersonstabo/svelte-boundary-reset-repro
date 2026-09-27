# svelte:boundary reset crash repro

```sh
pnpm install
pnpm dev
```

Open `/`, click **fail**, then **ok** and **home**. Each navigation logs `TypeError: Cannot read properties of null (reading 'r')` from `handleError` (see the browser console).
