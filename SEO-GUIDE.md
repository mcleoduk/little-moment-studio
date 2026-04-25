# SEO Guide — Little Moment Studio

Technical SEO rules and limits for every page and article on the site.

---

## Meta Title

- **Limit: ~60 characters** (Google truncates beyond this in search results)
- The meta title (`<title>`) and the H1 on the page can differ — and often should
- Meta title is for search result click-through; H1 is for the reader once they arrive
- Pattern for articles: `[Topic]: [Short Description] | Little Moment Studio`
- Pattern for service pages: `[Service] [Location] | Little Moment Studio`
- Do not stuff keywords — write for the searcher, not the algorithm

**Published examples:**
| Page | Meta Title | Chars |
|---|---|---|
| Baby shower cupcakes | Baby Shower Cupcake Ideas: 2 Easy Designs for Beginners | 55 |
| Halloween cupcakes | Halloween Cupcake Ideas: 2 Easy Designs for Beginners | 53 |
| 4th of July cupcakes | 4th of July Cupcake Ideas \| Little Moment Studio | 49 |

---

## Meta Description

- **Limit: ~160 characters** (Google truncates beyond this)
- Should summarise the page value clearly and invite the click
- Does not directly affect ranking — affects click-through rate
- Lead with the most specific, useful detail first
- Do not end with a filler sentence if it pushes past 160 chars — cut it

**Published examples:**
| Page | Meta Description | Chars |
|---|---|---|
| Baby shower cupcakes | Easy baby shower cupcake ideas with pastel swirls and baby feet toppers for a beautiful dessert table. | 101 |
| Halloween cupcakes | Create easy Halloween cupcakes with two beginner-friendly designs: mummy cupcakes with edible eyes and orange swirl cupcakes with black bat toppers. | 148 |
| 4th of July cupcakes | Two beginner-friendly 4th of July cupcake designs — red, white and blue buttercream swirls and navy rosettes with white stars. Step-by-step instructions. | 153 |

---

## OG / Social Tags

- `og:title` — can match meta title or be slightly expanded (social has more room)
- `og:description` — can be more descriptive than the meta description; 2–3 sentences is fine
- `og:image` — always set to the hero image with full absolute URL
- `twitter:card` — always `summary_large_image`

---

## H1

- One H1 per page, always
- Can be longer and more descriptive than the meta title
- Use Playfair Display italic (`<em>`) on the emotional word for visual accent
- Example: `Baby Shower Cupcake Ideas: 2 Easy Designs for a <em>Beautiful Dessert Table</em>`

---

## Schema (JSON-LD)

Every article needs at minimum:

**BlogPosting** — on every journal article:
```json
{
  "@type": "BlogPosting",
  "headline": "...",
  "description": "...",
  "datePublished": "YYYY-MM-DD",
  "dateModified": "YYYY-MM-DD",
  "author": { "@type": "Organization", "name": "Little Moment Studio" },
  "publisher": { "@type": "Organization", "name": "Little Moment Studio" },
  "mainEntityOfPage": "https://littlemomentstudio.co.uk/[filename]",
  "image": "https://littlemomentstudio.co.uk/gallery/[hero-image].png"
}
```

**FAQPage** — on every article with a FAQ section (which should be all of them):
```json
{
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Question text",
      "acceptedAnswer": { "@type": "Answer", "text": "Answer text" }
    }
  ]
}
```

**Service** — on service pages (baby-shower-balloons-kent.html etc.):
- Includes provider, areaServed, address

---

## Sitemap Priorities

```xml
1.0  — homepage (index.html)
0.9  — gallery.html
0.8  — main service pages (baby-shower-balloons-kent.html, birthday-balloons-kent.html, balloon-garlands-kent.html)
0.7  — location pages (Maidstone, Faversham etc.), faqs.html, journal.html
0.6  — journal articles
```

`lastmod` should reflect the actual publish or last-edited date.

---

## Canonical Tags

Every page has a canonical tag pointing to its own full URL:
```html
<link rel="canonical" href="https://littlemomentstudio.co.uk/[filename].html">
```

---

## Orphan Page Strategy

Articles are built and committed before the publish date but are **not added to journal.html or sitemap.xml** until ready to go live. They are accessible by direct URL but not linked from anywhere on the site. This means:
- The page can be reviewed and checked before publication
- Google will not find or index it (no sitemap entry, no inbound links)
- To publish: add journal card, sitemap entry, update content calendar, update schema dates

---

## Image SEO

### File naming
- All lowercase, hyphen-separated
- Descriptive of what is actually in the image
- Pattern: `[subject]-[detail]-kent.png` or `[subject]-[detail].png` depending on type

**Use `-kent`:**
- Balloon displays, garlands and setups
- Service and location page images
- Styling/table scenes where balloons are visible

**Omit `-kent`:**
- Pure cupcake design close-ups (Design 1, Design 2 shots) — the subject is not location-specific
- General decorating technique images

Examples: `baby-shower-swirl-cupcakes-kent.png` (balloon display context), `christmas-tree-cupcakes.png` (pure cupcake design)

### Alt text
- Describes what is **actually in the image** — not what we want to rank for
- Do not inject balloon references if the image does not show balloons
- Include technique or key detail where relevant (piping tip, fondant type)
- Examples:
  - "Pastel buttercream swirl cupcakes for a baby shower decorated with pearl sprinkles using a Wilton 1M piping tip"
  - "Baby shower cupcakes with pastel fondant circles, baby feet toppers and pearl decorations"
  - "Halloween mummy cupcakes with ivory buttercream wrapping and edible candy eyes"

### Format
- Current: PNG
- WebP would give better performance — worth a conversion pass in future but not urgent

---

## Internal Linking

- Every article links to **at least 2 other pages**
- Always include a link to the relevant **service page** (baby-shower-balloons-kent.html etc.)
- Add a **reverse link** from the service page back to the article (creates a two-way content loop)
- Reverse link placement on service pages: between the FAQ section and the CTA strip
- Link text should be natural, not "click here" or keyword-stuffed

---

## Article Tag Colours (for journal cards and article headers)

| Tag | Background | Text colour |
|---|---|---|
| Styling & Inspiration | `var(--secondary)` (#F6DDE4) | `#99556A` |
| Planning & Advice | `var(--primary)` (#DCEAF5) | `#5A7A99` |
| Practical / FAQ | `var(--primary)` (#DCEAF5) | `#5A7A99` |
| Seasonal | `#E8F0E0` | `#5A7A5A` |
| Trends | `var(--primary)` (#DCEAF5) | `#5A7A99` |

---

## Backdating Published Articles

Backdating is acceptable for content that was genuinely written and ready — it is standard practice. Rules:
- The backdated date should be plausible in the chronological sequence
- It should not predate an article that links to it (i.e. if Article A links to Article B, Article A cannot be dated earlier than Article B unless the link was added later)
- Update `datePublished` and `dateModified` in the JSON-LD schema
- Update the visible date in the article meta (`<span>Month YYYY</span>`)
- Update the journal card date in journal.html
- Update `lastmod` in sitemap.xml
- Update the content calendar

---

## Robots

All public pages use:
```html
<meta name="robots" content="index, follow">
```

Orphan pages that should not be indexed yet can use `noindex` temporarily, though the current strategy is simply to exclude them from the sitemap and avoid inbound links.
