<!-- Winsome Mundy design system. Online reference: https://claude.ai/artifact/8FzwMJ54xqNsem4fH3WKxB
     tokens.json is the source; tokens.css is generated from it; components/bundle.css holds the component classes;
     each components/<Name>/preview.html opens in a browser on its own.

     Use in an app (pin a tag; bump it to take updates):
       npm install github:winsomemundy/design-system#v1.3.0
       import '@winsomemundy/design-system/tokens.css'
       import '@winsomemundy/design-system/bundle.css'
     and load the fonts from Google Fonts (link below, under Type). -->

The visual language of winsomemundy.com: a Senior Technical Product Owner and educator's site, and the student tools that link from it. Everything is set on one dark night-violet ground taken from the brand banner, with gold and violet as the only accents. Use it for the website and for every new student app, so a student who moves between them feels they never left.

## Voice and content

- Write in the first person, plainly and confidently: "I translate between executives, engineers, regulators and end users." No hype words, no exclamation marks, no emoji.
- Lead with results and real numbers: "97% attach rate", "zero service disruptions", "in under six months". Numbers carry a unit or a short caption in `body-sm`.
- Name things the way the industry does: A-CSPO, NACHA, GDPR, Form I-9, Azure DevOps. Do not explain acronyms that the audience (hiring managers, product leaders) already knows.
- Student-facing copy is direct and practical: say what the tool does with the student's own numbers ("Enter a balance, interest rate and payment to see your payoff date").
- Labels and buttons are uppercase via CSS, never typed in capitals. Sentence case everywhere else, including headings.
- The brand's three lines, used as written: "Driving value. Empowering teams. Delivering impact." / "Clear vision. Strong priorities. Meaningful outcomes." / "Integrity in every decision. Excellence in every delivery."

## Color

- The page ground is `night`. Use `ink` for the deepest bands (hero, footer) and as the end of the one permitted gradient (`night` to `ink`, top to bottom, on the teaching section).
- Raise a card with `panel` plus a 1px `line` border. Never use shadows.
- The sticky nav sits on `ink-glass` with a 10px backdrop blur.
- `gold` is the signature: eyebrows, credentials, dates, the primary button, the portrait frame, the script lines and the focus ring. `violet` is the working accent: links, job titles, stat units, win-list diamonds and hover states. Do not put gold and violet text side by side in one line.
- Headings and emphasis are `text`; running copy is `muted`. Both read at 7:1 or better on every ground.
- `line` is decorative (about 1.5:1). Never let it be the only signal of a control; pair it with a label, as the ghost button does.
- Mark a selected or highlighted state with `violet-tint` (a chosen option, the area under a chart line, the final row of a schedule) and a quieter highlight with `gold-tint` (milestone rows). Tints sit on `night` or `panel`; never put them on a gold or violet fill.
- `alert` is for errors only: the border of an error Notice and the key words inside it. Always say what went wrong in words.
- No light theme. Pages and apps built on this system commit to the dark ground and set `color-scheme: dark`.

### Color reference

| Token | Hex | Role |
| --- | --- | --- |
| `ink` | `#120C2E` | Deepest ground: hero band, footer |
| `ink-glass` | `#120C2EE0` (88% ink) | Sticky nav bar. Solid: `#130D30` over night |
| `night` | `#1B1442` | Page ground |
| `panel` | `#241A57` | Raised cards |
| `line` | `#3A2E7A` | Hairline rules and borders |
| `violet` | `#9B7BFF` | Working accent: links, hovers, selected |
| `gold` | `#D4AE6A` | Signature accent: labels, primary button, focus |
| `text` | `#ECE8FF` | Headings and emphasis |
| `muted` | `#B5ACD9` | Running copy |
| `violet-tint` | `#9B7BFF24` (14% violet) | Selected and highlighted states. Solid: `#2D225C` on night, `#35286F` on panel |
| `gold-tint` | `#D4AE6A1A` (10% gold) | Milestone rows. Solid: `#2E2346` on night, `#362959` on panel |
| `alert` | `#FF9B9B` | Errors only |
| no fill | `#00000000` | Written `transparent` in CSS: hovered primary buttons, ghost buttons, placeholder tool cards. Not a token |

Every color in the system has a hex code above. Use the 8-digit hex for `ink-glass` and the tints wherever they sit over a token ground; use the solid value only where transparency is not available (an exported image, an email).

## Type

