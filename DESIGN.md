---
name: Flowdesk landing page
description: A calm, precise single-page SaaS landing template whose proof is a live product demo in the hero.
colors:
  ink: "#0b1220"
  ink-2: "#3d4757"
  ink-3: "#5f6979"
  line: "#e6e8ec"
  line-2: "#d5d9e0"
  paper: "#ffffff"
  paper-2: "#f6f7f9"
  accent: "#0b7a3d"
  accent-ink: "#0a6b35"
  accent-soft: "#e6f6ec"
  accent-bright: "#34d27b"
  tag-billing: "#fff1d6"
  tag-billing-ink: "#8a5a00"
  tag-bug: "#fde4e4"
  tag-bug-ink: "#a12a2a"
  tag-sales: "#e3ecff"
  tag-sales-ink: "#2347a8"
  tag-account: "#efe6ff"
  tag-account-ink: "#5b34a8"
  warn: "#a15c00"
  danger: "#b02a1f"
typography:
  display:
    fontFamily: "Geist, ui-sans-serif, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "clamp(2.6rem, 6.4vw, 4.75rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Geist, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(2rem, 4vw, 3rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Geist, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(1.5rem, 2.4vw, 2rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.03em"
  quote:
    fontFamily: "Geist, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(1.6rem, 3.2vw, 2.4rem)"
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Geist, ui-sans-serif, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Geist, ui-sans-serif, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 500
    lineHeight: 1
  data:
    fontFamily: "Geist Mono, ui-monospace, SFMono-Regular, Menlo, monospace"
    fontSize: "12px"
    fontWeight: 400
    fontFeature: "tnum"
rounded:
  tag: "5px"
  chip: "6px"
  control: "8px"
  panel: "10px"
  frame: "14px"
  band: "18px"
  pill: "99px"
spacing:
  gutter: "20px"
  sm: "10px"
  md: "18px"
  lg: "32px"
  xl: "64px"
  feature-gap: "96px"
  section: "128px"
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.paper}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 18px"
    height: "44px"
  button-primary-hover:
    backgroundColor: "{colors.accent-ink}"
  button-primary-on-ink:
    backgroundColor: "{colors.accent-bright}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 18px"
    height: "44px"
  input-email:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "44px"
  chip:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.chip}"
    padding: "0 10px"
    height: "28px"
  tag-billing:
    backgroundColor: "{colors.tag-billing}"
    textColor: "{colors.tag-billing-ink}"
    rounded: "{rounded.tag}"
    padding: "0 8px"
    height: "22px"
  badge:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.accent-ink}"
    rounded: "{rounded.tag}"
    padding: "3px 8px"
  panel:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.panel}"
    padding: "18px"
  cta-band:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.band}"
    padding: "clamp(40px, 7vw, 88px)"
---

# Design System: Flowdesk landing page

All tokens live as CSS custom properties in the `:root` block at the top of `public/index.html` (`--ink`, `--accent`, `--line`, `--radius`, and so on). Change them there and the whole page follows. Fonts are self-hosted variable WOFF2 files in `public/fonts/`.

## Overview

**Creative North Star: "The Working Product"**

The page is the category standard for a SaaS landing, executed with the restraint of the best product companies: a white daylight ground, near-black ink, one green, hairline borders and gently rounded rectangles. Its proof is not an illustration but the product itself: a live inbox in the hero where emails arrive, get tagged and get assigned while you watch. Everything else on the page borrows that product's interface vocabulary (chips, tags, panels, monospace counts) rather than marketing decoration.

Density is calm. Sections breathe on a 128px rhythm, copy is short and left-aligned, and each feature is shown by a small working vignette of the interface instead of an icon. Colour is almost entirely neutral; green means "this is the action" or "this got handled", and the tag pastels exist only to encode email categories.

The system rejects the stock gradient-SaaS look: no gradient blobs, no glass cards, no fake customer-logo walls, no grids of icon tiles.

**Key Characteristics:**
- White ground, ink text, one green accent with a clear job.
- 1px hairline borders do the structural work; shadows are soft and rare.
- Product UI as illustration: vignettes are built from the same chips, tags and panels as the demo.
- Geist for everything readable, Geist Mono for data (counts, times, rule values).
- Motion is short, eased and purposeful, and switched off under reduced motion.

## Colors

A neutral ink-on-white palette with a single deep green accent and four muted category pastels.

