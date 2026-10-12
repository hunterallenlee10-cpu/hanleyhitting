# CLAUDE.md

Guidance for Claude Code when working in this repository.

## What this is

Website template for **Hanley Hitting**, built from the G1 Baseball and
Softball Training site (same layout and animations), restyled with a light
theme and orange accents. No real Hanley Hitting content has been added yet.

Colors live in the `:root` tokens at the top of each page's `<style>`; the
hero canvas animation has its own `ACCENT` / `ACCENT2` values in the script
at the bottom of `index.html`.

- `index.html` — homepage (hero, testimonials carousel, program, about,
  coach, how it works, what's included, guarantee, FAQ, apply, newsletter)
- `bio.html` — full coach bio
- `partners.html` — official partners and discount codes

Each page is a single static file with all CSS and JS inline.

## Filling in content

- Dashed chips (`<span class="ph">…</span>`) mark text that still needs
  real content. Replace the whole span with the real text.
- Dashed image blocks (`<div class="ph-img …">`) mark photos. Swap each for
  an `<img>` with the same classes (e.g. `about-photo`, `coach-photo`,
  `bio-photo`). Testimonial photos use `<div class="t-photo pend">`;
  see the comment above the testimonials section.
- The logo is a placeholder "HH" SVG in the `.logo` CSS rule on each page;
  the favicon is in the `<link rel="icon">` tag.
- Contact placeholders: `tel:000-000-0000` and `you@example.com` appear on
  every page. The application form button (`#apply`) has `href="#"`.
- Newsletter: set `NEWSLETTER_WEBHOOK` and `NEWSLETTER_EMAIL` in the script
  at the bottom of `index.html`. With no webhook it falls back to a mailto.
- Social links in the footer are `href="#"` on every page.
