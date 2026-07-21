# Inter-society website

Static site built with [Hexo](https://hexo.io/), using the custom `isdcf` theme in `themes/isdcf`.

## Prerequisites

- Node.js 22 (matches `.github/workflows/deploy.yml`)

## Setup

```sh
npm ci
```

## Build

```sh
npm run build
```

Generates the static site into `public/`.

## Local preview

```sh
npm run server
```

Serves the site at `http://localhost:4000` with live rebuilds on file changes.

## Clean

```sh
npm run clean
```

Removes the `public/` output and Hexo's cache. Run this if a build looks stale.

## Deployment

Pushes to `main` trigger [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml), which runs `npm run build` and publishes `public/` to GitHub Pages. No manual deploy step is needed.
