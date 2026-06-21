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

## 21 Jun 2026 — Publish-date audit across June "Already Live" batch

**Trigger:** While publishing fairy-party-balloon-dessert-table-ideas.html on its scheduled date (21 Jun), found its `datePublished` was stuck at 29 May (the writing date, not the actual go-live date — article was "Committed — orphan" until today). Same pattern checked across the rest of the June publish-schedule batch.

**Fixes — datePublished corrected to actual go-live date (dateModified set to 2026-06-21 on all, sitemap lastmod synced to match):**
- fairy-party-balloon-dessert-table-ideas.html: 2026-05-29 → 2026-06-21 (published today, new)
- match-cupcakes-with-balloon-display.html: 2026-06-08 → 2026-06-03
- baby-shower-venue-styling-kent.html: 2026-07-03 → 2026-06-04 (was future-dated)
- trending-childrens-birthday-party-themes.html: 2026-07-05 → 2026-06-06 (was future-dated)
- baby-shower-dessert-table-ideas.html: 2026-06-12 → 2026-06-09
- farm-party-balloon-dessert-table-ideas.html: 2026-05-19 → 2026-06-11
- cling-film-method-multi-coloured-buttercream.html: 2025-05-20 → 2026-06-12 (wrong year, not just wrong date)
- gender-reveal-ideas-uk-guide.html: 2026-06-24 → 2026-06-13 (was 3 days in the future relative to today)
- how-to-choose-balloon-colour-palette.html: 2026-05-23 → 2026-06-15
- puppy-party-balloon-dessert-table-ideas.html: 2026-05-25 → 2026-06-17
- garden-party-balloon-styling-outdoors.html: checked, already correct (2026-06-07) — no change needed

**Other fixes found in the same pass:**
- Title tags missing `| Little Moment Studio` suffix, added to: fairy-party, farm-party, cling-film-method, gender-reveal-ideas-uk-guide, puppy-party (og:title/twitter:title updated to match)
- cling-film-method-multi-coloured-buttercream.html `<title>` was also shorter/inconsistent with its own og:title — aligned to the full "...Multi-Coloured Buttercream" wording
- Visible byline dates corrected on all affected pages (e.g. "May 2026" → "June 2026", "3 July 2026" → "4 June 2026")
- CONTENT-CALENDAR.md and CONTENT-CALENDAR.html both had the same stale "Committed — orphan" rows for fairy-party and the earlier colour-combinations fix — both files now kept in sync

**Why this happened:** the publish workflow writes the article file (with a real-looking date) ahead of its scheduled go-live date, then later adds the journal card + homepage slot on the actual date — but the in-file date metadata was never being updated at that second step.

**How to apply going forward:** when publishing an article from the schedule (adding journal card + homepage slot), always check and correct datePublished/dateModified/byline at the same time — don't assume the existing date is right just because it's in the past.

**Benchmark — check back ~late Jul 2026:**
- Any of these articles future-dated-in-search-results issues resolved in GSC (future dates can suppress freshness signals)?
- Confirm no recurrence on the next scheduled article (23 Jun rescue-pup-dinosaur-party-balloon-dessert-table-ideas.html) — check its date fields *before* publishing this time, not after.

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
