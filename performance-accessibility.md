# Performance & accessibility

## Performance

- **System fonts by default.** Every preset ships with a system font stack, so
  a fresh install downloads no web fonts. Switching to a Google font is one
  setting, served from Shopify's CDN.
- **Responsive images** everywhere, with explicit `width`/`height` to avoid
  layout shift, `loading="lazy"` below the fold, and eager + high
  `fetchpriority` for the hero / LCP image.
- **No jQuery, no heavy framework.** Interaction is a small amount of vanilla
  JavaScript (`theme.js`) plus one focused script for the product gallery.
- **CSS is a single stylesheet** built around CSS custom properties, so the
  colour system and both modes cost no extra requests.
- **Adaptive card grids** use container-based sizing rather than many fixed
  breakpoints, which keeps layout CSS small.
- Reveal animations are CSS transitions gated behind `IntersectionObserver`
  and can be turned off entirely.

## Accessibility

- **Light and dark palettes** with explicit "text on colour" roles, and
  editor guidance to keep pairs readable.
- The colour mode is resolved before first paint (no flash), and the mode
  switcher is a real, labelled toggle.
- **Reduced motion:** when the visitor's system prefers reduced motion, reveal
  animations and image zoom are disabled and all content renders immediately.
- Semantic landmarks and heading levels; the product heading is H1 on the
  product page, section headings step down from there.
- Keyboard-operable menus, drawers and accordions with appropriate ARIA state.
- Visible focus styles; skip-to-content link in the layout.
- Passes `theme-check:recommended` with no offenses.

## Browser support

Current versions of Chrome, Edge, Firefox and Safari, on desktop and mobile.
