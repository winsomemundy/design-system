# Calculation Explainer

A small link that opens a two-column panel: the rule in plain words and a formula box on the left, the student's own numbers worked through on the right.

## When to use
Wherever a tool uses a rule the student may not know (how a minimum payment is calculated, how interest accrues). Place it right-aligned directly above the result it explains. Closed by default.

## Markup
`.wm-explainer > button.wm-explainer__toggle[aria-expanded] + .wm-explainer__panel`. Left: `.wm-explainer__label.topic` "Formula", `.wm-explainer__text`, `.wm-formula` (with `span.wm-formula__or` between alternatives), `.wm-explainer__note` naming the source of the rule. Right: `.wm-explainer__label.topic` "Your first payment" (or the step it explains), `.wm-calc` rows of `span` label + `span` amount, and a `.wm-calc__total` row in `gold`.

## The consumer provides
The student's real numbers, recomputed each time the result changes. The toggle text ends in ▾ when closed and ▴ when open, and `aria-expanded` matches.

## Don't
Use it for content the student needs in order to read the result; that belongs in a Notice.
