# Hero

The top of the home page: the framed portrait and a live headline on the left, the compass art on the right.

## When to use
Once, at the top of the home page, directly under the Nav and followed by the Role Panels.

## Markup
```
header.wm-hero
  picture.wm-hero__art[aria-hidden]
    source[media="(min-width: 1100px)"] → hero-compass.jpg
    img → hero-art-1774.jpg (srcset hero-art-900.jpg 900w, hero-art-1774.jpg 1774w), alt=""
  .wm-wrap.wm-hero__content
    figure.wm-portrait.wm-hero__portrait > img (headshot.jpg)
    .wm-hero__text
      h1.wm-heading.display-xl (the name)
      p.wm-hero__title.heading-md ("Sr. Technical Product Owner & Educator")
      p.wm-hero__creds.credential ("MSCS • A-CSPO • CSM")
      p.wm-hero__tagline (optional; the website leaves it out)
      p.wm-hero__intro > strong ("Curious by nature. Analytical by design. Creative by choice.") + br + one sentence on its own line ("I build secure, intuitive products for regulated industries, and coach the people who build them.")
      .wm-hero__actions > a.wm-btn.button ("Get in touch") + a.wm-btn.wm-btn--ghost.button ("LinkedIn ↗") + a.wm-btn.wm-btn--ghost.button ("About me →", to /about)
```

## Layout
- 1100px and wider: the compass art sits on the right at the hero's full height (about 323px), fading into `night` on its left edge. The text column sets that height: 450px wide, with 28px above and below. The column is 450px so the three buttons fit on one row. The compass is about 206px across, matching the portrait's weight; don't make it smaller, and don't let it float shorter than the hero.
- Below 1100px: the compass becomes a 140px band across the top, fading into `night` on the left (`night` to `night-clear`), with the portrait and text side by side below it.
- 640px and below: no compass at all (the art is hidden on phones), then the portrait and text stacked; buttons share the width below 560px.
- Beside the text (641px and wider), the portrait's top lines up with the top of the capitals in the name, not the top of the heading's line box: it sits 0.22em of the heading size lower.

## The consumer provides
The three compass images from `assets/Images` and the headshot. Every word is live text; never put text back into the art. The art is decorative, so its `alt` is empty and the picture is hidden from screen readers.

## Don't
Widen the text column, add a fourth button, or place the portrait over the compass. Don't use the tagline with the intro line: two three-part slogans in a row read as filler. A longer intro or another button makes the hero taller and the compass art wider; check that the text stays clear of the art between 1100px and 1200px.
