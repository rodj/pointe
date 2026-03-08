# Making Money from pointe.com

**Created:** 2026-03-07
**Domain:** pointe.com (registered at Namecheap)
**Owner:** Robert Martin (rodj)

---

## Domain Asset Summary

**What you have:** A 6-letter, single-word .com domain that is:
- Short and memorable
- A real English/French word ("pointe" - ballet term, also geographic: "pointe" as in a promontory)
- Pronounceable and spellable
- Has a built-in niche association (ballet/dance)

**What limits it:** The trailing "e" makes it less intuitive than "point.com" for general use. However, "pointe" is the *correct* spelling for ballet, which is actually an advantage in that niche.

---

## Strategy Overview

Strategies are ranked by **effort vs. realistic return**. The best approach is to layer multiple low-effort strategies simultaneously.

| # | Strategy | Effort | Startup Cost | Realistic Monthly Revenue | Time to First $ |
|---|----------|--------|-------------|--------------------------|-----------------|
| 1 | Domain Parking | None | $0 | $0-5 | Immediate |
| 2 | Ballet Niche Affiliate Site | Medium | $0 | $50-500 | 3-6 months |
| 3 | Vanity Email Sales | Medium | $0-12/yr | $10-100 | 1-3 months |
| 4 | Subdomain Affiliate Pages | Low-Med | $0 | $10-200 | 3-6 months |
| 5 | Subdomain Rental | Low | $0 | $5-50 | 1-6 months |
| 6 | Domain Sale/Lease | None | $0 | One-time $500-5,000 | Unpredictable |
| 7 | Link Shortener Service | High | $5/mo VPS | $0-50 | 6-12 months |

---

## Strategy 1: Domain Parking (Baseline)

**What:** Point the domain to a parking service that shows ads. You earn pennies per click.

**Reality check:** Domain parking is nearly dead for revenue. Type-in traffic (people guessing URLs) is minimal in the age of Google. You might earn $0-5/month. However, it costs nothing and takes 5 minutes to set up, so it's worth doing as a baseline while you build other strategies.

**How:** Namecheap has built-in parking, or use Sedo, Bodis, or ParkingCrew.

**Verdict:** Do this immediately as a placeholder, but don't expect meaningful income.

---

## Strategy 2: Ballet/Dance Niche Affiliate Site (Best ROI)

This is your strongest play. "Pointe" IS the ballet term. The domain has natural authority for this niche.

### Why This Works
- **pointe.com** is arguably the most natural domain for ballet content
- Ballet parents spend serious money: pointe shoes ($80-120, replaced every 2-8 weeks for serious dancers), leotards, tights, warm-ups, bags
- The audience (dance parents, adult dancers) skews educated and has disposable income
- Competition exists but a premium domain gives you an SEO edge

### Content Ideas
- "Best Pointe Shoes for Beginners" (affiliate reviews)
- "When Is My Child Ready for Pointe?" (informational, builds trust)
- "Pointe Shoe Fitting Guide" (evergreen reference content)
- "Best Gifts for Ballet Dancers" (seasonal affiliate goldmine)
- Pointe shoe brand comparisons (Bloch, Capezio, Gaynor Minden, Suffolk)

### Affiliate Programs
- **Amazon Associates** — 4-8% commission on dance supplies
- **Discount Dance Supply** (discountdance.com) — dedicated dance affiliate program
- **Capezio** — direct affiliate program
- **Bloch** — direct affiliate program
- **DanceSupplies.com** — affiliate program available
- **ShareASale / CJ Affiliate** — search for "dance" merchants

### Revenue Model
- Average pointe shoe purchase: ~$100
- At 5% commission: $5 per sale
- 100 visitors/day (very achievable for niche): ~2-5 sales/day = $10-25/day = **$300-750/month**
- This is realistic within 6-12 months with consistent content

### Can This Run on GitHub Pages?
**Yes.** A static site with affiliate links is perfect for GitHub Pages. Use a static site generator (Hugo, Jekyll, or just plain HTML) to create review/guide pages. No server-side code needed.

