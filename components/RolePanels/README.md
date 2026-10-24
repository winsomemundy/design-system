# Role Panels

Two side-by-side panels, one for each of Winsome Mundy's roles: Senior Technical Product Owner (violet) and Educator (gold). Each gives a one-line thesis, a short story, three proof points, a quote and a link to its section.

## When to use
On the home page directly after the Values Strip, under an Eyebrow ("Product and classroom") and a `heading-lg` line ("Two roles, one habit: making complex things clear."). It replaces a résumé-style summary paragraph.

## Markup
`.wm-roles__grid > article.wm-role-panel.wm-role-panel--product` and `article.wm-role-panel.wm-role-panel--educator`, each with:
`h3.wm-role-panel__label` (the role) · `p.wm-role-panel__thesis` (one first-person sentence) · `p.wm-role-panel__body` (two or three sentences) · `dl.wm-role-panel__proof` (three `div > dt + dd`) · `figure.wm-quote` · `a.wm-role-panel__link` ("See my experience →" / "See my teaching →").

## Color
The modifier sets `--wm-accent`: `violet` for product, `gold` for teaching. The label, diamond, proof numbers, quote mark and link take it; everything else stays `text` and `muted`.

## The consumer provides
- A thesis of five to eight words in Winsome's voice ("I turn regulation into roadmaps." / "I make the math make sense.").
- Proof points that don't repeat numbers shown elsewhere on the page (the accomplishments row already has 97%, #1, 0 and <6 mo). Keep each `dt` to a few characters: a number, a year or a short word.
- A real quote of similar length in each panel, so the two panels end at the same height.

## Layout
Side by side from 901px, stacked below. At 560px and below the proof points become rows with the number on the left.

## Don't
Add a third panel, use the accent for body text, or put an accent bar on the panel edge.
