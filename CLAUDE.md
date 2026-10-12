# CLAUDE.md

Guidance for Claude Code when working in this repository.

## What this is

The website for **Hanley Hitting LLC**: BJ Hanley's hitting lessons and indoor
training facility ("the Lab") in Fredericksburg, Virginia, plus the Cardinals
travel baseball teams (13U, 15U, 17U).

- `index.html` is the whole site: one static page, all CSS and JS inline.
  Sections: hero, quick facts, Lessons, The Lab (+ build-out strip),
  Cardinals Baseball (17U tryouts, Summer 2027 schedule, results), About BJ,
  Reels, Contact.
- `img/` holds responsive WebP photos (640 / 1280, hero up to 1920; never
  upscaled, EXIF stripped) plus the favicon and touch icon. Only files the
  page uses are committed.

## Facts and content rules

- The only facts allowed on the site are the ones BJ published on his Facebook
  (facebook.com/bj.hanley.1), collected in `site-info.md` (kept outside the
  repo, in the "Hanley Hitting - Website Photos" Drive folder). Do not invent
  testimonials, stats, ratings, prices or player names.
- Anything that still needs BJ's OK is an HTML `TODO CONFIRM` comment in
  `index.html`, never a visible claim. Search for `TODO` to find them all.
- Lessons are booked by Facebook message; there is no phone, email or address
  on the site until BJ confirms one.
- Many photos show minors: prefer facility and wide team shots, write alt text
  without names, and keep the parents'-permission TODO until BJ confirms.

## Brand

- Primary: navy `#282165` and silver `#BCBDBF`, sampled from the HH logo.
  Colors live in the `:root` tokens at the top of the `<style>` block.
- The Cardinals section uses its own red/black/white sub-brand.
- The HH logo file is only 472px: never show it larger. BJ should send the
  original vector.
- The hero canvas animation's colors are `ACCENT` / `ACCENT2` in the script
  at the bottom of `index.html`.