### Primary
- **Signal Green** (`accent`): the primary action (filled buttons), focus rings, checkmarks in feature and plan lists, the "on" switch, and the routing arrow in the log. Chosen deep enough to carry white button text at AA contrast.
- **Signal Green Deep** (`accent-ink`): hover state of the primary button and green text on white (success notes, the yearly discount, SLA met, badge text).
- **Mint Wash** (`accent-soft`): the faint highlight on a freshly routed email and the "Most popular" badge ground.
- **Live Green** (`accent-bright`): green on dark only: the primary button inside the ink CTA band, the live dot, the logo mark, and text selection. Never use it for text on white.

### Tertiary: category tags
- **Billing Amber**, **Bug Rose**, **Sales Blue**, **Account Lilac** (`tag-*` with matching `tag-*-ink` text): muted pastel grounds with dark same-hue text. They encode an email's category and appear only on tags.

### Neutral
- **Ink** (`ink`): headings, body text, the CTA band ground, workload bars, focused input border.
- **Slate** (`ink-2`): secondary copy, sub-headlines, nav links, list items.
- **Mist Slate** (`ink-3`): tertiary text: captions, timestamps, placeholders, footer.
- **Hairline** (`line`): every structural 1px border and divider.
- **Hairline Strong** (`line-2`): borders on interactive controls (inputs, ghost buttons, chips).
- **Paper** (`paper`) and **Paper Grey** (`paper-2`): page ground and the quiet secondary surface (demo toolbar, routing log, highlighted plan, toggle track).
- **Warn** / **Danger** (`warn`, `danger`): SLA countdown states and form error text only.

### Named Rules
**The One Green Rule.** Green appears only on the primary action and on things that were handled (routed, resolved, met, included). It is never decoration, never a section background, and the hero headline stays all ink.

**The Two Greens Rule.** `accent` on light grounds, `accent-bright` on the ink band. Swap them and either contrast or the glow breaks.

**The Pastels Mean Categories Rule.** Tag pastels are a data encoding, not a palette to decorate sections with.

## Typography

**Display Font:** Geist (with ui-sans-serif, system-ui fallback)
**Body Font:** Geist
**Label/Mono Font:** Geist Mono (with ui-monospace fallback)

**Character:** One neutral, precise grotesque at several weights, tightened at large sizes; its mono sibling marks anything that is data.

### Hierarchy
- **Display** (600, clamp 2.6rem to 4.75rem, 1.08, -0.04em): the hero headline only, max 15ch, balanced wrap.
- **Headline** (600, clamp 2rem to 3rem, 1.08, -0.03em): section headings; the CTA band uses a larger step (up to 3.4rem).
- **Title** (600, clamp 1.5rem to 2rem): feature headings; plan names drop to 20px.
- **Quote** (500, clamp 1.6rem to 2.4rem, 1.3): the single testimonial.
- **Body** (400, 17px, 1.6): running text; secondary paragraphs capped at 42 to 62ch. Section intros sit at 18px, hero sub up to 1.25rem.
- **Label** (500, 14 to 15px): buttons, nav, FAQ questions (17px).
- **Data** (Geist Mono, 11 to 13px, tabular numbers): counts, timestamps, rule values, SLA clocks, prices use tabular figures too.

### Named Rules
**The Mono Means Data Rule.** Geist Mono is reserved for machine values: numbers, times, rule keys and values. Never for headings or marketing copy.

**The Tight Headings Rule.** All headings are 600 weight with negative tracking (-0.03em, -0.04em at display size) and line-height 1.08.

## Layout

Single column of content in a centred container of 1160px with 20px side gutters (`min(1160px, 100% - 40px)`). The hero demo deliberately breaks out wider, up to 1320px, to read as the product rather than a card in the page. Everything is left-aligned except the demo caption.

Vertical rhythm: 128px between sections, 88px above the hero headline, 72px between section head and content, 96px between feature rows. Features are two-column rows (copy 1fr, vignette 1.15fr, 64px gap) that alternate sides and stack below 860px. Pricing is one bordered three-column block divided by hairlines (stacks below 900px). FAQ is a 1fr / 1.6fr split (stacks below 860px). The sticky nav is 64px tall and hides links below 760px. The demo drops its sidebar below 980px and becomes one column below 680px.

## Elevation & Depth

Depth comes from hairline borders and the white-versus-paper-grey tonal step first; shadows are soft, low-contrast and few.

