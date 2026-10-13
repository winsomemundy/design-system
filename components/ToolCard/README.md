# Tool Card

A whole-card link to a student app: topic tag, name, what it does, its address and an "Open tool ↗" action.

## When to use
In the Student Tools section, one card per released app. A dashed `--soon` card holds the place for upcoming tools.

## Markup
`a.wm-card.wm-tool > span.wm-tool__topic.topic + h3.wm-card__title.heading-md + p.wm-card__text + span.wm-tool__url + span.wm-tool__open.button`. Placeholder: `div.wm-card.wm-tool.wm-tool--soon` without the url and action.

## The consumer provides
The course topic ("Personal finance · Amortization"), the tool's name, one or two sentences in the student's terms, and its address. The link opens in a new tab.

## States
Hover lifts the card 2px and turns its border `violet`. Replace the placeholder when the next tool ships; keep the grid even.
