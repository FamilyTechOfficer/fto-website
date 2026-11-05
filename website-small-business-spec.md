# Website Spec: Home & Small Business Update

**For:** FTO developer
**Owner:** Kevin
**Goal:** Reposition familytechnicalofficer.com from home-only to **Home & Small Business Technology**. Two parts:

- **Part A:** Homepage updates, so visitors immediately see that FTO serves both homes and businesses
- **Part B:** A new `/small-business` page that sells the secure small-business network service

Companion files:
- `FTO-Secure-Business-Network.pdf` — the printed one-pager, for reference only (not posted on the site)
- `secure-business-network.html` — source for the PDF. Reuse its colors, copy, and the before/after diagram markup.

**Ground rule:** keep the existing homepage sections, founder story, and residential content. This update adds the business side and adjusts the framing. It is not a redesign.

---

# Part A: Homepage

## A1. Site-wide positioning

| Item | Value |
|---|---|
| Positioning line (under logo or in header) | Home & Small Business Technology |
| Homepage `<title>` | Family Technical Officer · Home & Small Business Technology · Coeur d'Alene, Post Falls, Spokane |
| Homepage meta description | Networks, Wi-Fi, security, and smart home for homes and small businesses in North Idaho and Spokane. No markup on equipment, no monthly contracts, and you own everything. |
| Footer tagline | Home & Small Business Technology · Same person, every time. |

## A2. Navigation

Top-level nav, in this order:

**Home · Home Services · Small Business · About · Contact**

- "Home Services" points to the existing residential services page or section. Rename the current label if it says just "Services."
- "Small Business" points to the new `/small-business` page (Part B).
- On mobile, keep both service items visible in the menu, not nested.

## A3. Hero (replace current hero copy)

- **H1:** Technology done right, for your home and your business.
- **Subhead:** Networks, Wi-Fi, security, and smart home, designed and installed by one person. No markup. No monthly contracts. You own it.
- **Two buttons, equal weight:**
  - "For your home" → existing home services page or section
  - "For your business" → `/small-business`

If the current hero has a photo, keep it. If it's clearly residential-only (a living room, a kitchen), add a second image or swap to something neutral like an equipment shot or Kevin on site.

## A4. New section: "Two ways we help"

Place directly under the hero. Two cards side by side on desktop, stacked on mobile. Each card links to its page.

| | **For your home** | **For your business** |
|---|---|---|
| Who | Homeowners, custom builders, vacation rental owners | Offices, practices, studios, shops, and building owners |
| What | Whole-home Wi-Fi and networking · Smart home and lighting (Lutron, Home Assistant) · Audio and video · Cameras and doorbells | Secure, separated networks · Guest Wi-Fi kept off your computers · Office Wi-Fi · Cameras · Networks for shared buildings |
| Line at bottom | Built for how your family lives. | Business-grade security without the IT contract. |
| Button | See home services | See business services |

## A5. New or updated section: "Why FTO"

One strip of five short points that apply to both audiences. If the homepage already has a "why us" section, update it to this wording rather than adding a second one.

1. **No markup on equipment.** You pay what I pay.
2. **You own everything.** Equipment, passwords, and settings are yours.
3. **No monthly contracts.** Built right once, not rented.
4. **Engineering first.** 25 years of software quality engineering behind every design.
5. **Same person, every time.** You call me, not a call center.

## A6. Contact form (site-wide)

Add one field at the top: **"Is this for your home or your business?"** (Home · Business). If Business, show the extra fields from Part B, section 2.8.

## A7. Leave as-is

- Founder story / About content
- Existing residential service details, project photos, and builder content
- Contact details and service area

---

# Part B: Small Business page

## 1. Page setup

| Item | Value |
|---|---|
| URL | `/small-business` |
| Nav label | Small Business |
| Page title (`<title>`) | Secure Small Business Networks · Family Technical Officer |
| Meta description | Business-grade network security for small offices in Coeur d'Alene, Post Falls, and Spokane. Built once, no monthly contract, and you own it. |
| CTA | Call 208.640.2341 or email webcontact@familytechnicalofficer.com |

