<p align="center">
  <img src="public/logo.png" alt="Bookhoarder" width="96" />
</p>

<h1 align="center">Bookhoarder Docs</h1>

<p align="center">
  Documentation site for <a href="https://github.com/bookhoard/bookhoarder">Bookhoarder</a>,
  a self-hosted EPUB library. Built with <a href="https://nimbus-docs.com">Nimbus</a>.
</p>

<p align="center">
  <a href="https://github.com/bookhoard/docs/actions/workflows/deploy.yml"><img src="https://github.com/bookhoard/docs/actions/workflows/deploy.yml/badge.svg" alt="Deploy"></a>
  <a href="https://docs.bookhoarder.dev"><img src="https://img.shields.io/badge/site-docs.bookhoarder.dev-blue" alt="Site"></a>
  <a href="https://github.com/bookhoard/bookhoarder"><img src="https://img.shields.io/badge/app-bookhoard%2Fbookhoarder-orange" alt="App repo"></a>
</p>

Live at [docs.bookhoarder.dev](https://docs.bookhoarder.dev) — covers
[Features](https://docs.bookhoarder.dev/features),
[Deployment](https://docs.bookhoarder.dev/deployment) (Docker, Cloudflare,
Kubernetes), [Storage](https://docs.bookhoarder.dev/storage) backends, and
the [HTTP API](https://docs.bookhoarder.dev/api/overview).

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

A `Makefile` wraps these as `make dev`, `make build`, `make preview`,
`make typecheck`, `make lint`, and `make clean` — see `make help`.

## Deploy

Pushes to `main` build and deploy automatically to GitHub Pages via
[`.github/workflows/deploy.yml`](.github/workflows/deploy.yml). The site is
served at https://docs.bookhoarder.dev, backed by GitHub Pages' default
`bookhoard.github.io` host via a `CNAME` record and the `public/CNAME` file
in this repo.

On first deploy, enable Pages for this repo under **Settings → Pages →
Source → GitHub Actions**.

## Contributing

This repo holds only the documentation — for the application itself, see
[bookhoard/bookhoarder](https://github.com/bookhoard/bookhoarder). See
[`AGENT.md`](AGENT.md) for the site's file layout and authoring
conventions (frontmatter shape, adding pages, running `nimbus-docs check`).
