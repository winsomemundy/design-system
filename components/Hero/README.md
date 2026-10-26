# Hero

The top of the home page: the framed portrait and a live headline on the left, the compass art on the right.

## When to use
Once, at the top of the home page, directly under the Nav and followed by the Role Panels.

## Markup
```
header.wm-hero
  picture.wm-hero__art[aria-hidden]
    source[media="(min-width: 1000px)"] → hero-compass.jpg
    img → hero-art-1774.jpg (srcset hero-art-900.jpg 900w, hero-art-1774.jpg 1774w), alt=""
  .wm-wrap.wm-hero__content
    figure.wm-portrait.wm-hero__portrait > img (headshot.jpg)
    .wm-hero__text
      h1.wm-heading.display-xl (the name)
      p.wm-hero__title.heading-md ("Sr. Technical Product Owner & Educator")
      p.wm-hero__creds.credential ("MSCS • A-CSPO • CSM")
      p.wm-hero__tagline ("Driving value. Empowering teams. Delivering impact.")
      .wm-hero__actions > a.wm-btn.button ("Get in touch") + a.wm-btn.wm-btn--ghost.button ("LinkedIn ↗")
```

## Layout
- 1000px and wider: the compass art sits on the right at the hero's full height (about 287px), fading into `night` on its left edge. The left side sets that height: a 150px portrait and a 420px text column with 40px above and below. The compass is about 206px across, matching the portrait's weight; don't make it smaller, and don't let it float shorter than the hero.
- Below 1000px: the compass becomes a 180px band across the top, fading into `night` on the left (`night` to `night-clear`), with the portrait and text side by side below it.
- 640px and below: a 160px band, then the portrait and text stacked; buttons share the width below 560px.

## The consumer provides
The three compass images from `assets/Images` and the headshot. Every word is live text; never put text back into the art. The art is decorative, so its `alt` is empty and the picture is hidden from screen readers.

## Don't
Widen the text column, add a third button, or place the portrait over the compass.
