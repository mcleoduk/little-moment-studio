# Marketing Plan — Little Moment Studio

## Priority Checklist

### WhatsApp (do first — free, high ROI)
- [ ] Download WhatsApp Business app on Sam's phone
- [ ] Set up business profile (name, description, opening hours, website)
- [ ] Set up away message: "Thanks for your message! We'll get back to you within a few hours 💛"
- [ ] Add quick replies for common questions (pricing, availability, how to book)
- [ ] Add WhatsApp icon + link to website header (all pages)
- [ ] Add floating WhatsApp button to all pages
- [ ] After every job: send WhatsApp follow-up asking for a Google review

### Google Business Profile (do second — free, drives local search)
- [ ] Claim/create Google Business Profile for Little Moment Studio
- [ ] Add all details: address, phone, website, opening hours
- [ ] Add service categories: balloon styling, event decoration, baby shower
- [ ] Upload 10+ photos of best work
- [ ] Get first 5 Google reviews from existing clients
- [ ] Post regularly (weekly if possible — Google rewards activity)
- [ ] Add products/services with prices

### Google Search Console
- [ ] Verify littlemomentstudio.co.uk in Search Console
- [ ] Submit sitemap: https://littlemomentstudio.co.uk/sitemap.xml
- [ ] Monitor which pages are being indexed
- [ ] Check for crawl errors

### Instagram
- [ ] Post first Reel (balloon garland time-lapse — see UGC-CONTENT-PLAN.md)
- [ ] Post consistently — see UGC-CONTENT-PLAN.md for schedule
- [ ] Tag location (Sittingbourne, Kent) on every post
- [ ] Add website link in bio
- [ ] Engage with local wedding/baby/event accounts
- [ ] Restore Instagram links to site (see below)

#### Restoring Instagram links to the site
Links were removed from all pages (commit `5423b40`) because the account didn't exist yet. When ready, ask Claude to restore them site-wide. The two elements per page are:

**Gallery CTA button** (after the gallery grid on `index.html` and `gallery.html`):
```html
<div class="gallery-cta reveal">
  <a href="https://www.instagram.com/littlemomentstudio" class="btn btn-outline" target="_blank" rel="noopener">
    <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="2" width="20" height="20" rx="5"/><path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg>
    Follow us on Instagram @littlemomentstudio
  </a>
</div>
```

**Footer icon** (in `.footer-socials`, before the Facebook icon, on every page):
```html
<a href="https://www.instagram.com/littlemomentstudio" class="footer-social" aria-label="Instagram">
  <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="2" width="20" height="20" rx="5"/><path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg>
</a>
```

### Venue Partnerships
- [ ] Draft outreach email template for venues
- [ ] Contact venues featured on Maidstone page (BarnYard Lenham, Mercure Great Danes, Mu Mu, White Horse Bearsted)
- [ ] Contact venues on Sittingbourne venues article
- [ ] Offer to be listed as recommended supplier
- [ ] Follow up after 2 weeks if no response

### Client Referrals
- [ ] After every job: photograph finished setup + send to client via WhatsApp
- [ ] Include soft ask: "If you loved it, we'd really appreciate a Google review — it makes a huge difference for a small business"
- [ ] Consider a referral incentive (e.g. £20 off next booking if they refer a friend who books)

---

## WhatsApp Business Setup — Step by Step

**Number:** 07762 549 648

### Step 1 — Download the app
App Store (iPhone) or Google Play (Android) → search **WhatsApp Business** (briefcase icon, separate from regular WhatsApp).

### Step 2 — Verify your number
Enter 07762 549 648 → enter the 6-digit code sent by text.

### Step 3 — Create your profile
Tap ⋮ → **Settings** → **Business tools** → **Business profile**:
- **Name:** Little Moment Studio
- **Category:** Event Planner
- **Description (max 139 characters):** Balloon styling & celebration décor for baby showers, birthdays & events across Kent ✨ DM to book or get a quote
- **Address:** Forum Shopping Centre, Sittingbourne, ME10 3DL
- **Hours:** Mon–Sat 9:00am–5:30pm / Sun & Bank Hols 10:00am–4:00pm
- **Email:** hello@littlemomentstudio.co.uk
- **Website:** littlemomentstudio.co.uk

### Step 4 — Add profile photo
Settings → tap the circle at the top → upload logo → Save.

**Photo tip:** Use the logo on the cream (`#FAF7F2`) background — clean, recognisable, and on-brand. Avoid a busy photo at this small size; the logo reads much better.

### Step 5 — Set greeting message
Business tools → **Greeting message** → toggle on → edit:
> Hi! Thanks for reaching out to Little Moment Studio 🎈 To help us put together the perfect quote, could you let us know: your event date, type of celebration, and venue? We'll come back to you within 24 hours.

### Step 6 — Set away message
Business tools → **Away message** → toggle on → edit → set schedule to **Outside business hours**:
> Hi! Thanks for your message 💛 We're currently closed but will get back to you during opening hours. If you'd like to get started, visit littlemomentstudio.co.uk for ideas and inspiration.

### Step 7 — Quick replies
Business tools → **Quick replies** → tap **+** for each:
- `/quote` → standard pricing/quote response
- `/gallery` → link to littlemomentstudio.co.uk/gallery.html
- `/book` → booking enquiry message

### Step 8 — Catalogue (optional)
Business tools → **Catalogue** → add main service packages with photos and descriptions so clients can browse without asking.

---

### Why the greeting and away messages matter most

The greeting and away messages do the heavy lifting. They qualify enquiries automatically (date, event type, venue) and set response expectations without Sam needing to be online constantly. These two are the most important things to get right — set them up at the same time as the profile, not later.

---

## WhatsApp Business Notes

- **Number:** 07762 549 648 (WhatsApp Business — updated May 2026)
- **App:** WhatsApp Business (free, available on iOS/Android)
- **Future (GHL):** Plan to migrate to GoHighLevel for WhatsApp workflow automation — number carries straight across via Meta Business API, no website changes needed
  - GHL enables: automated follow-ups, CRM integration, booking workflows
  - Note: Meta now supports coexistence — you can run the WhatsApp Business app and the API (GHL) on the same number simultaneously

---

## Longer-Term Channels (when ready)

| Channel | Why | When |
|---------|-----|------|
| Pinterest | Drives evergreen traffic to journal articles | When 10+ articles live |
| Google Ads | Targeted local search ads | When budget allows, start with £5/day |
| Email newsletter | Retain past clients, seasonal promotions | When CRM/list in place |
| TikTok | Younger audience, high organic reach | When Reels established |

---

## Review & Referral Templates

### Post-job WhatsApp message
> "Hi [name]! So lovely to style your celebration — I hope you had the most wonderful day 💛 If you have a moment, a Google review would mean the world to us as a small local business. Here's the link: [Google review link]. Thank you so much! Sam x"

### Referral ask
> "If any of your friends are planning a baby shower or birthday celebration, we'd love to help them too. Mention Little Moment Studio and we'll take £20 off their first booking 🎈"
