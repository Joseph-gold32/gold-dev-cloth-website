# Gold & Dev Website — Responsive Fix Progress

## ✅ Completed

### `style.css` (Shared for index.html)
- [x] Added 768px, 480px, 360px, 320px breakpoints
- [x] Hero grid stacks on mobile
- [x] Category grid fully fluid
- [x] Product grid responsive gaps
- [x] Testimonial, newsletter, footer stacking

### `men.html`
- [x] Added 360px, 320px breakpoints  
- [x] Category/grid sections fluid on mobile
- [x] Product grid responsive (2-col → 1-col on 360px)
- [x] Hero, video, testimonials mobile-sized

### `skin.html`
- [x] Added 360px, 320px breakpoints
- [x] Hero grid stacked
- [x] Category grid single column
- [x] Product grid, tabs, newsletter, footer fixed

### `contact.html`
- [x] Added 768px, 480px, 360px, 320px breakpoints
- [x] Form card and info side stack
- [x] FAQ accordion mobile-friendly
- [x] Social icons and map frame sized down

### `blog.html`
- [x] Added 480px, 360px, 320px breakpoints
- [x] Grid collapses properly (3 → 2 → 1 column)
- [x] Featured post stacks
- [x] Newsletter, picks, footer fixed

### `story.html`
- [x] Added 360px, 320px breakpoints
- [x] Hero, stats, timeline, values, process sections mobile
- [x] Film, quote block, gallery, CTA banner sized down
- [x] Footer stacks

### `auth.html` / `sign.css`
- [x] Added 480px, 360px, 320px breakpoints
- [x] Form inputs, tabs, buttons sized down
- [x] Social auth stacks vertically on small screens

## Notes
- The "not showing other pages" issue is likely because not all `.html` files were committed/pushed to GitHub. Run `git add . && git commit -m "Add all pages + responsive fixes" && git push` to deploy all pages.
- All images use responsive `max-width: 100%` and `object-fit: cover` where applicable.
- All grids use `grid-template-columns: repeat(auto-fill, ...)` or explicit breakpoint overrides.

