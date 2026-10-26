# Form Fields

Labeled number inputs in a grid, a two-option toggle and a full-width submit button, set in a `wm-card`.

## When to use
For the inputs of every student tool. Group related inputs under a `heading-sm` title ("Your debt", "Payoff plan").

## Markup
- Grid: `.wm-fields` (3 columns) or `.wm-fields.wm-fields--2`; one column below 640px.
- Field: `label.wm-label[for]` + `input.wm-input[id]`. Every input has a visible label tied to it with `for`/`id`.
- Toggle: `.wm-toggle > button.wm-toggle__option[aria-pressed]`, exactly one pressed. The pressed option takes `violet-tint` with a `violet` border.
- Submit: `button.wm-btn.wm-btn--block.button` with a one-word verb ("Calculate").
- Checked answers (quiz-style tools): after a "Check my answers" button, add `wm-input--right` or `wm-input--wrong` to each answered input, set `aria-invalid="true"` on the wrong ones (remove it when rechecking), and put the score in a `span` with `aria-live="polite"` beside the button ("3 of 14 correct (2 blank)."). Right takes a `violet` border, `violet-tint` fill and a ✓; wrong takes an `alert` border and text and a ✗.

## The consumer provides
Realistic defaults so the tool shows a result on first use (the payoff calculator opens on $5,000, 18%, $150). Units belong in the label ("Monthly payment ($)", "Annual interest rate (%)"), limits too ("Number of months (up to 600)"), and `min`/`max`/`step` on the input to match.

## Accessibility
Right and wrong never rely on color alone: the ✓ and ✗ marks show it, `aria-invalid` makes a screen reader say "invalid" on a wrong answer, and the live score announces the total. Input borders are `muted` (8.1:1 on `night`), above the 3:1 a control boundary needs; `line` is never used for an input border. Focus is the 2px `gold` ring.
