# Bookhoarder Docs

Documentation site for [Bookhoarder](https://github.com/bookhoard/bookhoarder), a self-hosted EPUB library. Built with [Nimbus](https://nimbus-docs.com).

## Develop

```sh
pnpm install
pnpm dev
```

## Build

```sh
pnpm build   # static output to dist/
pnpm preview
```

## Deploy

Pushes to `main` build and deploy automatically to GitHub Pages via `.github/workflows/deploy.yml`. The site is served at https://docs.bookhoarder.dev, backed by GitHub Pages' default `bookhoard.github.io` host via a `CNAME` record and the `public/CNAME` file in this repo.

On first deploy, enable Pages for this repo under **Settings → Pages → Source → GitHub Actions**.
