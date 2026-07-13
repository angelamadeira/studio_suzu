# Studio Suzu

Brand guidelines for **Studio Suzu** — an authorial mold studio for confectionery.

**→ [Read the brandbook](https://angelamadeira.github.io/studio_suzu/)**

## What's here

| | |
|---|---|
| `index.html` | The brandbook. One self-contained file. |
| `Studio_Suzu_Logo/` | Source vectors (SVG) and rasters (PNG) for every logo variant and flavor seal. |
| `licenses/` | SIL Open Font License for the embedded typefaces. |

## The brandbook is one file

`index.html` carries everything inside it: the vectors, the wave illustration, and the Jost and
Cormorant typefaces as embedded `woff2`. It fetches nothing over the network — open it from a USB
stick on a plane and it renders whole.

That means you can also just **email the file**. Hosting is a convenience, not a requirement.

## It gives you the assets

Inside the brandbook, every logo, flavor seal and pattern has a `SVG ↓` button:

- **Logos and seals** export as standalone SVG. The vectors live in a shared `<defs>` and the colors
  come from CSS, so the export resolves every `<use>` and bakes the computed paint into attributes —
  otherwise the downloaded file would be empty.
- **Patterns** export at **300 × 300 mm**, vector, ready for packaging.
- **Typefaces** export as the same `woff2` that the page itself uses, plus a `Studio_Suzu_Type.css`
  with the roles.
- **Every color value** — hex and `rgba` alike — copies to the clipboard on click.

## Light and dark

The brandbook follows your system theme and has a toggle. The dark theme is not an inversion: on
charcoal the accent colors become *type*, because on light none of them reaches 4.5:1. That flip is
documented in the palette section, with measured contrast ratios.

Printing always produces the light theme, whichever theme is on screen.

## Typefaces

| | | |
|---|---|---|
| Jost | variable, 100–900 | [SIL OFL 1.1](licenses/OFL-Jost.txt) |
| Cormorant | variable, 300–700, italic only | [SIL OFL 1.1](licenses/OFL-Cormorant.txt) |

The OFL permits embedding and redistribution. The license texts travel with the fonts, as it requires.

## Note

This repository is public so the page can be served, but it carries `robots.txt` and a `noindex`
meta tag. Search engines will not list it. That is discretion, not privacy — anyone with the link
can read it.

The brand marks, palette, photography direction and copy are © Studio Suzu.
