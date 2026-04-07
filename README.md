# Circuitscape Website

Source for [circuitscape.org](https://circuitscape.org), built with [Franklin.jl](https://github.com/JuliaDocs/Franklin.jl).

## Local development

Install [Julia](https://julialang.org/downloads/), then:

```sh
julia --project=. -e 'using Pkg; Pkg.instantiate(); using Franklin; serve()'
```

This starts a local server at `http://localhost:8000` with live reloading.

## Project structure

- `_css/` — Stylesheets (`main.css`, `normalize.css`)
- `_layout/` — HTML templates (`head.html`, `header.html`, `foot.html`, `page_foot.html`)
- `_assets/img/` — Images
- `pubs/` — PDF publications
- `downloads/` — Legacy Circuitscape 4 installers
- `config.md` — Site-wide configuration (title, description, docs link)
- `*.md` — Page content (Franklin Markdown with TOML frontmatter)
- `__site/` — Generated output (not committed)

## Deployment

Pushing to `master` triggers the [Build and Deploy](.github/workflows/deploy.yml) GitHub Actions workflow:

1. Checks out the repo
2. Installs Julia with cached packages
3. Builds the site with `Franklin.optimize()`
4. Deploys to GitHub Pages via `actions/deploy-pages`

The site is published at [circuitscape.org](https://circuitscape.org). DNS is configured via the `CNAME` file.

Dependabot checks for GitHub Actions updates monthly.
