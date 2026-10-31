# Nav

The sticky top bar: the uppercase wordmark with the surname in `gold`, and page links in `muted`, with the current page in `gold`.

## When to use
Once per page, at the top. The website has five pages: the wordmark links home (`/`), and the links read Product (`/product`), Teaching (`/teaching`), Tools (`/tools`), About (`/about`) and Contact (`#contact`, the contact block that closes the page; on a page without one, `/#contact`).

## Markup
`nav.wm-nav > .wm-wrap.wm-nav__inner > a.wm-nav__brand.brand (+ span for the surname) + ul.wm-nav__links > li > a`. The link to the page you're on carries `aria-current="page"`, which turns it `gold` and tells screen readers which page this is.

## The consumer provides
The links, with `aria-current` on the current page's. On the live site the bar is `position: sticky` with an 88% `ink` translucent ground and a 10px backdrop blur, and the page sets `scroll-padding-top` (72px, 100px on phones) so headings are not hidden.

## Phones
Below `bp-nav` (760px) the links move to their own row under the wordmark and scroll sideways with the scrollbar hidden, at 0.76rem; `bundle.css` does this for any nav with `.wm-nav__links`. At 420px and below the gap narrows to 14px and the letter-spacing to 0.08em, so all five links fit a 375px phone without scrolling; on narrower phones they still scroll. Never hide the links.

## Adding a link
Five links is the most the bar holds. Before adding a sixth, check the row at 375px: if it no longer fits, merge or drop a page rather than shrinking the type further.

## In a student tool
Replace the section links with one `a.wm-nav__link` reading "Student tools", linked to https://winsomemundy.com/tools. See Tool Page.

## Don't
Add icons, a hamburger menu or a button to the bar.
