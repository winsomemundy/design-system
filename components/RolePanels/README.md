# Role Panels

Two side-by-side panels, one for each of Winsome Mundy's roles: Senior Technical Product Owner (violet) and Educator (gold). Each gives an icon and label, a one-line thesis, a short story, three proof cards, a quote and a link to its section.

## When to use
On the home page directly after the Hero, under an Eyebrow ("Product and classroom") and a `heading-lg` line ("Making complex things clear", with no closing period). It replaces a résumé-style summary paragraph.

## Markup
`.wm-roles__grid > article.wm-role-panel.wm-role-panel--product` and `article.wm-role-panel.wm-role-panel--educator`, each with:
`h3.wm-role-panel__label` (an inline `svg[aria-hidden]` icon, then the role: layers for product, a graduation cap for educator) · `p.wm-role-panel__thesis` (one first-person sentence) · `p.wm-role-panel__body` (two or three sentences) · `dl.wm-role-panel__proof` (three `div`, each `dt` > `span.wm-role-panel__icon > svg[aria-hidden]` + `span.wm-role-panel__stat`, then `dd` > `strong` title + one line of detail) · `figure.wm-quote` · `a.wm-role-panel__link` ("See my experience →" / "See my teaching →").

Where the two roles meet, a full-width band follows the grid inside the same `.wm-wrap`:
`div.wm-roles__meet > div.wm-roles__meet-head (p.wm-roles__meet-label, h3.wm-role-panel__thesis) + p.wm-roles__meet-body`. Its label reads "Where the two roles meet" and its title names the shared practice ("Mentoring"). A violet-to-gold rule along the top joins the two accents. (The `span.wm-roles__meet-marks` diamonds were retired in v1.7.5; the style stays so older pages don't break.)

## Color
The modifier sets `--wm-accent`: `violet` for product, `gold` for teaching, and `--wm-accent-tint` (`violet-tint` / `gold-tint`) for the circles behind the proof icons. The label and its icon, proof icons and numbers, quote mark and link take the accent; everything else stays `text` and `muted`.

## The consumer provides
- A thesis of five to eight words in Winsome's voice ("I turn regulation into roadmaps" / "I make the math make sense"), with no closing period: it reads as a headline.
- Proof points that don't repeat numbers shown elsewhere on the page, except the one headline result the page leads with (97%, also in the accomplishments row). Don't repeat a story the band tells: the BHG mentoring result lives in the band, not in a proof point. Keep each number to a few characters (97%, <6 mo, 2×) so it sits beside its icon; in a narrow card all three icons move above their numbers together. Titles are two to five words; the detail line is one sentence.
- A real quote of similar length in each panel, so the two panels end at the same height.

## Layout
Side by side from 901px, stacked below. The proof cards sit three across, and one per row at 560px and below. The band puts its title beside its text from 901px and stacks below.

## Don't
Add a third panel, a second band, use the accent for body text, put an accent bar on the panel edge, put a diamond before the labels, or use icons from outside the system's set (see Iconography).
