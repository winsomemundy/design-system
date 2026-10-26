# Tag List

Labelled rows of short outlined tags: a `text` row label on the left and `muted` tags on the right, rows divided by `line` hairlines.

## When to use
For keywords a reader scans rather than reads: domains, standards, integrations, tools. On the home page it closes "How I build products" under the title "Domains and tools", so the skills a recruiter searches for stay on the page. Anything that needs a sentence of explanation belongs in a Principle Card instead.

## Markup
A title `h3.wm-creds__label[id]`, then `dl.wm-taglist[aria-labelledby]`, then one `div` per row: `dt` (the row label) + `dd > span.wm-tag` (one per tag).

## The consumer provides
- Four to six rows, each with two to six tags of one to three words.
- Names written the way the industry writes them (GDPR, Form I-9, Azure DevOps).
- The space above the title; the list itself has no outer margin.

## Layout
Label column 190px wide; tags wrap within their row. At 640px and below the label sits above its tags.

## Don't
Link the tags, color them by category, or use them as buttons or filters: they are plain text in a frame.
