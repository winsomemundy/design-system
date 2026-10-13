# Comparison Callout

A gold-framed panel that compares the student's plan with paying the card's minimum each month, in one sentence with the two numbers that matter in `gold`.

## When to use
In every money tool, directly after the inputs and any Notice, before the detailed results. It answers the first question a student has: is this plan better or worse than paying the minimum?

## Markup
`div.wm-callout > p.wm-eyebrow.eyebrow ("Compared to paying the minimum") + p.wm-callout__text` with the amounts in `strong`.

## Versions
- **Saves money:** "You'll save **$4,555.02 in interest** and finish **175 months sooner**."
- **Costs more:** "This plan costs **$30,012.77 more in interest** and takes **332 months longer** than paying the minimum each month." Use it whenever the plan pays more total interest than the minimum path; say it as plainly as a saving. If the plan itself is not paid off within 50 years, add "+" to the amount and say "and is not paid off within 50 years" instead of the months.
- **Minimum never pays off:** when new charges keep the minimum-payment balance from ever reaching $0: "Under minimum payments, your ongoing charges would cause your balance to **grow indefinitely** — you'd never pay it off. Your plan saves **$44,010.83+ in interest**." The "+" marks that the true saving is larger. (Example: $5,000 at 18% APR, $300 a month, $50 of new charges a month.)

## The consumer provides
The interest difference and the month difference against a minimum-payment schedule built with the same rule as the minimum-payment warning (the greater of $25 or 1% of the balance plus interest, each month). Round amounts to the cent and months to whole numbers. Show nothing when the plan exactly matches the minimum.

## Accessibility
`gold` reads 7.4:1 and `text` 12.9:1 on `panel`. The sentence carries the meaning; color only emphasizes it.

## Don't
Use red or green to signal better or worse, add icons or arrows, show more than one callout, or round a cost down to make a plan look better.
