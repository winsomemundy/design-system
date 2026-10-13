# Notice

A full-width message on `panel`: a `gold` border for a note the reader should weigh, an `alert` border for an error they must fix.

## When to use
Directly above the content it is about, such as above a calculator's results. Use the note (`.wm-notice`) for a caution that does not stop the reader ("the derived monthly payment is less than $25"). Use the error (`.wm-notice.wm-notice--alert`) when the input cannot produce a result ("Payment too low").

## Markup
`div.wm-notice` or `div.wm-notice.wm-notice--alert` with `role="alert"` on the error, so screen readers announce it when it appears. Put the one value the reader needs, such as the minimum payment, in `strong`; in an error it turns `alert`.

## The consumer provides
One or two plain sentences: what went wrong, then what to do or the number that fixes it. Start a note with "Note:".

## Minimum-payment warning
Any money tool that takes or derives a monthly payment shows this note when the payment is below what a card issuer would require in the first month: the greater of $25 or 1% of the balance plus that month's interest. Skip it when the payment clears a balance smaller than that minimum.

Word it with both amounts and the reason, in this order: "the $75.02 monthly payment is below the $125.00 minimum a card issuer would likely require in the first month (1% of the balance plus interest), so a real card would not accept this plan." It is a note, not an error: the tool still shows the schedule so the student can see what the plan would cost.

Pair it with the Comparison Callout, which states how much more interest the plan costs and how many months longer it takes.

## Several cautions at once
Show one notice. Start with "Note:" once and join the cautions as sentences, most serious first: a payment under $25, then the minimum-payment warning, then a plan that finishes before its target because payments are rounded to the cent.

## Accessibility
`alert` reads 7.7:1 on `panel`; `text` 12.9:1. The color is never the only signal: the words name the problem.

## Don't
Stack more than one notice, add icons or emoji, use the alert border for anything but an error, or use a notice for success messages; show results instead.
