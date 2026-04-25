# Cupcake Series — Article Reference

This document is the template and content reference for all cupcake tutorial articles on the Little Moment Studio journal. Use it when building new articles in the series.

---

## Series Positioning

These articles are **dessert table inspiration**, not standalone baking tutorials. The framing is always:

> Little Moment Studio's focus is balloon styling and celebration setups. Cupcakes and cakes are part of the coordinated look. We do not make them ourselves, but we inspire the styling and can recommend a trusted local cake maker.

Every article should include:
1. A studio context paragraph near the top (balloon styling focus + cake maker referral offer)
2. Internal links to related cupcake articles and the baby shower / birthday balloon pages
3. A CTA that references the referral offer, not just balloon styling

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

| File | Publish Date | Status |
|---|---|---|
| `baby-shower-cupcake-ideas.html` | TBC (Jul 2026 drafted) | Orphan |
| `halloween-cupcake-ideas.html` | 1 Oct 2026 | Orphan |
| `fourth-of-july-cupcake-ideas.html` | 20 Jun 2026 | Orphan |

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
