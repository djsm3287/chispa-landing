---
name: Chispa
description: Late-night Venezuelan street-food menu, ordered by WhatsApp.
colors:
  brasa: "#ff5a1f"
  brasa-viva: "#ff6a33"
  maiz: "#ffc41f"
  cilantro: "#2fbf71"
  asfalto: "#14110f"
  carbon: "#1f1a17"
  plancha: "#2a2420"
  hollin: "#3a322c"
  masa: "#f7efe3"
  humo: "#b5a898"
  tinta: "#1c1612"
typography:
  display:
    fontFamily: "Bowlby One, Arial Black, Impact, sans-serif"
    fontSize: "clamp(3.25rem, 7vw, 5.5rem)"
    fontWeight: 400
    lineHeight: 0.96
  headline:
    fontFamily: "Bowlby One, Arial Black, Impact, sans-serif"
    fontSize: "clamp(1.6rem, 5vw, 2.6rem)"
    fontWeight: 400
    lineHeight: 1.1
  title:
    fontFamily: "Bowlby One, Arial Black, Impact, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 400
    lineHeight: 1.15
  figure:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "1.75rem"
    fontWeight: 700
    lineHeight: 1.15
    fontFeature: "\"tnum\""
  marker:
    fontFamily: "Permanent Marker, cursive"
    fontSize: "1.125rem"
    fontWeight: 400
    lineHeight: 1.2
  lead:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "1.125rem"
    fontWeight: 600
    lineHeight: 1.25
  body:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.5
  meta:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
    lineHeight: 1.4
  micro:
    fontFamily: "Rubik, system-ui, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.06em"
rounded:
  s: "8px"
  m: "16px"
  l: "24px"
  pill: "999px"
spacing:
  "1": "4px"
  "2": "8px"
  "3": "12px"
  "4": "16px"
  "6": "24px"
  gutter: "clamp(16px, 3vw, 40px)"
components:
  button-primary:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    typography: "{typography.lead}"
    rounded: "{rounded.pill}"
    height: "56px"
  button-add:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.pill}"
    size: "44px"
  button-dark:
    backgroundColor: "{colors.tinta}"
    textColor: "{colors.masa}"
    rounded: "{rounded.pill}"
    height: "48px"
    padding: "0 20px"
  icon-button:
    backgroundColor: "{colors.plancha}"
    textColor: "{colors.masa}"
    rounded: "{rounded.pill}"
    size: "44px"
  chip:
    textColor: "{colors.masa}"
    typography: "{typography.micro}"
    rounded: "{rounded.m}"
    height: "72px"
  chip-active:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.m}"
  card:
    backgroundColor: "{colors.carbon}"
    rounded: "{rounded.m}"
  input:
    backgroundColor: "{colors.carbon}"
    textColor: "{colors.masa}"
    rounded: "{rounded.m}"
    height: "48px"
    padding: "12px 16px"
  input-search:
    backgroundColor: "{colors.plancha}"
    rounded: "{rounded.pill}"
    height: "48px"
  sticker:
    backgroundColor: "{colors.maiz}"
    textColor: "{colors.tinta}"
    typography: "{typography.micro}"
    rounded: "{rounded.s}"
    padding: "4px 8px"
  segmented-active:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.pill}"
    height: "44px"
  orderbar:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.pill}"
    height: "56px"
  sheet:
    backgroundColor: "{colors.plancha}"
    rounded: "{rounded.l}"
  promo-tile:
    backgroundColor: "{colors.brasa}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.l}"
---

# Design System: Chispa

## Overview

**Creative North Star: "Neon Street Counter"**

Chispa looks like a street-food counter at night: a dark, warm street lit by loud signage, specials scrawled by hand, and food under warm light. The page is a near-black warm asphalt (Asfalto) with a fine 4% film grain. Two hot accents do all the shouting. Brasa orange is the "act now" color, and Maíz yellow is the hand-lettered aside. They meet in the striped awning (toldo) with scalloped trim that runs across the fixed header and doubles as a scroll-progress bar.

The signage register (Bowlby One headlines, Permanent Marker scribbles tilted −3°, rotated stickers with hard black offset shadows, a scrolling marquee of specials) is loud on purpose. Components are **tactile but tidy**. They press in, pop, and spring on touch, but at rest they are calm, bordered, dark surfaces that let food photos and prices lead. Density is a phone menu's: two cards per row on mobile, one scrolling row per category on desktop, and every control at least 44px for a thumb.

