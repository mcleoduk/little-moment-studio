# Celebration Styling Studio — Project Context

## About the Business
- **Name:** Little Moment Studio
- **Industry:** Premium balloon styling and celebration installations
- **Location:** Forum Shopping Centre, Sittingbourne, ME10 3DL, UK
- **Phone:** 07700 900 123
- **Email:** hello@littlemomentstudio.co.uk
- **Domain:** littlemomentstudio.co.uk
- **Speciality:** Luxury baby showers, first birthdays, children's celebration styling, balloon installations, backdrops, prop hire, helium balloons — local delivery and venue installation across Sittingbourne & Kent

## Project
Single-page website homepage (`index.html`).

**Tech stack:** Plain HTML + CSS + JS — no frameworks, no build tools. Opens directly in browser.

## Files
| File | Purpose |
|---|---|
| `index.html` | Main website — all HTML, CSS and JS in one file |
| `logo.png` | Brand logo |
| `hero.jpg` | Homepage hero image background |
| `gallery-1.jpg` | Signature setup / featured celebration image |
| `gallery-2.jpg` | Baby shower or first birthday installation image |
| `gallery-3.jpg` | Balloon garland / backdrop installation image |

## Brand Positioning
This is **not** a generic balloon shop website.

The brand should feel like a **premium celebration styling studio** specialising in:
- Baby showers
- First birthdays
- Children's celebrations
- Balloon garlands and luxury installations
- Prop hire and styled event setups

The site should communicate:
- premium
- soft
- elegant
- modern
- family-focused
- Instagram-worthy
- local and trusted

Avoid anything that feels:
- cheap
- loud
- party-shop style
- toy-shop style
- overly childish

## Design System
| Token | Value | Usage |
|---|---|---|
| `--bg` | `#FAF7F2` | Main background (warm ivory) |
| `--bg2` | `#F2F4F7` | Alternate light section background |
| `--bg3` | `#FFFFFF` | Cards / elevated panels |
| `--text` | `#4A4A4A` | Main body text |
| `--muted` | `#7A7A7A` | Secondary text |
| `--primary` | `#DCEAF5` | Powder blue |
| `--secondary` | `#F6DDE4` | Blush pink |
| `--accent` | `#D8C4A5` | Champagne gold accent |
| `--accent-lt` | `#E6D8C3` | Hover / lighter accent |
| `--sage` | `#DDE8DF` | Optional soft sage highlight |
| `--border` | `rgba(74, 74, 74, 0.10)` | Subtle borders |
| `--white` | `#FFFFFF` | White |
| `--shadow` | `0 2px 10px rgba(74,74,74,0.06), 0 12px 36px rgba(74,74,74,0.08)` | Layered soft shadow |

## Typography
**Headings:** `Playfair Display` (serif)  
**Body:** `Inter` (sans-serif)

### Typography Rules
- Use **Playfair Display** for all major headings and elegant emphasis
- Use **Inter** for body copy, buttons, navigation and supporting text
- Never use the same font for both headings and body
- Large headings should use slightly tighter tracking, around `-0.03em`
- Body text should have generous line-height, around `1.7`
- Keep type elegant, airy and premium

## Hero Section Copy
### Recommended Headline
**Luxury Baby & Children's Celebration Styling**

### Recommended Subheadline
**Beautiful balloon installations, baby showers and first birthdays in Sittingbourne & Kent.**

### Primary CTA
**Book Your Celebration**

### Secondary CTA
**View Our Work**

## Page Sections (in order)
1. **Top bar** — phone number + quick enquiry / book CTA
2. **Nav** — logo + key links + hamburger menu on mobile
3. **Hero** — full-width hero image with text overlay and two CTAs
4. **Service Overview** — Baby Showers / First Birthdays / Balloon Installations
5. **Signature Setup** — featured “Sky Celebration” or premium featured styling package
6. **Gallery** — real photography / styled installations
7. **Packages** — simple starting pricing / package guidance
8. **How It Works** — 3-step booking process
9. **Local Area Section** — Sittingbourne & Kent service area
10. **Testimonials** — trust-building customer reviews
11. **Contact / Booking Form** — enquiry form
12. **Footer** — logo, links, services, contact details, socials

