# Guane documentation site

Documentation and tutorials for [Guane](https://github.com/alarconvv/Guane)

Published at <https://alarconvv.github.io/guane-site/>.

## Preview and build

Requires [Quarto](https://quarto.org) 1.6 or later. No R code runs during the build.

```bash
quarto preview
```

```bash
quarto render
```

The rendered site is written to `_site/`

## Layout

| Path | Contents |
| --- | --- |
| `index.qmd`, `faq.qmd` | Home and FAQ |
| `get-started/` | Install, interface tour, example data |
| `tutorials/` | One tutorial per module; `tutorials/advanced/` covers the advanced controls |
| `reference/` | Input formats, exports, scientific limitations |
| `example/` | The bundled example tree and trait table |
| `images/` | Screenshots captured from the running app |
| `theme/` | Light and dark SCSS themes |
| `_includes/` | Skip link and accessibility fixes injected into every page |
| `DESIGN.md` | The site's design system (not rendered) |
