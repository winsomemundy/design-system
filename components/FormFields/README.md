# Form Fields

Labeled number inputs in a grid, a two-option toggle and a full-width submit button, set in a `wm-card`.

## When to use
For the inputs of every student tool. Group related inputs under a `heading-sm` title ("Your debt", "Payoff plan").

## Markup
- Grid: `.wm-fields` (3 columns) or `.wm-fields.wm-fields--2`; one column below 640px.
- Field: `label.wm-label[for]` + `input.wm-input[id]`. Every input has a visible label tied to it with `for`/`id`.
- Toggle: `.wm-toggle > button.wm-toggle__option[aria-pressed]`, exactly one pressed. The pressed option takes `violet-tint` with a `violet` border.
- Submit: `button.wm-btn.wm-btn--block.button` with a one-word verb ("Calculate").

## The consumer provides
Realistic defaults so the tool shows a result on first use (the payoff calculator opens on $5,000, 18%, $150). Units belong in the label ("Monthly payment ($)", "Annual interest rate (%)"), limits too ("Number of months (up to 600)"), and `min`/`max`/`step` on the input to match.

## Accessibility
Input borders are `muted` (8.1:1 on `night`), above the 3:1 a control boundary needs; `line` is never used for an input border. Focus is the 2px `gold` ring.
