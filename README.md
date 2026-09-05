# Unbound Silicon Website

This repository contains the Hugo source for the Unbound Silicon website at
[unboundsilicon.com](https://unboundsilicon.com/).

## Local preview

Install Hugo Extended, then run:

```sh
hugo server
```

Open <http://localhost:1313/> in a browser. Hugo rebuilds the site when source
files change.

## Production build

```sh
hugo --minify
```

The generated site is written to `public/`. This directory is build output and
is not committed to Git.

## Project structure

- `content/` contains pages, project descriptions, and posts.
- `layouts/` contains Hugo templates.
- `assets/` contains resources processed by Hugo, including CSS.
- `static/` contains files copied directly into the generated site.
- `hugo.toml` contains site configuration and navigation.

## Licensing

Website code—including templates, CSS, scripts, and configuration—is available
under the [BSD 2-Clause License](LICENSE).

Except where otherwise noted, original written content under `content/` is
available under the [Creative Commons Attribution 4.0 International
License](LICENSE-CONTENT.md). Unbound Silicon names, logos, and trademarks are
not included in these license grants. Third-party material remains subject to
its identified terms.
