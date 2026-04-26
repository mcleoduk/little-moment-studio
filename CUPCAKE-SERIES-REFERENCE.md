# Cupcake Series — Article Reference

This document is the template and content reference for all cupcake tutorial articles on the Little Moment Studio journal. Use it when building new articles in the series.

---

## SEO Rationale

Cupcake and dessert table articles help SEO **because the audience is identical** — someone searching for baby shower cupcake ideas, Halloween dessert table ideas, or birthday table styling is clearly planning an event and is likely to also need balloons, a backdrop and a stylist.

**What these articles do:**

1. **Bring in party-planning traffic earlier in the journey** — before someone searches "balloon stylist Sittingbourne", they may be searching "baby shower dessert table ideas". This puts Little Moment Studio in front of them at the research stage.

2. **Build topical authority** — Google needs to understand this site is about parties, celebrations, balloon displays, dessert tables, baby showers, birthdays and styled events — not just "balloons". Journal articles covering these topics build that map.

3. **Feed authority to service pages** — every cupcake article links to the baby shower balloon page, birthday balloon page, or contact page. The article acts as a funnel, not a destination.

4. **Image SEO** — images can rank in Google Images and Pinterest-style visual searches. File names and alt text matter. See naming convention and alt text guidelines below.

5. **Shareable content** — each article can be reused for Google Business Profile posts, Instagram captions, Pinterest pins, Facebook local groups and email.

**The important guardrail:** these articles must not make the site look like a cupcake bakery. The framing is always *inspiration and styling*, never *order from us*. The studio context block (see Series Positioning below) enforces this on every article.

**Alt text note:** Alt text must describe what is actually in the image. Do not inject balloon references into the alt text if the image does not show balloons. The internal links and page copy create the association — alt text is for accessibility and image indexing, not keyword stuffing.

**Image format note:** Current images are PNG. WebP would give better performance and should be considered for a future conversion pass, but is not urgent.

**Internal link loop:** From cupcake articles, link to balloon service pages. From balloon service pages, add a line like "Looking for dessert table inspiration? See our baby shower cupcake ideas." This creates a two-way content loop that reinforces topical relevance.

---

## Series Positioning

These articles are **dessert table inspiration**, not standalone baking tutorials. The framing is always:

> Little Moment Studio's focus is balloon styling and celebration setups. Cupcakes and cakes are part of the coordinated look. We do not make them ourselves, but we inspire the styling and can recommend a trusted local cake maker.

Every article should include:
1. A studio context paragraph near the top (balloon styling focus + cake maker referral offer)
2. Internal links to related cupcake articles and the baby shower / birthday balloon pages
3. A CTA that references the referral offer, not just balloon styling

---

## Layout Decision Guide

There are three article layouts. Choose based on the content structure — not the tag.

### Layout 1 — Hero + Design 1 & Design 2 badges
**Use when:** the article covers exactly two named designs, each with its own image, ingredients/materials list and step-by-step instructions.
**Signals:** article title includes "2 Easy Designs"; content has a clear Design 1 / Design 2 split; three images (hero + one per design).
**Tag:** Styling & Inspiration
**Examples:** baby-shower-cupcake-ideas.html, mermaid-cupcake-ideas.html, halloween-cupcake-ideas.html

### Layout 2 — Hero + inline images (no badges)
**Use when:** the article is a how-to guide or reference piece with process or reference images placed mid-article to illustrate specific sections. No two distinct named designs.
**Signals:** images support steps or show a variety of results; article covers a technique or range of options rather than two designs; can have 2–3 images.
**Tag:** DIY & Tutorial, or Styling & Inspiration when covering multiple themes
**Examples:** top-10-piping-tips-for-cupcakes.html, cling-film-method-multi-coloured-buttercream.html, match-cupcakes-with-balloon-display.html

### Layout 3 — Hero only
**Use when:** the article is text-led — Q&A, planning advice, trends, FAQ-style or general inspiration. No design-specific images needed mid-article.
**Signals:** content is primarily paragraphs, tables and lists; single hero image is sufficient; no step-by-step designs to illustrate.
**Tag:** Planning & Advice, Practical/FAQ, Trends
**Examples:** baby-shower-questions-answered.html, how-long-do-balloons-last.html, best-balloon-colours-2025.html

---

## Article Template Structure

1. **Intro** — what the article covers, who it is for, why these designs
2. **Studio context block** — balloon focus + cake maker referral (near top, after intro)
3. **Why These Designs** — comparison table (Style / Difficulty / Best For)
4. **Design 1** — badge divider → landscape image → What You Need table → How to Make (numbered steps) → Colour Ideas table → Tip box
5. **Design 2** — badge divider → landscape image → What You Need table → How to Make (numbered steps) → Colour Ideas table → Tip box
6. **Display & Styling** — how to present on a dessert table; coordinate with balloons
7. **Suggested Box** — mix of both designs
8. **Beginner Tips** — positive framing (not "mistakes to avoid")
9. **FAQ** — 4–6 Q&As; must match FAQPage schema
10. **Useful Tools** — bulleted kit list
11. **Closing paragraph** — summarise the two designs together
12. **Internal links block** — 2–3 "For more… see our guide to…" lines
13. **CTA block** — location-specific; include cake maker referral line

---

## Design Section Template (CSS)

```html
<!-- Badge divider -->
<div class="design-section-header reveal">
  <div class="design-section-line"></div>
  <div class="design-badge">Design 1</div>
  <div class="design-section-line"></div>
</div>

<!-- Full-width landscape image -->
<div class="design-img reveal">
  <img src="gallery/cupcakes/[filename].png" alt="[descriptive alt text]" loading="lazy">
</div>
```

