# ngpaladi.github.io

Noah Paladino's personal/academic site, built with [Hugo](https://gohugo.io/).

## Development

```sh
hugo server -D
```

Serves the site locally at http://localhost:1313 with drafts enabled and live reload.

## Build

```sh
hugo --minify
```

Outputs the static site to `public/`.

## Structure

- `hugo.toml` — site config (title, baseURL, params)
- `data/` — research and projects entries rendered on the homepage
- `layouts/` — page templates (`index.html`, `404.html`) and `layouts/partials/`
- `static/` — assets served as-is (images, CSS, fonts, PDF, favicon, `CNAME`)

## Deployment

Deployed to GitHub Pages via the GitHub Actions workflow in
`.github/workflows/hugo.yml`. The repo's Pages source must be set to
"GitHub Actions" under Settings → Pages.
