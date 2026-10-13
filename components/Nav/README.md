# Nav

The sticky top bar: the uppercase wordmark with the surname in `gold`, and section links in `muted`.

## When to use
Once per page, at the top. Links are in-page anchors to sections, in page order.

## Markup
`nav.wm-nav > .wm-wrap.wm-nav__inner > a.wm-nav__brand.brand (+ span for the surname) + ul.wm-nav__links > li > a`

## The consumer provides
The anchors. On the live site the bar is `position: sticky` with an 88% `ink` translucent ground and a 10px backdrop blur, and the page sets `scroll-padding-top` (72px, 100px on phones) so headings are not hidden.

## Phones
Below `bp-nav` (760px) the links move to their own row under the wordmark and scroll sideways with the scrollbar hidden, at 0.76rem; `bundle.css` does this for any nav with `.wm-nav__links`. Never hide the links.

## In a student tool
Replace the section links with one `a.wm-nav__link` reading "Student tools", linked to winsomemundy.com/#tools. See Tool Page.

## Don't
Add icons, a hamburger menu or a button to the bar.