### Implementation
1. Create a simple, clean static site (Hugo or plain HTML/CSS)
2. Write 10-15 high-quality articles targeting ballet/pointe keywords
3. Embed affiliate links naturally in content
4. Host on GitHub Pages (free)
5. Submit sitemap to Google Search Console
6. Total cost: $0 (just your time writing content, or use AI to help draft)

---

## Strategy 3: Vanity Email Sales

### The Concept
Sell email addresses like `bob@pointe.com`, `mary@pointe.com`, `david@pointe.com`.

### Who Would Buy This?
- People named Pointe (it's a real surname)
- Ballet professionals wanting a professional email
- People who just want a short, clean email address
- Small dance studios wanting studio@pointe.com, info@pointe.com

### Pricing Models
- **$0.99-2.99/month** for basic forwarding
- **$4.99-9.99/month** for full mailbox (send + receive)
- **$19.99-49.99/year** (annual discount)
- **$99 one-time** for lifetime forwarding

### Technical Implementation

**Option A: Cloudflare Email Routing (Free)**
- Move DNS to Cloudflare (free plan)
- Cloudflare Email Routing lets you create unlimited forwarding addresses for free
- Customer gets `bob@pointe.com` forwarded to their personal email
- You manage it manually or build a simple admin interface
- **Limitation:** Forwarding only, customer can't *send* from the address

**Option B: Zoho Mail (Low Cost)**
- Zoho Mail free tier: 5 users
- Zoho Mail Lite: $1/user/month — you charge $3-5/month, pocket the difference
- Full send/receive capability

**Option C: MXRoute ($25-45/year for unlimited)**
- Budget email hosting provider
- Pay a flat annual fee, create unlimited mailboxes
- Sell each for $2-5/month = pure profit after covering the flat fee
- This is the sweet spot for this business model

### Payment Processing
- **Stripe** for recurring subscriptions
- **Gumroad** or **LemonSqueezy** for simpler setup (they handle tax, billing)
- **PayPal** recurring payments

### Marketing
- A simple landing page on pointe.com: "Get your name @pointe.com"
- List on email marketplace sites
- Target ballet/dance forums and communities

### Can This Run on GitHub Pages?
**Partially.** The marketing/landing page can be static on GitHub Pages. But the actual email provisioning needs either:
- Manual setup (you create accounts when someone pays — fine at low volume)
- A simple backend (your existing RjCoreWebApi could handle this)
- A third-party automation (Zapier: Stripe payment → email to you → you provision)

---

## Strategy 4: Subdomain Affiliate Pages

### The Concept
Create niche landing pages on subdomains, each targeting a different topic with affiliate links.

### GitHub Pages and Subdomains — How It Works
**Yes, this works.** Each GitHub repo can have its own custom domain, including subdomains:

```
rodj/pointe-main         → pointe.com (or www.pointe.com)
rodj/pointe-ballet       → ballet.pointe.com
rodj/pointe-camping      → camping.pointe.com
rodj/pointe-cooking      → cooking.pointe.com
```

For each subdomain:
1. Create a repo with static content
2. Enable GitHub Pages
3. Set the custom domain to the subdomain
4. Add a CNAME record at Namecheap: `camping` → `rodj.github.io`

### Best Subdomain Niches
Pick niches with good affiliate programs and buyer intent:

| Subdomain | Niche | Affiliate Programs |
|-----------|-------|-------------------|
| ballet.pointe.com | Dance supplies | Capezio, Bloch, Amazon |
| shoes.pointe.com | Pointe shoes specifically | Dance retailers |
| gifts.pointe.com | Gift guides (seasonal) | Amazon, various |
| books.pointe.com | Book reviews/recommendations | Amazon |
| travel.pointe.com | Travel deals | Booking.com, TripAdvisor |
| tech.pointe.com | Tech reviews | Amazon, Best Buy |
| fitness.pointe.com | Home fitness equipment | Amazon, retailer programs |

### Revenue Per Subdomain
- Each page realistically earns $0-50/month depending on traffic
- 10 subdomains × $20/month average = $200/month
- Low effort per page: each is a single landing page with curated affiliate links

### Implementation
- Each subdomain is a single-page or few-page static site
- Focus on "best X" or "top 10 X" content (high purchase intent)
- Use a consistent template across all subdomains
- Total cost: $0 (GitHub Pages)

---

## Strategy 5: Subdomain Rental

### The Concept
Rent subdomains to small businesses or individuals who want a short, memorable web address.

### Who Would Pay?
- Small dance studios: `mystudio.pointe.com`
- Ballet teachers: `sarah.pointe.com`
- Small businesses who can't afford a premium domain
- Hobbyists who want a cool URL for a project

### Pricing
- $2-5/month or $20-50/year
- Target: 10-20 tenants = $200-1,000/year

### Technical Setup
- Tenant provides their own hosting (GitHub Pages, Netlify, etc.)
- You add a CNAME record pointing their subdomain to their host
- Or: you host a simple page for them (more work, charge more)

### Marketing
- List on forums, social media
- Approach dance studios directly
- The ballet niche site (Strategy 2) can advertise this

---

## Strategy 6: Domain Sale or Lease

### Sell the Domain
Short .com domains have value. Comparable sales:
- 6-letter dictionary-word .com domains typically sell for $1,000-$10,000+
- "Pointe" being a real word (ballet term) with commercial applications adds value
- Realistic asking price: **$2,000-$8,000**

### Lease the Domain
Instead of selling outright:
- Lease for $50-200/month to a business that wants it
- They use it, you retain ownership
- If they stop paying, you get it back
- List on Sedo, Dan.com, or Afternic for lease

### Where to List
- **Dan.com** — modern domain marketplace
- **Sedo.com** — largest domain marketplace
- **Afternic.com** — GoDaddy's marketplace (huge reach)
- **Namecheap Marketplace** — since you're already there

### "For Sale" Landing Page
Even if you pursue other strategies, put a small "This domain is available for purchase" link in the footer. You never know when a ballet company with funding will come looking.

**Verdict:** Keep this as a passive option. Don't actively try to sell unless you get a good offer. The domain appreciates over time as short .coms become scarcer.

---

## Strategy 7: Link Shortener Service

### The Concept
Use `pointe.com/xyz` as a URL shortener (like bit.ly but with a cooler domain).

### Why It's Hard
- Requires server-side redirects (can't do on GitHub Pages)
- Needs a VPS ($3-5/month) or serverless functions
- Competitive market (bit.ly, tinyurl are free)
- Monetization is unclear without massive scale

**Verdict:** Skip this unless you find a specific angle. The effort-to-reward ratio is poor.

---

## Recommended Action Plan

### Phase 1: Immediate (This Weekend) — Cost: $0

1. ~~**Set up GitHub Pages** for `pointe.com` with a simple landing page~~ **DONE 2026-03-07** — repo `rodj/pointe`, main branch, root folder
2. ~~**Add a "Domain for sale/lease" notice** in the footer with a contact email~~ **DONE 2026-03-07**
3. ~~**Set up Cloudflare** (free) for DNS management and email routing~~ **DONE 2026-03-08** — Free plan, nameservers switched from Namecheap BasicDNS to Cloudflare (brett/cass.ns.cloudflare.com). DNS records imported: 4 A records (GitHub Pages), CNAME www, 5 MX records (Google). SSL/TLS set to "Full", confirmed active and serving via HTTPS.
4. ~~**Create `info@pointe.com`** forwarding to your personal email~~ **DONE 2026-03-08** — Already works via existing Google Workspace (colleague manages). Catch-all or alias delivers to colleague. No Cloudflare Email Routing needed; MX records left pointing to Google.
5. ~~**Register with Google Search Console** and submit sitemap~~ **DONE 2026-03-08** — Verified via HTML file method, sitemap.xml submitted. Property: https://www.pointe.com

### Phase 2: Week 1-2 — Cost: $0

1. ~~**Write 3-5 ballet/pointe articles**~~ **DONE 2026-03-08** — 3 articles published: "Best Pointe Shoes for Beginners", "Pointe Shoe Fitting Guide", "When Is My Child Ready for Pointe?"
2. ~~**Sign up for affiliate programs**~~ **PARTIAL 2026-03-08** — Amazon Associates active (tag: pointe09-20, account: rodjmartin@gmail.com). CJ Affiliate account created for Discount Dance (pending approval).
3. ~~**Add affiliate links** to content~~ **DONE 2026-03-08** — Amazon affiliate links added to all 6 product cards in best pointe shoes article.
4. ~~**Create a "Get @pointe.com email" landing page**~~ **DONE 2026-03-08** — email.html with pricing and Formspree inquiry form (endpoint: mwvrpjrg, account: rodjmartin@gmail.com).

### Phase 3: Month 1-2 — Cost: $0-25

1. **Expand to 10-15 articles** on the ballet site
2. **Set up 2-3 subdomain affiliate pages** for non-ballet niches
3. **Set up email hosting** (MXRoute ~$25/year) if there's demand from the landing page
4. ~~**List domain on Dan.com and Afternic**~~ — Deferred indefinitely. Not a priority.

### Phase 4: Month 3-6 — Evaluate and Double Down

1. **Check analytics**: Which pages get traffic? Which affiliate links convert?
2. **Double down on what works**, drop what doesn't
3. **Expand email sales** if there's traction
4. **Consider paid promotion** if affiliate revenue justifies it
5. **Run Google Ads experiment** — Small budget ($3-5/day) targeting "custom email address", "short email address", "ballet email" to drive traffic to email.html. Test whether paid traffic converts to email subscriptions.

---

## The Math: Realistic Year-1 Projection

| Source | Monthly (Low) | Monthly (High) |
|--------|--------------|----------------|
| Ballet affiliate site | $20 | $300 |
| Subdomain affiliate pages | $10 | $100 |
| Email sales (5-10 customers) | $10 | $50 |
| Subdomain rental | $0 | $30 |
| Domain parking | $0 | $5 |
| **Total** | **$40** | **$485** |

**Annual: $480 - $5,820**

This won't replace a salary, but it's passive income from a domain you already own, hosted for free on GitHub Pages. The ballet niche is the real opportunity — if you commit to content, the upper range is achievable.

---

## Technical Notes: GitHub Pages Setup

### Main Site (pointe.com)
```
Repo: rodj/pointe-site
DNS at Namecheap:
  A     @     185.199.108.153
  A     @     185.199.109.153
  A     @     185.199.110.153
  A     @     185.199.111.153
  CNAME www   rodj.github.io
```

### Each Subdomain
```
Repo: rodj/pointe-ballet (for ballet.pointe.com)
DNS at Namecheap:
  CNAME ballet   rodj.github.io

Then in repo Settings → Pages → Custom domain: ballet.pointe.com
```

### Using Cloudflare (Recommended)
If you move DNS to Cloudflare (free), you get:
- Free SSL/TLS
- CDN caching (faster page loads)
- Email routing (free forwarding)
- Analytics
- DDoS protection
- Easy DNS management for all your subdomains

Transfer nameservers at Namecheap to Cloudflare's (keep registration at Namecheap).

---

## Resources

- [GitHub Pages Custom Domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Cloudflare Email Routing](https://developers.cloudflare.com/email-routing/)
- [Amazon Associates](https://affiliate-program.amazon.com/)
- [Discount Dance Supply Affiliate](https://www.discountdance.com/affiliate)
- [Dan.com Domain Marketplace](https://dan.com)
- [MXRoute Email Hosting](https://mxroute.com)