- Three families, all from Google Fonts. Load them with: `https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700&family=Jost:wght@300;400;500&family=Allura&display=swap`.
- `display` (Poppins) for headings, numbers and every uppercase label. `body` (Jost Light, 300) for running text. `script` (Allura) for at most one featured line per section, always in `gold`.
- Headings use `display-xl`, `heading-lg`, `heading-md` and `heading-sm`, with `text-wrap: balance`. Large sizes scale fluidly; each style's note gives its `clamp()`.
- Uppercase labels (`eyebrow`, `credential`, `button`, `date`, `topic`, `nav`) always carry their letter-spacing. Dates and stats use tabular figures.
- Keep running text near 60–75 characters wide.

## Layout and spacing

- The home page opens with the Hero, then the Values Strip, then a short summary paragraph.
- One centered column, `content-max` wide, with `gutter` side padding at every width. Sections are separated by a `line` rule and padded `section-y` (`section-y-sm` on phones).
- Every section opens with an Eyebrow, a `heading-lg` heading and an optional `muted` subline, then its content.
- Cards sit in grids with `grid-gap`; text columns sit `column-gap` apart. Layouts drop to fewer columns at the `breakpoint` tokens and never scroll sideways on a 375px phone.
- Corners are square (`radius-none`). The only rounding is `radius-hairline` on buttons, chips and the focus ring.

## Structure and motifs

- **The compass.** The banner's compass gives the site its bearings: the first four section eyebrows carry N 000°, E 090°, S 180° and W 270°. Use bearings only on those four sections, in that order, never as decoration elsewhere.
- **The gold rule.** A 36px (`rule-mark`) 1px gold line precedes each eyebrow and is the only horizontal flourish.
- **The diamond.** A rotated square marks things: violet-filled 9px in win lists, gold-outlined 13px on the timeline spine, and the ◆ glyph before an award.
- **The offset frame.** The portrait sits on a gold hairline frame offset 14px down and to the right.

## Imagery

- The compass art (`assets/Images/hero-compass.jpg`, with `hero-art-1774.jpg` and `hero-art-900.jpg` for smaller screens) is the Hero's backdrop: the brand banner with every word removed. All text in the Hero is live; never bake text into the art. The original banner (`banner-1774.jpg`) is kept for reference only.
- The portrait (`assets/Images/headshot.jpg`, 4:5) is the only photograph. It shows a real person: never crop it tighter, filter it or reuse it outside Winsome Mundy's own pages.
- No stock photography, illustrations or decorative gradients beyond the teaching section's `night` to `ink` fade.

## Iconography

- There is no icon set and no logo mark; the wordmark is the name set in `brand`. Do not draw a logo.
- Use text glyphs only: ↗ after links that open another site, ◆ before awards, · and • as separators. No emoji.

## Motion

- Hover changes color and border over 0.2s; tool cards also lift 2px. Nothing animates on load.
- Under `prefers-reduced-motion: reduce`, transitions and smooth scrolling are switched off.

## Accessibility

- Keyboard focus is a solid 2px `gold` outline, 3px offset, `radius-hairline` corners (8.2:1 on `night`).
- Text pairs meet WCAG AA in every case listed in the color notes. Do not put `muted` or `violet` text on `line`.
- Every meaningful image has descriptive alt text. The Hero's compass art is decorative (`alt=""`, hidden from screen readers) because its words are live text.
- Sticky navigation reserves scroll padding (72px desktop, 100px phone) so anchored headings are not hidden.

## Building a student tool on this system

- Install the system from GitHub, pinned to a release tag (`npm install github:winsomemundy/design-system#v1.3.0`), import `@winsomemundy/design-system/tokens.css` and then `@winsomemundy/design-system/bundle.css`, load the three fonts (link above), and set `<body class="wm-surface">`. Put only the tool's own additions in its stylesheet, loaded after these two. To take a design-system change, release a new tag and bump it in the tool.
- Reuse the `wm-` component classes rather than restyling: Button for actions, Eyebrow and `heading-lg` for section heads, Impact Stat for results, panels for grouped inputs, Notice for cautions and input errors, Form Fields for inputs, Balance Chart and Data Table for projected results, and a Calculation Explainer for any rule a student may not know.
- Money tools compare every plan with paying the card's minimum in a Comparison Callout. When the plan saves money, say how much interest and how many months it saves; when it costs more, say that just as plainly. When a payment is below the issuer's first-month minimum ($25, or 1% of the balance plus interest if greater), show the minimum-payment warning (see Notice).
- Lay every tool out as a Tool Page: the nav with a "Student tools" link, a tool header, an 860px column of cards, and the footer "A free student tool by Winsome Mundy", linking to winsomemundy.com/#tools.
