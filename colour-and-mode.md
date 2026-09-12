# Colour & light/dark mode

## The palette model

Equinox Trail uses one set of **semantic colour roles**, defined twice, once for
light mode and once for dark mode. You never style a section with a raw hex
value; you choose which role it uses, and the theme resolves the right colour
for the current mode.

The ten roles, in **Theme settings → Light colour palette** and **→ Dark
colour palette**:

| Role | Used for |
|---|---|
| Page background | The page behind everything |
| Surface | Cards, drawers, raised panels |
| Alternative surface | Secondary panels, striped sections |
| Text | Body and heading text |
| Muted text | Captions, metadata, secondary text |
| Borders | Card borders, dividers, input outlines |
| Primary action | Primary buttons, key accents |
| Text on primary | Label colour on primary buttons |
| Secondary action | Secondary buttons, tags |
| Text on secondary | Label colour on secondary buttons |

Set the two palettes to your brand. Each "text on…" colour must stay readable
against the colour it pairs with. The editor notes this next to the fields.

## The mode switcher

**Theme settings → Colour mode**:

- **Default mode**: `System` (follow the visitor's device), `Light`, or `Dark`.
- **Show light and dark mode switcher**: shows a toggle in the header.
- **Remember visitor choice**: persists the visitor's manual choice on their
  device between visits.

The theme resolves the mode before first paint, so there is no flash of the
wrong palette on load.

## Per-section surfaces

Many sections have a **Background** setting with options like *Default*,
*Surface*, and *Alternative surface*. This selects which palette role the
section sits on, so alternating sections stay consistent in both modes.

## Lifestyle fallback image

**Theme settings → Brand → Lifestyle fallback style** picks one of 19 bundled
art directions (Nordic, Forest, Midnight, Bookshop, Ocean, Industrial, and
more). Where a section can show a lifestyle image but you have not set one,
for example the Hero with its image left blank, the theme uses the bundled
image for the selected style. Setting your own image always takes precedence.
