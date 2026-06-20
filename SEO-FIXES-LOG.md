# SEO Fixes Log

Record of GSC-driven fixes, so we can benchmark whether each one moved clicks/CTR/position afterwards. Check back via GSC 2-4 weeks after a fix and note the outcome.

---

## 18 Jun 2026 — balloon-colour-combinations-that-always-work-together.html

**Trigger:** GSC quick-wins check — "best balloon colour combination" / "balloon colour combination(s)" ranking position 9-11 with 100+ combined impressions but 0 clicks over 28 days.

**Fixes:**
- Title: "Timeless Balloon Colour Combinations" → "Best Balloon Colour Combinations That Always Work" (matches query intent)
- Meta description, og:title/description, twitter:title/description updated to match
- JSON-LD `headline`/`description` updated to match
- `datePublished` was wrongly future-dated `2026-07-25` (page was already indexed since 4 Jun) — corrected to `2026-05-16`, the actual git commit/live date. `dateModified` set to `2026-06-18`
- Visible byline date on page corrected from "25 July 2026" to "16 May 2026"
- `sitemap.xml` `lastmod` corrected from `2026-07-25` to `2026-06-18`
- `CONTENT-CALENDAR.html` — row moved from "July 2026" section (status "🟡 Committed — orphan") to "May 2026" section (status "LIVE"), matching reality

**Benchmark — check back ~mid-July 2026:**
- Did CTR move off 0% for "balloon colour combination(s)" queries?
- Did clicks appear for this page where there were none in the 21 May–17 Jun period?

---

## Template for future entries

```
## [date] — [page]

**Trigger:** [what GSC tool/data flagged this]

**Fixes:**
- [change 1]
- [change 2]

**Benchmark — check back ~[date]:**
- [what metric to compare, and against what baseline]
```
