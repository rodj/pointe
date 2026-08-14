# pointe.com

## Project Overview

Static website for **pointe.com** - a ballet/dance niche affiliate site hosted on GitHub Pages.

See `Make_Money_From_pointe.md` in the **private** `rodj/pointe-docs` repo (cloned at
`C:\src\pointe-docs`) for the full business plan and monetization strategy.

## IMPORTANT: This repo is PUBLIC and everything in it is served on the live site

`rodj/pointe` is intentionally public — it is just the source of a public website, so the HTML,
CSS, affiliate tags and analytics IDs are all visible on pointe.com anyway.

The non-obvious part: **GitHub Pages copies every tracked file to the live site verbatim, including
Markdown.** Files are not private just because they aren't linked from a page. Project docs were
publicly readable at `https://www.pointe.com/doc/Make_Money_From_pointe.html` until 2026-08-06.

Therefore:

- **Never put anything non-public in this repo** — no business plans, revenue figures, negotiating
  positions, personal email addresses, credentials, or internal notes. Private docs go in
  `rodj/pointe-docs`.
- `doc/` is gitignored here to prevent it coming back.
- `_config.yml` excludes `CLAUDE.md`, `README.md`, `doc/` and `articles/drafts/` from the built site.
  **Anything added to this repo that is not part of the public website must be added to that list.**

## Architecture

- **Hosting:** GitHub Pages (free), served from the `main` branch root
- **Domain:** pointe.com, registered at Namecheap
- **DNS:** Configured at Namecheap (or Cloudflare if migrated)
- **Repo:** github.com/rodj/pointe

## Key Files

- `index.html` — Main landing page
- `CNAME` — GitHub Pages custom domain config
- `_config.yml` — Jekyll config; its `exclude:` list keeps non-website files off the live site
- Business plan and work log live in the private `rodj/pointe-docs` repo (`C:\src\pointe-docs`)

## Tech Stack

- Plain HTML/CSS (no build tools, no frameworks)
- Static site — no server-side code required
- GitHub Pages handles SSL and CDN

## Work Log

This project's work log is `worklog.md` in the private `rodj/pointe-docs` repo, cloned at
`C:\src\pointe-docs\worklog.md`. Use this instead of the global Personal_Work_Log.md.

It was moved out of this repo on 2026-08-06 because it was publicly readable on the live site.
Remember to commit and push `pointe-docs` separately after updating it.

## Publishing Schedule

Publishing one article per week to build topical authority and signal activity to Google. New niche sites typically need 3-6 months of consistent content before organic traffic appears.

Publishing day is **Wednesday**. One article per week.

### Published articles (in `articles/`):
- `how-to-sew-pointe-shoe-ribbons.html` — published March 18, 2026
- `how-to-make-pointe-shoes-last.html` — published March 30, 2026
- `pointe-shoe-accessories.html` — published June 22, 2026
- `best-gifts-ballet-dancers.html` — published July 15, 2026 (originally scheduled July 1; caught up late)
- `how-pointe-shoes-are-made.html` — published July 23, 2026 (originally scheduled July 22; caught up late)
- `breaking-in-pointe-shoes.html` — published August 6, 2026
- `pointe-shoe-foot-care.html` — published August 14, 2026 (originally scheduled August 12; caught up late)

### Remaining drafts in `articles/drafts/`:
- (none — draft new articles to continue the Wednesday cadence)

### Publishing checklist (each article):
1. Copy from `articles/drafts/` to `articles/`
2. Fix stylesheet path (`../../style.css` → `../style.css`)
3. Add Google Analytics snippet (same as other articles)
4. Add nav link to all existing pages
5. Add homepage card to `index.html`
6. Add entry to `sitemap.xml`
7. Commit and push

## Git Policy

Do NOT commit unless explicitly asked. See global CLAUDE.md for details.
