# KINGTOKENZ CAROUSEL AUTOMATION — Landing Page Spec

## 1. Concept & Vision

A high-converting, authority-driven landing page for a premium Instagram carousel automation service. The page should feel like you're stepping into a luxury marketing agency — bold, confident, and dripping with credibility. Think dark elegance meets warm gold accents: the kind of page that makes a business owner think "these guys know what they're doing." No generic SaaS vibes. This is premium positioning.

## 2. Design Language

### Aesthetic Direction
Dark luxury with warm gold accents — think high-end finance meets creative agency. Not flashy, but undeniably premium. Clean lines, bold typography, strategic use of space.

### Color Palette
- **Background Primary:** `#0a0a0a` (near-black)
- **Background Secondary:** `#141414` (dark charcoal)
- **Surface:** `#1f1f1f` (card backgrounds)
- **Gold Primary:** `#d4a853` (warm gold — main accent)
- **Gold Light:** `#e8c77b` (hover states, highlights)
- **Text Primary:** `#f5f5f5` (headings)
- **Text Secondary:** `#a0a0a0` (body copy)
- **Success Green:** `#4ade80` (checkmarks, positive metrics)

### Typography
- **Display / Hero:** "Playfair Display" (serif, 700) — authority, editorial weight
- **Headings:** "Playfair Display" (serif, 600)
- **Body / UI:** "Inter" (sans-serif, 400/500/600) — clean, modern, readable
- **Scale:** 16px base, 1.5 line-height body, tight tracking on display text

### Spatial System
- Section padding: 120px vertical (desktop), 80px (mobile)
- Container max-width: 1200px
- Card border-radius: 16px
- Consistent 8px spacing grid

### Motion Philosophy
- Subtle fade-in on scroll (opacity + slight translateY, 600ms ease-out)
- Gold accent elements pulse gently in hero
- Button hover: scale 1.02 + glow effect
- Stats counter animate on scroll into view

### Visual Assets
- Hero: Cinematic video (dark, abstract, high-energy) — muted autoplay
- Icons: Lucide or Feather icons (line style, 2px stroke)
- Decorative: Subtle gold gradient orbs, grain texture overlay

## 3. Layout & Structure

### Page Flow (Top to Bottom)
1. **Hero** — Full viewport, video background, massive headline, CTA
2. **The Numbers** — Dark section, 4-column stats grid
3. **How It Works** — 3-step horizontal timeline with icons
4. **What You Get** — Feature checklist with gold checkmarks
5. **Pricing** — 3-tier pricing cards, middle card highlighted as "Popular"
6. **Results Timeline** — 30/60/90 day milestones
7. **Social Proof** — Case study callout with metrics
8. **Final CTA** — Bold section, calendar booking CTA
9. **Footer** — Minimal, Instagram handle + email

### Responsive Strategy
- Desktop: Full layouts, horizontal grids
- Tablet: 2-column grids collapse gracefully
- Mobile: Single column, hero text scales down, pricing cards stack

## 4. Features & Interactions

### Hero
- Full-screen video background (muted, autoplay, loop)
- Large headline: "10 Authority Carousels. Every Single Day."
- Subheadline: value prop
- Primary CTA: "Book Your Free 15-Min Call" → gold button
- Scroll indicator animation at bottom

### Stats Section
- 4 key metrics in a row
- Numbers animate up when scrolled into view
- Gold accent underline on each stat

### How It Works
- 3 cards: Week 1 (Setup) / Weeks 2-4 (Execution) / Month 2+ (Authority)
- Each card has icon, title, bullet points
- Subtle connecting line between cards

### Features Grid
- 6 features with gold checkmark icons
- 2-column grid on desktop, 1 on mobile

### Pricing Cards
- 3 tiers: STARTER / PRO / PREMIUM
- PRO card: slightly elevated, gold border, "Most Popular" badge
- Each card: price, carousel count, feature list, CTA button
- Hover: subtle lift + shadow increase

### Results Timeline
- Vertical timeline with 30/60/90 day milestones
- Each milestone has metric + description
- Gold line connecting milestones

### Final CTA
- Dark section with gold gradient background accent
- Large headline + CTA button

### Footer
- Minimal: logo/text, Instagram handle, email

## 5. Component Inventory

### Buttons
- **Primary:** Gold background (#d4a853), dark text, rounded-full, hover: scale + glow
- **Secondary:** Transparent with gold border, gold text, hover: gold fill
- **Disabled:** Greyed out, no hover effect

### Cards
- Background: #1f1f1f, border-radius: 16px, subtle border: 1px solid #2a2a2a
- Hover: border-color shifts to gold, subtle shadow lift

### Pricing Card
- Same base as cards but PRO version has gold border
- "Most Popular" badge: small pill, gold background

### Checkmarks
- SVG checkmark icon in gold (#d4a853)
- Used in feature lists and pricing inclusions

### Stat Item
- Large number (Playfair, 48-64px)
- Label below in secondary text
- Gold underline accent

### Timeline Node
- Gold circle, white checkmark inside
- Connected by gold vertical line

## 6. Technical Approach

- **Stack:** Single HTML file with embedded CSS and minimal JS
- **Fonts:** Google Fonts (Playfair Display + Inter)
- **Icons:** Inline SVGs (no external icon library dependency)
- **Video:** MP4 hero video, muted autoplay loop, no poster image
- **Animations:** CSS transitions + Intersection Observer for scroll reveals
- **Responsive:** CSS Grid + Flexbox, media queries at 768px and 480px
- **Performance:** Inline critical CSS, lazy-load images below fold