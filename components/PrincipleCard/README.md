# Principle Card

A `panel` card for one way of working: a `heading-sm` name, a gold one-line idea, a short paragraph and, at the foot, one line of proof under a violet "Proof" label.

## When to use
On the Product page's "How I build products" section (eyebrow "Product principles"): four cards, two by two. Use it wherever a claim about how Winsome works needs evidence from a real role. For a list of skills or keywords with no story, use the Tag List instead.

## Markup
`.wm-grid.wm-grid--2 > article.wm-card.wm-principle`, each with:
`h3.wm-card__title.heading-sm` (two to four words) · `p.wm-principle__thesis` (one sentence) · `p.wm-card__text` (two sentences) · `p.wm-principle__proof > span.wm-principle__proof-label.topic` ("Proof") + the proof sentence.

## The consumer provides
- Proof that is true and checkable: a named employer or a shipped result ("Defined NACHA-mandated encryption of ACH data at rest, delivered ahead of the deadline."). Never a claim the work can't back up.
- An even number of cards, so the two-by-two grid has no gap. The proof line sits at the bottom of every card, so cards in a row line up even when their paragraphs differ in length.

## Layout
Two across from 761px, one below. The proof rule is a `line` hairline.

## Don't
Add icons or numbers, color the paragraph, or use more than one proof sentence.
