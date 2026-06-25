# Aries Website

Static landing page for [Aries Agent](https://github.com/haozhongsheng/aries).

Aries is presented here as a trusted runtime for autonomous agents: the host
keeps identity and secrets, tool access stays scoped, and every run leaves
inspectable evidence.

## Preview

This site has no build step. Open the page directly:

```bash
open index.html
```

Or serve the directory locally if you want browser behavior closer to a deployed
static host:

```bash
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/`.

## Files

- `index.html`: single-page content and semantic structure.
- `styles.css`: layout, typography, responsive behavior, and visual system.
- `assets/aries-logo.jpg`: canonical Aries logo asset used by the page.

## Content Direction

Keep the page simple, sharp, and easy to understand on first read.

- Lead with "Run agents you can trust" instead of abstract infrastructure
  language.
- Avoid direct competitor comparisons in hero copy.
- Treat `local-first` as a deployment detail, not the headline promise.
- Keep the three core claims aligned with Aries documentation:
  host-held trust, narrow execution scope, and clear run history.
- Preserve the one-screen layout: the hero, trust cards, quickstart, and footer
  should fit without page scrolling on common desktop viewports.

## Design Notes

- Use the existing Aries logo from `assets/aries-logo.jpg`.
- Keep the cyan-on-black brand direction, but prefer restraint over decoration.
- Favor fewer sections, stronger spacing, and readable copy.
- The stylesheet query string in `index.html` is used as a lightweight cache
  bust when CSS changes.

## Deployment

Deploy the repository root as a static site. No package install, bundler, or
generated output directory is required.

For GitHub Pages, publish from the `main` branch root. For any other static
host, upload:

```text
index.html
styles.css
assets/
```