Images are **full-width landscape** (1536×1024 or similar). Never side-by-side — too small on mobile.

---

## Image Naming Convention

```
gallery/cupcakes/[occasion]-cupcakes-kent.png          ← hero
gallery/cupcakes/[occasion]-[design1-name]-kent.png    ← Design 1
gallery/cupcakes/[occasion]-[design2-name]-kent.png    ← Design 2
```

Examples:
- `baby-shower-cupcakes-kent.png`
- `baby-shower-swirl-cupcakes-kent.png`
- `baby-shower-feet-cupcakes-kent.png`
- `halloween-cupcake-table-kent.png`
- `halloween-mummy-cupcakes-kent.png`
- `fourth-of-july-cupcakes-kent.png`

---

## Alt Text Guidelines

Alt text should describe the cupcakes, technique and occasion — not the brand. Include the piping tip or key technique where relevant.

Good examples:
- "Pastel baby shower dessert table with buttercream swirl cupcakes, baby feet topper cupcakes, balloons, flowers and soft neutral decorations"
- "Pastel buttercream swirl cupcakes for a baby shower decorated with pearl sprinkles using a Wilton 1M piping tip"
- "Baby shower cupcakes with pastel fondant circles, baby feet toppers and pearl decorations"
- "Halloween mummy cupcakes with ivory buttercream wrapped in white piping and edible candy eyes"

---

## Meta Title & Description Guidelines

- Meta title: under 60 characters. Pattern: `[Occasion] Cupcake Ideas: [short description]`
- Meta description: under 160 characters. Lead with the two designs + "step-by-step instructions" or "for a beautiful dessert table"

Published examples:
| Article | Meta Title (chars) | Meta Description (chars) |
|---|---|---|
| Baby shower | Baby Shower Cupcake Ideas: 2 Easy Designs for Beginners (55) | Easy baby shower cupcake ideas with pastel swirls and baby feet toppers for a beautiful dessert table. (101) |
| Halloween | Halloween Cupcake Ideas: 2 Easy Designs for Beginners (53) | Create easy Halloween cupcakes with two beginner-friendly designs: mummy cupcakes with edible eyes and orange swirl cupcakes with black bat toppers. (148) |
| 4th of July | 4th of July Cupcake Ideas \| Little Moment Studio (49) | Two beginner-friendly 4th of July cupcake designs — red, white and blue buttercream swirls and navy rosettes with white stars. Step-by-step instructions. (153) |

---

## Schema

Every article needs two JSON-LD blocks:
1. `BlogPosting` — headline, description, datePublished, dateModified, image, author, publisher
2. `FAQPage` — 4–6 questions matching the FAQ section

---

## Tag Colour

All cupcake articles use the **Styling & Inspiration** tag:
```html
<div class="article-tag" style="background: var(--secondary); color: #99556A;">Styling &amp; Inspiration</div>
```

---

## Orphan Page Strategy

Cupcake articles are built and committed **before the publish date** but are not added to `journal.html` or `sitemap.xml` until ready to go live. They are accessible by direct URL but not linked from anywhere on the site.

---

## Articles Built

| File | Layout | Publish Date | Status |
|---|---|---|---|
| `baby-shower-cupcake-ideas.html` | Design 1 & 2 | Apr 2026 | Live |
| `birthday-cupcake-ideas.html` | Design 1 & 2 | 25 Apr 2026 | Live |
| `mermaid-cupcake-ideas.html` | Design 1 & 2 | 27 Apr 2026 | Live |
| `easter-cupcake-ideas.html` | Design 1 & 2 | 20 Mar 2026 | Live |
| `fondant-cupcake-ideas-baby-shower-birthday.html` | Hero only | Apr 2026 | Live |
| `halloween-cupcake-ideas.html` | Design 1 & 2 | 1 Oct 2026 | Orphan — pushed to Vercel |
| `fourth-of-july-cupcake-ideas.html` | Design 1 & 2 | 20 Jun 2026 | Orphan — pushed to Vercel |
| `christmas-cupcake-ideas.html` | Design 1 & 2 | 10 Oct 2026 | Orphan — pushed to Vercel |
| `match-cupcakes-with-balloon-display.html` | Inline images | 8 Jun 2026 | Orphan — pushed to Vercel |
| `top-10-piping-tips-for-cupcakes.html` | Inline images | 8 May 2026 | Orphan — committed, not pushed |
| `cling-film-method-multi-coloured-buttercream.html` | Inline images | 20 May 2025 (backdated) | Orphan — committed, not pushed |

---

## Articles Planned (from Content Calendar)

| Article | Target Date | Notes |
|---|---|---|
| Mother's Day Cupcake Ideas | 22 Feb 2027 | Soft pinks, florals, pastel buttercream; publish 2 weeks before 14 Mar (UK Mothering Sunday) |
| St Patrick's Day Cupcake Ideas | 1 Mar 2027 | Green, shamrock, gold fondant; publish 2 weeks before 17 Mar |
| St George's Day Cupcake Ideas | 1 Apr 2027 | Red & white St George's Cross; publish 3 weeks before 23 Apr; England-specific |
| Gender Reveal Cupcakes | TBC | Pink, blue and neutral; pairs well with gender reveal article (Jun 2026) |
| Birthday Cupcakes | TBC | Natural extension of series |

---

## Content Plan Source

Original article plan provided April 2026 covering: article goal, image plan, full structure, design 1 and 2 instructions, display ideas, make-ahead/storage, transport tips, beginner mistakes, useful tools, internal links and future article ideas.

Key addition not in original plan: studio context block (balloon styling focus + cake maker referral) added during production — this is now a required element on every article in the series.
