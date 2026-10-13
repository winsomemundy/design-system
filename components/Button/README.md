# Button

A square-cornered uppercase action: gold fill for the main action, ghost outline for a secondary one.

## When to use
Primary (`.wm-btn`) for the one action you most want, such as "Get in touch". Ghost (`.wm-btn.wm-btn--ghost`) beside it for a secondary or external link. At most one primary per group.

## Markup
`a.wm-btn.button` or `button.wm-btn.button`; add `.wm-btn--ghost` for the outline version. Add ↗ to the label when it opens another site.

## States
Primary hover empties the fill and turns the label `gold`. Ghost hover turns border and label `violet`. Focus is the system's 2px gold ring.

## Phones
Below `bp-phone` buttons in a row share the width (`flex: 1 1 auto`, centered label).

## Accessibility
Ink on gold reads 9.0:1. The ghost border is `line`, below 3:1, so the ghost label (14.3:1) is what identifies it: never make a ghost button icon-only.