## Signature Style Direction
The brand’s signature visual style should centre around:
- soft pastel balloon clouds
- hot-air balloon props
- teddy bears / cloud props where appropriate
- symmetrical, elegant setups
- airy curtain backdrops
- fresh floral styling
- premium, lightly styled dessert tables

## Recommended Colour Palettes for Content and Imagery
### 1. Pastel Sky
- Powder blue
- White
- Champagne accents

### 2. Soft Pastel Mix
- Powder blue
- Blush pink
- Ivory
- Champagne

### 3. Neutral Luxury
- Ivory
- Cream
- Beige
- Champagne

### Guidance
- Use **2–3 colours maximum** per setup
- Avoid bright rainbow palettes
- Avoid harsh, saturated primaries
- Everything should feel soft, premium and photograph beautifully

## Window Display / Visual Merchandising Context
The physical shop has approximately **2 metres of window space**.

The website visuals should align with rotating display themes such as:
- Baby shower styling
- First birthday styling
- Sky theme / balloon cloud installations
- Soft safari or teddy-bear themes

## Copy Style
- **See `TONE-GUIDE.md` for the full writing voice and content guidelines**
- British English spelling throughout
- Use “we” not “I” — future-proofs for team growth
- Elegant, soft and premium tone
- Clear and conversion-focused
- Family-friendly but never childish
- Position the business as a **celebration styling studio**, not a party shop
- Prefer “celebration styling”, “balloon installations”, “baby showers”, “first birthdays”, “styled setups”, “prop hire”
- Avoid overusing the word “balloons” in every line
- Avoid anything that sounds discount-led or low-end
- See `CONTENT-CALENDAR.md` for article scheduling and status

## Image Metadata
- **Whenever a new image is added to the gallery**, ask "Do you want to add/update the metadata for this image?" before proceeding. If yes, invoke the `image-metadata` skill and ask the three questions (subject, date, camera).

## Design Guardrails
- **Invoke the `frontend-design` skill** before writing any frontend code, every session, no exceptions.
- The website should feel premium, airy and feminine-neutral
- Use only the design system colours above unless explicitly asked otherwise
- Shadows must be soft, layered and subtle
- Use warm, elegant gradients and very light overlays where needed
- Only animate `transform` and `opacity`
- Never use `transition-all`
- Every clickable element must have hover, focus-visible, and active states
- Hero image should include a subtle overlay to support text readability
- Maintain strong whitespace and breathing room
- Layout should feel editorial and boutique, not dense

## Hero Image Guidance
The hero image should be:
- landscape 16:9 or suitable for a 1920px-wide desktop hero
- softly lit
- slightly pastel, not oversaturated
- symmetrical or balanced
- have enough negative space for text overlay
- premium and realistic
- focused on baby shower / first birthday styling

Preferred image content:
- pastel balloon clouds
- fabric hot-air balloons
- dessert table
- teddy bears or cloud props
- soft florals
- white curtain backdrop
- champagne or ivory detailing

## Buttons
Primary buttons should use:
- Background: `#D8C4A5`
- Text: `#FFFFFF`

Secondary buttons should use:
- White or ivory background
- Soft charcoal text
- Subtle border

Buttons should feel soft, elegant and premium — never loud or overly rounded.

## SEO / Location Notes
This business serves:
- Sittingbourne
- Kent
- nearby towns and venues

Key service themes:
- baby shower balloons Sittingbourne
- first birthday balloons Sittingbourne
- celebration styling Sittingbourne
- balloon garland Sittingbourne
- baby shower decorations Kent

## Hard Rules
- Do not make the site look like a generic party shop
- Do not introduce bright rainbow colours unless explicitly asked
- Do not use childish graphics or cartoon-heavy styling
- Do not use dark backgrounds unless explicitly requested
- Do not use American spelling
- Do not use `transition-all`
- Do not add sections or content that were not requested
- Keep the positioning premium and specialist
