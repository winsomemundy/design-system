# Data Table

A dense numeric table on `panel`: gold uppercase column heads over a gold rule, hairline row rules, tabular figures, and tinted highlight rows with small square pills.

## When to use
For schedules and other row-per-period data (a payment schedule, an amortization table, a frequency table).

## Markup
`h2.wm-card__title[id]`, then `div.wm-table-scroll[tabindex="0"][role="region"][aria-labelledby]` (pointing at the heading) `> table.wm-table`, with `caption.wm-sr-only` as the table's first child ("Payment schedule, one row per monthly payment"). Numbers right-aligned (the default); text columns take `wm-left` on both `th` and `td`. Secondary numbers (a row number, interest) take `td.wm-dim`; the key result per row (the ending balance) takes `td.wm-strong`.

## Highlights
- `tr.wm-row--milestone` (`gold-tint`) with `span.wm-pill` for a milestone row ("25%").
- `tr.wm-row--final` (`violet-tint`) with `span.wm-pill.wm-pill--final` for the row where the goal is reached ("100%").

## The consumer provides
Values already formatted (currency to the cent). The table keeps a 600px minimum width and scrolls sideways inside `.wm-table-scroll` on phones; the page never scrolls sideways.

## Accessibility
On phones the table scrolls sideways inside its wrapper. `tabindex="0"` lets keyboard users focus the wrapper (it takes the gold focus ring) and scroll it with the arrow keys; `role="region"` and the label tell screen readers what it is. The hidden caption names the table for screen readers without repeating the visible heading.

## Don't
Color whole numbers red or green, zebra-stripe rows, or hide columns on phones instead of scrolling.
