# Impact Stat

A row of headline results: a large number with its unit in `violet` and a one-line caption, in cells divided by 1px `line` gaps.

## When to use
Once, at the top of an accomplishments section, for three or four real, verifiable results. In a student tool, for the key outputs (months to payoff, total interest).

## Markup
`.wm-impact > .wm-impact__cell > b.wm-impact__value.stat (+ em.wm-impact__unit) + span.wm-impact__caption.body-sm`

## The consumer provides
Exactly four cells (two per row below `bp-grid`) so no cell sits alone. Keep captions under about 60 characters.

## Don't
Invent or round numbers for effect, or add icons to the cells.
