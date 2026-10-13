# Timeline Role

One position on the experience timeline: a gold-outlined diamond on a `line` spine, the employer, dates, title, company line, points and an optional award chip.

## When to use
For work history, newest first. Each employer is one `li.wm-role` inside one `ol.wm-timeline`.

## Markup
`ol.wm-timeline > li.wm-role > .wm-role__head (h3.wm-role__name.heading-md + span.wm-role__when.date) + p.wm-role__title + p.wm-role__company + ul.wm-role__points + span.wm-award`

## The consumer provides
Dates as "Mon YYYY – Mon YYYY" with an en dash; the job title and city joined by " · "; two or three points; awards joined by " · " in one chip.

## Don't
Put more than one award chip on a role, or color the title anything but `violet`.