### Shadow Vocabulary
- **Panel** (`box-shadow: 0 1px 2px rgb(11 18 32 / .06), 0 8px 24px -8px rgb(11 18 32 / .12)`): feature vignette panels and the selected billing toggle segment.
- **Demo Lift** (`box-shadow: 0 1px 2px rgb(11 18 32 / .05), 0 30px 60px -30px rgb(11 18 32 / .25)`): the hero demo frame only.
- **Input Focus Halo** (`box-shadow: 0 0 0 3px rgb(11 18 32 / .08)`): focused email field, with an ink border.

### Named Rules
**The Hairline First Rule.** Separate things with a 1px `line` border or a `paper-2` ground before reaching for a shadow. Pricing, FAQ, footer and sections are flat.

## Shapes

Gently rounded rectangles throughout, with radius growing with the size of the object: 5px tags and badges, 6px chips and sidebar items, 8px buttons, inputs and log entries, 10px panels and the billing toggle (`--radius`), 14px for the large framed objects (demo, pricing block), 18px for the dark CTA band. Avatars and the live dot are circles; switches and progress bars are full pills. Icons are inline SVG line checkmarks drawn with `currentColor`.

## Components

### Buttons
Quiet and solid; 44px tall, 8px corners, 500-weight 15px label.
- **Primary:** green fill, white label. Hover darkens to `accent-ink`. Inside the ink CTA band it becomes `accent-bright` with ink text (hover `#5be096`).
- **Ghost:** white fill, ink label, `line-2` border; hover darkens the border to `ink-3`. On the ink band: transparent with a `#3a4558` border.
- **Nav size:** 36px tall, 14px label.
- **States:** pressed nudges down 1px; disabled drops to 55% opacity. Transitions use 0.2s with the house ease.

### Chips and Tags
- **Chip:** 28px, white, `line-2` border, 6px corners; the value variant uses Geist Mono on `paper-2`. Used in the rule-builder vignette.
- **Tag:** 22px, 5px corners, pastel ground with same-hue ink text, 12px 500 weight. Pops in (scale 0.85 to 1) when an email is routed.
- **Badge:** mint ground with deep green text, used once for "Most popular".

### Cards / Containers
- **Panel:** white, 1px `line` border, 10px corners, Panel shadow, 18px padding. The vessel for every feature vignette.
- **Pricing block:** one 14px-rounded bordered frame split into plans by hairlines; the recommended plan sits on `paper-2`, not on a raised card.
- **CTA band:** ink ground, white headline, `#b9c1ce` supporting text, 18px corners.

### Inputs / Fields
- **Style:** 44px, white, `line-2` border, 8px corners, 15px text, `ink-3` placeholder.
- **Focus:** border turns ink plus a 3px faint ink halo.
- **Error:** red border and halo, message in `danger` below the field, announced via a status region.

### Navigation
Sticky, 64px, white at 78% with a light blur so content scrolls under it; a hairline bottom border appears once the page scrolls. Logo mark plus wordmark at left, 15px `ink-2` links that darken on hover, sign-in text link and a compact primary button at right. Links and sign-in hide below 760px.

### Live Inbox Demo (signature)
A framed three-column app view: folder sidebar, email list, routing log on `paper-2`. Every ~2.5s a new email slides in from above with a mint wash, then a category tag and an assignee chip pop in and a log entry records the rule that fired. Counts and times are in Geist Mono. All motion stops under `prefers-reduced-motion`. Section labels inside the app chrome (sidebar group, log title) are small uppercase app UI, not page-level labels.

### FAQ
Native `details`/`summary` rows divided by hairlines, 17px 500 questions, a drawn chevron that rotates on open.

## Do's and Don'ts

### Do:
- **Do** keep green for the primary action and handled states; use `accent` on light grounds and `accent-bright` only on ink.
- **Do** separate content with 1px `line` hairlines and the `paper-2` tonal step before adding shadows.
- **Do** show features with small vignettes built from the real interface parts (panels, chips, tags, mono data).
- **Do** set every number, time and rule value in Geist Mono with tabular figures.
- **Do** keep headings 600 weight, tightly tracked, left-aligned, in ink.
- **Do** keep motion to short eased arrivals (`cubic-bezier(.16, 1, .3, 1)`, 0.2 to 0.6s) and disable it under reduced motion.

### Don't:
- **Don't** use gradient blobs, glassmorphism cards, fake customer-logo walls or grids of icon tiles.
- **Don't** colour headline words green or use green as a section background.
- **Don't** use the tag pastels outside category tags.
- **Don't** add small uppercase labels above page headings; uppercase tracking belongs only to app chrome inside the demo.
- **Don't** use `accent-bright` for text or controls on white; it fails contrast.
