# Changelog

## Unreleased
- **Fixed collection card text contrast.** The white-text-on-image override on
  collection cards (Collection list page, Collection list section) was
  targeting a literal `h3` element and never matched the theme's actual
  markup, so card titles rendered in the standard dark heading colour and
  were hard to read over darker photography. Added a **Collection name
  colour** setting on the Collection list page section (defaults to white,
  matching the section's dark gradient overlay) and fixed the underlying
  selector.
- **Nordic preset reworked** so it is genuinely distinct from the Equinox preset:
  cool grey-white palette, dusty slate-blue accent, square 0&nbsp;px corners,
  uppercase UI labels, wider page and larger spacing, lighter and smaller
  headings.
- New **Theme demo grid** section and `page.demo` template for a preset
  comparison page.

## 1.8.0
- Cart race-condition fixes and hardening of the add-to-cart / drawer flow.
- Product gallery: blank-image fallback handling.
- Reworked the metafield accordion to use real theme blocks, rendered through
  the new **Flexible blocks** section on the product template.
- Standalone **Share** block with per-network toggles and centred / left
  alignment.
- Tooling and dependency security pass; removed dead code.
- Theme Store submission fixes.

## 1.6.x series
- Availability and gallery work.
- Map and accordion-item blocks gained full functionality.
- Product information block refinements.

---

For older internal revisions, see the theme repository history.