**Key Characteristics:**
- Dark, warm, single-theme ("Noche") interface; no light mode.
- Two accents only: Brasa for action and price, Maíz for marker text, stickers, and focus.
- Striped-awning motif (24px stripes, 12px scallops) as the signature ornament.
- Signage type for headings, a marker hand for asides, Rubik for everything that must be read.
- Physical feedback (press-scale, spring pops, fly-to-cart, pointer tilt) that turns off under reduced motion.

## Colors

A warm charcoal ground with two hot accents taken from the grill and the arepa.

### Primary
- **Brasa** (`brasa`): ember orange. Fills every primary action: the add button, the full-width CTA, the floating order bar, the active rail chip, the selected segment, the promo tile, and the cart count badge. It also forms half of the toldo stripes.
- **Brasa Viva** (`brasa-viva`): a slightly lighter orange for orange *text* on dark surfaces (prices, links, the spicy tag), where plain Brasa is too dim.

### Secondary
- **Maíz** (`maiz`): corn yellow. Used for the hand-lettered marker lines, stickers ("Más pedido", "Nueva"), the marquee stars, the wavy section ornaments, the focus ring, text selection, and field error text and borders. It is the other half of the awning.

### Tertiary
- **Cilantro** (`cilantro`): green, used only for the vegetarian tag. It is a meaning color, never decoration.

### Neutral
- **Asfalto** (`asfalto`): the page ground and `theme-color`.
- **Carbón** (`carbon`): the first raised surface, for cards, rows, combos, the marquee band, and form fields.
- **Plancha** (`plancha`): the second raised surface, for sheets, the search field, icon buttons, and empty photo slots.
- **Hollín** (`hollin`): every 1px border and divider, plus the sheet grabber.
- **Masa** (`masa`): warm cream primary text.
- **Humo** (`humo`): muted text for descriptions, counts, labels, placeholders, and the footer.
- **Tinta** (`tinta`): near-black ink used *on* Brasa and Maíz fills, and as the dark pill inside orange surfaces.

### Named Rules
**The Two-Flame Rule.** Brasa and Maíz are the only accents. Brasa means "do this or pay this"; Maíz means "a note from the cook". Don't swap their jobs, and don't add a third accent.

**The Ink-on-Fire Rule.** Text on a Brasa or Maíz fill is always Tinta, never white or cream.

## Typography

**Display Font:** Bowlby One (fallback: metric-adjusted Arial Black, then Impact)
**Body Font:** Rubik 400–700 (fallback: metric-adjusted Arial, then system-ui)
**Marker Font:** Permanent Marker (fallback: Comic Sans MS, cursive)

**Character:** Bowlby One is the painted sign over the counter; Permanent Marker is the cook's scrawl on the whiteboard; Rubik is the friendly, legible menu text underneath. Sizes are set in rem by role, so the type respects the user's font size.

### Hierarchy
- **Display** (Bowlby One 400, clamp 3.25–5.5rem, line-height 0.96, uppercase): the promo tile headline ("2×1 en perros") only.
- **Headline** (Bowlby One 400, clamp 1.6–2.6rem, 1.1): section titles, which reveal by sliding up inside an overflow mask.
- **Title** (Bowlby One 400, 1.5rem, 1.875rem on desktop): combo names. Sheet titles use the same face at the figure size (1.75rem).
- **Figure** (Rubik 700, 1.75rem, tabular): totals and combo prices.
- **Marker** (Permanent Marker, 1.125rem, 1.25rem on desktop, rotated −3°, Maíz): section asides like "¡recién salidas!" and "¡solo los jueves!".
- **Lead** (Rubik 600–700, 1.125rem): item names, card prices, the main CTA.
- **Body** (Rubik 400, 1rem, 1.5): full descriptions in sheets and general text.
- **Meta** (Rubik 400, 0.875rem, 1.5): card descriptions (clamped to 2 lines), counts, footer, and the marquee (Bowlby uppercase, tracking 0.04em).
- **Label** (Rubik 600, 0.8125rem): field labels, line notes, errors.
- **Micro** (Rubik 700, 0.75rem, uppercase, tracking 0.06em on stickers): stickers, count badge, mobile rail chips.

