# Tool Page

The frame every student tool shares: the nav bar with a "Student tools" link, a tool header, an 860px column of stacked cards, and the "free student tool" footer.

## When to use
As the outer layout of every student app, so moving between the website and any tool feels like one place. The tool supplies only its own cards.

## Markup
```
div.wm-surface.wm-tool-page
  nav.wm-nav > .wm-wrap.wm-wrap--tool.wm-nav__inner
    a.wm-nav__brand.brand ("Winsome <span>Mundy</span>", to https://winsomemundy.com/)
    a.wm-nav__link ("Student tools", to https://winsomemundy.com/tools)
  main.wm-wrap.wm-wrap--tool.wm-tool-page__main
    header.wm-tool-header
      p.wm-eyebrow.eyebrow (the course topic: "Personal finance · Amortization")
      h1.wm-heading.heading-lg (the tool's name)
      p.wm-tool-header__desc (one line: what the student gets)
    section.wm-card … (inputs, Notice, Comparison Callout, results)
  footer.wm-tool-footer.caption > .wm-wrap.wm-wrap--tool
    "A free student tool by <a href="https://winsomemundy.com/tools">Winsome Mundy</a>. More tools at winsomemundy.com."
```
Also give `html` and `body` a `night` background and zero margin, so the ground shows past the page edges.

## The consumer provides
The topic, the tool's name and its one-line description. Use the same topic on the tool's Tool Card on the website. Keep the footer text exactly as written so every tool credits and links back the same way.

## Spacing
Cards inside a Tool Page stack 24px apart, with card titles `stack-sm` above their content. The column is 860px wide with the standard `gutter`; body text drops to 1rem below `bp-phone`.

## Don't
Add other links to the nav, change the footer wording, or widen the column to the site's 1100px.
