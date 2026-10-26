# Balance Chart

A line chart of a balance falling to $0 over time: a `violet` line over a `violet-tint` area, gold diamond markers at milestones, a violet diamond where the balance reaches $0, and a "Milestone dates" legend below.

## When to use
In any tool that projects a balance over time (debt payoff, savings, loans), inside a `wm-card` headed "Progress to payoff" with "Balance over time" on the right.

## Markup
An inline SVG `svg.wm-chart[role="img"][aria-label]` (viewBox 630 × 200; plot from x 42 to 620 and y 12 to 170):
- `line.wm-chart__grid` at $0, 25%, 50%, 75% and 100% of the starting balance, dashed (`stroke-dasharray="2,3"`) except the $0 line, each with a `text.wm-chart__axis` label in $k ("$3.8k").
- `polygon.wm-chart__area` under `polyline.wm-chart__line`, one point per payment plus the starting point.
- Per milestone: a dashed `line.wm-chart__marker-line`, a 6px diamond `polygon.wm-chart__marker` and a `text.wm-chart__marker-label`.
- `polygon.wm-chart__end`, a 7px diamond at the last payment, only when the balance actually reaches $0.
- `text.wm-chart__axis` "Now" at the left and the final payment date at the right.

Below the SVG: `.wm-legend > h3.wm-legend__label.topic ("Milestone dates") + .wm-legend__items > .wm-legend__item (span.wm-diamond + text)`. Use `wm-diamond--end` for 100%. Put a related caveat in `p.wm-footnote` after the items.

## The consumer provides
The schedule, scaled with one x scale and one y scale. Milestone labels within 40px of the right edge sit to the left of their marker (`text-anchor="end"`, x − 8) so they are never clipped. A milestone that is not reached reads "not reached within 50 years" in the legend; never print a placeholder date.

## Accessibility
The SVG is one image to a screen reader: `role="img"` with an `aria-label` that states the result, built from the data ("Balance over time: falls from $5,000.00 to $0.00 over 47 months. The payment schedule below lists every month."). Never a generic label like "Balance over time chart". The Data Table that follows is the full text alternative. Axis and marker labels read 7:1 or better on `panel`.

## Don't
Add a second series color, a chart library, gridline numbers that the data does not reach, or animation.