### Named Rules
**The Sign-Painter Rule.** Bowlby One is only for headings, combo names, the marquee, and the promo. It is never used for prices, item names, or anything a customer must read in a sentence.

**The Tabular Price Rule.** Every price, count, and total uses tabular figures so numbers don't jitter as they animate.

## Layout

A single centered column (max 1280px) with a fluid gutter (clamp 16–40px). A fixed header stack sits on top: a translucent topbar (82% Asfalto, 12px backdrop blur) with the logo, search, and cart; then the toldo; then a horizontally scrolling category rail with a sliding Brasa indicator. On scroll, the header compacts: the logo swaps to the isotipo, the scallops hide, and the rail chips shrink from 72px stacked icon-over-label to 44px inline.

Spacing follows a 4px base (4, 8, 12, 16, 24). Sections are separated by 48px on mobile and 64px on desktop.

- **Mobile (<760px):** item cards sit in a 2-column grid. An odd last card spans full width with the photo beside the text. Featured items scroll sideways at 200px each. Drinks are a single-column list. Sheets rise from the bottom edge with a grabber.
- **Desktop (≥760px):** search moves inline. Each category becomes one snapping, horizontally scrolling row of 3 cards (4 at ≥1040px) with prev/next round buttons. Featured items become a 3-column grid (4 at ≥1040px). Drinks use 2 columns (3 at ≥1040px) and combos use 2. Sheets become a centered modal (max 520px wide). The order bar docks to the bottom-right.
- The floating order bar respects `safe-area-inset-bottom`, and the footer reserves 120px so the bar never covers content.

## Elevation & Depth

Depth is mostly tonal: Asfalto → Carbón → Plancha, each separated by a 1px Hollín border. Two shadows add accents on top of that, and each has one job.

### Shadow Vocabulary
- **Sticker** (`3px 3px 0 #000`): a hard offset shadow with no blur, for stickers, tilted promo photos, and the wide combo photo. It reads as printed paper stuck on.
- **Glow** (`0 8px 28px` of Brasa at 35%): the warm halo under Brasa-filled actions (add button, CTA, order bar, the "next" arrow) and under a card while it tilts.

### Named Rules
**The Flat-at-Rest Rule.** Cards, rows, fields, and sheets carry no shadow at rest. Glow belongs to actions, and to a card only while the pointer is tilting it.

## Shapes

Corners are soft and friendly, and every interactive pill is fully round. Cards, rows, fields, and choices use 16px. Combos, the promo tile, sheets, and the empty state use 24px. Stickers use 8px, and small thumbnails 12px. Buttons, search, the segmented control, the stepper, count badges, and the order bar are pills (999px).

The signature shapes are the toldo, 24px alternating Brasa/Maíz stripes with a row of 12px scallops; and the **tilt**: stickers at −4°, marker text at −3°, and promo and combo photos at +3° to +6°. The tilts add the hand-made feel inside an otherwise orderly grid.

## Components

### Buttons
Tactile pills: they press in on touch and spring back.
- **Primary CTA:** a full-width Brasa pill, 56px tall, with Lead text in Tinta and the Glow shadow. Active state scales to 0.97 and darkens to the pressed Brasa (86% Brasa mixed with Tinta). Disabled is 45% opacity with no glow.
- **Add (+):** a 44px Brasa circle with the Glow shadow. Hover scales to 1.08. Active scales to 0.84. After a tap, the plus icon spins 90° and a copy of the photo flies to the cart.
- **Dark pill:** a 48px Tinta pill with Masa text, used inside orange surfaces (the promo CTA). Hover nudges it 3px right.
- **Icon button:** a 44px Plancha circle with a Hollín border. Active scales to 0.92, and hover to 1.06.
- **Focus (all):** a 3px Maíz outline with 2px offset.

### Chips (category rail)
- **Style:** transparent with a Hollín border and a 16px radius. Masa text with a 24px stroke icon.
- **Active:** a Brasa indicator slides behind the chip (0.45s ease-out), and the text turns Tinta and bold. A Maíz ripple spreads from the press point.