Nav placement: a top-level item next to the existing residential services, so business visitors don't have to dig through homeowner content.

---

## 2. Sections (top to bottom)

Copy below is final unless Kevin changes it. Keep it plain. The audience is not technical.

### 2.1 Hero
- **H1:** A Secure Network for Your Small Business
- **Subhead:** Built right once. Yours to keep. No monthly contract.
- **Body:** Your network carries your customer records, your payments, and your passwords. Most small businesses end up with one of two options, and neither one is a great fit. There's a better middle ground.
- **Button:** "Set up a walkthrough" (scrolls to contact section)

### 2.2 Your three options
Three cards side by side on desktop, stacked on mobile. The third card is visually highlighted (gold border, matching the PDF).

| Card | Short description | Points (✓ = green, ✕ = red) | Verdict line |
|---|---|---|---|
| **The shared router** | The box from your internet provider. Staff, guests, and devices all on one network. | ✓ Already installed · ✕ Often a monthly rental fee · ✕ Guests on the same network as your computers · ✕ One virus can spread to every device | Convenient, but wide open. |
| **The IT contract** | A managed IT company with a monthly fee, often locked in for years. | ✓ Secure setup · ✕ You pay every month, forever · ✕ They often hold the passwords · ✕ Hard to leave if you're unhappy | Secure, but you rent it. |
| **The FTO way** | A business-grade network, designed and installed once, then handed to you. | ✓ Staff, guests, and devices kept apart · ✓ No monthly fees to us, no contract · ✓ You own the equipment and passwords · ✓ Same person to call, every time | Secure, and it's yours. |

### 2.3 Before / after diagram
The key visual. Build it in HTML/CSS or inline SVG (not an image), so it stays sharp and stacks on mobile.

- **Left, "Today: one shared network":** a red dashed box with pill labels: Office computers, Guest phones, Card reader, Cameras, Printer, Tenant laptop, Smart TV. Caption (red): *Every device can see every other device.*
- **Arrow** (gold). Points down on mobile.
- **Right, "After: separate networks":** a "Business-grade firewall" bar on top, then four colored boxes: **Staff** (computers, printer) · **Guests** (Wi-Fi only) · **Devices** (card reader, cameras) · **Tenants** (each on their own). Caption (green): *Each network reaches the internet, not each other.*

Markup and colors are in `secure-business-network.html` (`.ba` section).

### 2.4 What you get
Six items in a 2×3 or 3×2 grid on desktop, one column on mobile. Bold title plus one line.

1. **Separate networks:** Staff, guests, payments, and cameras each walled off.
2. **Guest Wi-Fi that can't see your computers:** Customers get internet. Nothing else.
3. **Strong, reliable Wi-Fi:** Business-grade equipment, placed where you need it.
4. **A map of your network:** A simple diagram and equipment list for your records.
5. **Locked-down admin access:** No default passwords. You hold the keys.
6. **Equipment at cost:** No markup on hardware. No licenses or monthly fees.

### 2.5 Who it's for
Short intro, then a row of simple tiles or icons:

> Offices, practices, studios, and shops with a handful of staff, customers on the Wi-Fi, and information worth protecting.

Tiles:
- **Health and wellness practices** (chiropractic, massage, counseling, PT, dental)
- **Professional offices** (accountants, attorneys, insurance, real estate)
- **Salons, studios, and shops** (guest Wi-Fi plus card readers)
- **Building owners** (shared internet, separate network for each tenant)

Callout box under the tiles (blue left border, as in the PDF):

> **Health and wellness practices:** each practice runs on its own private network, and you get a network map and equipment list to support your patient-privacy obligations.

### 2.6 How it works
Four numbered steps in a horizontal row on desktop, vertical on mobile.

