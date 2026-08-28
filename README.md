# Bookhoard Docs

Documentation site for [Bookhoard](https://github.com/bookhoard/bookhoard), a self-hosted EPUB library. Built with [Nimbus](https://nimbus-docs.com).

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

Pushes to `main` build and deploy automatically to GitHub Pages via `.github/workflows/deploy.yml`. The site is served at https://bookhoard.github.io/docs/.

On first deploy, enable Pages for this repo under **Settings → Pages → Source → GitHub Actions**.
