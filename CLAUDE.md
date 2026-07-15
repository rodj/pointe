# pointe.com

## Project Overview

Static website for **pointe.com** - a ballet/dance niche affiliate site hosted on GitHub Pages.

See [doc/Make_Money_From_pointe.md](doc/Make_Money_From_pointe.md) for the full business plan and monetization strategy.

## Architecture

- **Hosting:** GitHub Pages (free), served from the `main` branch root
- **Domain:** pointe.com, registered at Namecheap
- **DNS:** Configured at Namecheap (or Cloudflare if migrated)
- **Repo:** github.com/rodj/pointe

## Key Files

- `index.html` — Main landing page
- `CNAME` — GitHub Pages custom domain config
- `doc/Make_Money_From_pointe.md` — Business plan and strategy document

## Tech Stack

- Plain HTML/CSS (no build tools, no frameworks)
- Static site — no server-side code required
- GitHub Pages handles SSL and CDN

## Work Log

This project has its own work log at `doc/worklog.md`. Use this instead of the global Personal_Work_Log.md.

## Publishing Schedule

Publishing one article per week to build topical authority and signal activity to Google. New niche sites typically need 3-6 months of consistent content before organic traffic appears.

Publishing day is **Wednesday**. One article per week.

### Published articles (in `articles/`):
- `how-to-sew-pointe-shoe-ribbons.html` — published March 18, 2026
- `how-to-make-pointe-shoes-last.html` — published March 30, 2026
- `pointe-shoe-accessories.html` — published June 22, 2026
- `best-gifts-ballet-dancers.html` — published July 15, 2026 (originally scheduled July 1; caught up late)

### Remaining drafts in `articles/drafts/`:
- `how-pointe-shoes-are-made.html` — publish **July 22, 2026**

After July 22, draft new articles to continue the Wednesday cadence.

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