1. **Walkthrough.** I look at your space and what you use today.
2. **Clear proposal.** Equipment and pricing, up front.
3. **Install and setup.** Usually uses the wiring you already have.
4. **Handoff.** Your map, your passwords, your equipment.

### 2.7 Case study (placeholder, fill after first install)
Leave this section built but hidden until Kevin supplies content.

- Title: "Real example: a shared office building"
- Before/after summary (3–4 sentences), 1–2 photos, a short quote from the building owner
- Kevin will provide copy, photos, and the owner's approval to publish. **Do not publish without written approval from the owner.**

### 2.8 Contact / CTA
Dark band, matching the PDF footer CTA.

- **Headline:** Not sure what you have today? Let's take a look.
- **Body:** Call or email to set up a walkthrough.
- Phone (tap-to-call on mobile): 208.640.2341
- Email: webcontact@familytechnicalofficer.com
- If the site already has a contact form, reuse it here. Add a "Business name" field and a dropdown: *Type of business* (Health/wellness · Professional office · Retail/salon/studio · Building owner · Other).

---

## 3. Design

Match the existing FTO proposal style (see the PDF).

| Token | Hex | Use |
|---|---|---|
| Cream (background) | `#F5F0E8` | Page background |
| Card | `#FBF8F2` | Card backgrounds |
| Gold | `#9A7B2F` | Brand name, section labels, highlights |
| Ink | `#1F1F1F` | Body text, CTA band |
| Gray | `#555555` | Secondary text |
| Blue | `#1F5FA8` | Links, step numbers, health callout |
| Green | `#3E7B4B` | ✓ marks, "good" captions, Guests box |
| Red | `#A33A2B` | ✕ marks, "bad" captions |
| Navy / Rust / Purple | `#2C5B8C` / `#B0552E` / `#6A4F98` | Diagram network boxes |

- **Font:** Helvetica / Arial (system sans). Bold for headings.
- **Section labels:** small, uppercase, gold, with a thin gold underline.
- **Mobile:** everything stacks to one column. Diagram arrow points down. No horizontal scroll at 360px wide.
- **Footer line:** "Same person, every time."

---

## 4. Copy rules (important)

These are business and liability rules. Please don't edit around them.

- **Never** say "HIPAA compliant," "HIPAA certified," "guaranteed secure," or "hack-proof." Use the wording above ("support your patient-privacy obligations").
- Don't use "IT services," "managed services," or "MSP" for FTO. The point is that FTO is *not* a monthly IT contract.
- Don't name competitor companies.
- Don't publish hourly rates or prices on this page. Pricing is quoted after the walkthrough.
- Keep the language plain. If a sentence needs a networking term to make sense, rewrite it.

---

## 5. SEO

- H1 once (hero). H2 for each section.
- Target phrases (use naturally, don't stuff): *small business network setup Coeur d'Alene*, *secure office Wi-Fi Post Falls*, *business network Spokane*, *guest Wi-Fi for small business*.
- Add `LocalBusiness` schema if the site doesn't already have it (name, phone, service area: Coeur d'Alene, Post Falls, Spokane).
- Alt text on any images. The diagram should have a text equivalent (screen-reader summary: "Before: all devices on one shared network. After: staff, guests, devices, and tenants on separate networks behind a firewall.").

---

## 6. Deliverables checklist

**Homepage (Part A)**
- [ ] Positioning line, homepage title, meta description, and footer tagline updated
- [ ] Nav reordered with Home Services and Small Business
- [ ] Hero copy and two buttons updated
- [ ] "Two ways we help" section added
- [ ] "Why FTO" strip added or updated
- [ ] Contact form home/business field added

**Small Business page (Part B)**
- [ ] `/small-business` page live with sections 2.1–2.6 and 2.8
- [ ] Section 2.7 built and hidden
- [ ] Nav link added
- [ ] Contact form updated with business fields
- [ ] Mobile check at 360px and 768px
- [ ] Kevin reviews copy before publish
