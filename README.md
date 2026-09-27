# Guane documentation site

Documentation and tutorials for [Guane](https://github.com/alarconvv/Guane), a local R/Shiny app for phylogenetic comparative methods.

Published at <https://alarconvv.github.io/guane-site/>.

## Preview and build

Requires [Quarto](https://quarto.org) 1.6 or later. No R code runs during the build.

```bash
quarto preview
```

```bash
quarto render
```

The rendered site is written to `_site/`, which is not committed.

## Deploy

Every push to `main` builds the site and publishes it to GitHub Pages through `.github/workflows/deploy.yml`. In the repository settings, set **Pages → Source** to **GitHub Actions**.

## Layout

| Path | Contents |
| --- | --- |
| `index.qmd`, `faq.qmd` | Home and FAQ |
| `get-started/` | Install, interface tour, example data |
| `tutorials/` | One tutorial per module; `tutorials/advanced/` covers the advanced controls |
| `reference/` | Input formats, exports, scientific limitations |
| `example/` | The bundled example tree and trait table, copied from `inst/example/` in the Guane repository. Keep them in sync when the app's example changes. |
| `images/` | Screenshots captured from the running app |
| `theme/` | Light and dark SCSS themes |
| `_includes/` | Skip link and accessibility fixes injected into every page |
| `DESIGN.md` | The site's design system (not rendered) |

## Writing rules

- Name only interface labels that exist in the app (`R/ui_mod_*.R` in the Guane repository), styled as `[Label]{.ui}`.
- The example data are synthetic. Never present results from them as biological evidence.