### Cards / Containers
- **Item card:** Carbón background, Hollín border, 16px radius. A square photo slot (4:3 in Featured) fades into the card at the bottom. The body uses 12px padding (16px on desktop), then the name, a 2-line description, tags, and a footer with the price and the Add button. Cards reveal by rising 24px and fading in with a stagger. With a fine pointer, a card tilts up to ±6° with a glare that follows the cursor, and its photo zooms to 1.06.
- **Row (drinks):** a compact Carbón row with a 64px rounded thumbnail.
- **Combo:** Carbón, 24px radius, 16px padding (24px on desktop). Bowlby name, an included-items list in Humo, a figure-size price, and two photos overlapping at opposite tilts.

### Inputs / Fields
- **Style:** Carbón fill, Hollín border, 16px radius, at least 48px tall, with labels in Label/Humo above. The search field is a Plancha pill with a leading icon.
- **Choice rows:** 48px bordered rows with a Brasa radio or checkbox, and the price delta right-aligned in Humo.
- **Error:** the border and message turn Maíz, in casual copy ("Dinos a nombre de quién va.").

### Navigation
The fixed header (topbar, toldo, rail) is the only navigation. The toldo's progress layer fills with scroll position, and the base layer fades to 25% when the header compacts.

**The opening moment.** On load, the toldo unrolls left to right behind a clip-path (0.7s, expo ease-out), and the scallops follow and drop 6px into place. It is the system's one authored entrance and never delays content. With reduced motion, it fades in instead.

### Motion grammar
- **Exits are faster than entrances.** Sheets open in 0.45s ease-out and close in 0.26s ease-in.
- **State slides, it doesn't snap.** The delivery/pickup thumb glides between options, totals count to their new value, and a cart line at zero slides out and collapses.
- **Errors nudge once.** An empty required field shakes for 0.32s, and a second send attempt replays it.
- **Loops sleep offscreen.** The marquee and the bestseller shimmer pause when they're out of view.
- **Reduced motion keeps feedback.** Adding to the cart flashes the badge and order bar Maíz, and sheets fade in and out.

### Sheets
A Plancha surface with a 24px top radius that slides up from the bottom on mobile (0.45s ease-out) over a 72% Asfalto scrim. On desktop it becomes a centered modal that scales up from 0.96. It traps focus and closes on Escape. The header uses a Bowlby title with a Humo count. The footer holds the total and the CTA.

### Order Bar (signature)
A floating Brasa pill (56px, 60px on desktop) with a Tinta count disc, a summary, and "Ver pedido". It springs up from below once the cart has items, and bumps on each add.

### Promo Tile (signature)
A full-bleed Brasa block with its own inverted toldo (Maíz/Tinta stripes and scallops). It holds a Tinta marker line, the uppercase Display headline, a dark pill CTA, and a +6° tilted photo with the Sticker shadow that drifts with scroll.

### Sticker
A Maíz tag with Tinta text in Micro uppercase, an 8px radius, rotated −4°, with the Sticker shadow. The bestseller sticker carries a slow shimmer sweep every 4s.

## Do's and Don'ts

### Do:
- **Do** keep text on Brasa or Maíz fills in Tinta (`tinta`).
- **Do** use Brasa Viva, not Brasa, for orange text on dark surfaces.
- **Do** separate surfaces with tone plus a 1px Hollín border before reaching for a shadow.
- **Do** keep every tap target at least 44px and every primary action a full pill.
- **Do** use tabular figures for every price, count, and total.
- **Do** give every new motion a `prefers-reduced-motion` fallback, the way the marquee, tilt, reveals, and springs already have one.
- **Do** reuse the toldo stripe (24px) and scallop (12px) geometry when a surface needs brand ornament.

### Don't:
- **Don't** add a third accent hue or recolor Cilantro for decoration; green means vegetarian.
- **Don't** set prices, item names, descriptions, or form text in Bowlby One or Permanent Marker.
- **Don't** put a resting shadow on cards, rows, fields, or sheets.
- **Don't** use white (#fff) or pure black text; Masa and Tinta are the extremes (pure black is reserved for the sticker shadow).
- **Don't** add a light theme without a deliberate redesign; the system is "Noche" only.
- **Don't** tilt functional controls (buttons, fields, chips); tilt belongs to stickers, marker text, and photos.
