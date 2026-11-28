# Xiang Labs

The Astro landing page for [jasonxiang.com](https://jasonxiang.com), with a link to [B2W](https://www.b2w-ai.com/).

## Local development

Use Node 24; `.nvmrc` pins the project major version without changing your global default.

```sh
nvm install
nvm use
npm ci
npm run dev
```

## Production build

```sh
npm run build
npm run preview
```

Astro outputs a static site to `dist/`. Deploy the **contents of `dist/`** to the Hostinger website's document root (`public_html`). The source repository itself is not the publishable site. No Node process is needed on the hosting server.

The initial static build has been deployed directly to Hostinger. `.hostinger/site.json` records the deployment target. Git auto-deployment is not configured; future source changes need a fresh build and deployment.

## Editing

- `src/pages/index.astro`: page content and B2W links.
- `src/styles/global.css`: responsive layout, colors, and typography.
- `src/components/Monogram.astro`: scalable XL mark based on the selected design concept.
- `src/layouts/Layout.astro`: metadata and self-hosted fonts.
- `public/favicon.svg`: matching browser icon.
