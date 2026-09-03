---
name: StakeMyGold
description: Crypto XP leaderboard where every point is a stake on future gold.
colors:
  navy: "#0E1729"
  navy-2: "#1B2942"
  gold: "#F0BD5E"
  gold-lt: "#F9DDA0"
  gold-pale: "#FDF0CC"
  gold-dp: "#9A6A0A"
  ink: "#12161F"
  muted: "#7C7768"
  line: "#E7E0D2"
  paper: "#FFFFFF"
  cream: "#F8F6F2"
  bg: "#FDFCFA"
  bronze: "#A9763F"
  silver: "#98A2B0"
  plat: "#6E7B8B"
typography:
  display:
    fontFamily: "'Archivo Black', sans-serif"
    fontSize: "clamp(50px, 11vw, 132px)"
    fontWeight: 900
    lineHeight: 0.86
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "'Playfair Display', serif"
    fontSize: "33px"
    fontWeight: 700
    lineHeight: 1.2
  title:
    fontFamily: "'Playfair Display', serif"
    fontSize: "36px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "'IBM Plex Mono', monospace"
    fontSize: "9.5px"
    fontWeight: 500
    letterSpacing: "0.1em"
rounded:
  pill: "999px"
  card-lg: "18px"
  card-md: "16px"
  card-sm: "14px"
  input: "999px"
  sm: "6px"
spacing:
  page-max: "1180px"
  wrap-pad: "24px"
  wrap-pad-mobile: "18px"
  section-gap: "60px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "#2A2004"
    rounded: "{rounded.pill}"
    padding: "8px 18px"
  button-primary-hover:
    backgroundColor: "{colors.gold-lt}"
    textColor: "#2A2004"
    rounded: "{rounded.pill}"
    padding: "8px 18px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "8px 18px"
  button-gold-gradient:
    backgroundColor: "linear-gradient(180deg, {colors.gold-lt}, {colors.gold})"
    textColor: "#2A2004"
    rounded: "{rounded.pill}"
    padding: "10px 24px"
  stat-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.navy}"
    rounded: "{rounded.card-md}"
    padding: "21px 23px"
  stat-card-me:
    backgroundColor: "linear-gradient(160deg, #FFFEF9, #FFFBEF)"
    textColor: "{colors.gold-dp}"
    rounded: "{rounded.card-md}"
    padding: "21px 23px"
  podium-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.navy}"
    rounded: "{rounded.card-sm}"
    padding: "20px 22px 24px"
  podium-card-first:
    backgroundColor: "linear-gradient(160deg, #FFFEF8, #FFFAEC)"
    textColor: "{colors.gold-dp}"
    rounded: "{rounded.card-sm}"
    padding: "24px 22px 28px"
---

# Design System: StakeMyGold

## Overview

**Creative North Star: "The Gilded Vault"**

StakeMyGold is a leaderboard where participation is a bet on future value — XP accumulates like gold in a vault, and this interface communicates that gravity. The visual system pairs a deep navy that reads as sealed, authoritative darkness with a warm, measured gold that signals real achievement rather than decoration. These are not "cool crypto colors" — they are the palette of a treasury: serious, considered, earned.

The surface layer — cream, paper, near-white — keeps the day-to-day experience warm and legible. Navy is reserved for command surfaces (the header, the referral block, the mobile nav). Gold appears exactly as often as it should: to mark live status, to highlight the user's own rank, to crown the podium leader. Its restraint is its power.

Typography operates in three registers: Archivo Black for the wordmark alone (a stamp, not a label), Playfair Display for editorial weight (section headings, large stat numbers — these feel cast, not typed), and IBM Plex Mono for data precision (rank positions, step labels, stat axis labels — this is the ledger typeface). Inter handles everything else: approachable, neutral, fast to scan.

**Key Characteristics:**
- Navy + warm gold as the only authority pairing — not gradient-washed, not glassy
- Three-typeface system with strict role assignment: stamped / cast / measured / readable
- Gold used as certification, not wallpaper — scarcity maintained across every surface
- Flat-by-default depth with state-responsive shadows (hover, elevation, focus)
- Podium ranking inherits real metal semantics: gold / silver / bronze, not arbitrary hues

## Colors

A treasury palette: deep authority, warm precious metal, cream warmth — and nothing else.

### Primary
- **Midnight Vault** (`#0E1729`): The dominant dark. Used for the sticky header, the referral block, the mobile navigation overlay, and the dark-mode base. Not softened with blue-tint — this reads as sealed storage.
- **Navy Depth** (`#1B2942`): One step lighter than Midnight Vault. Used sparingly for layering in dark surfaces only.

### Secondary
- **Alchemist's Gold** (`#F0BD5E`): The primary accent. CTA button fill, "Live" status border, focus rings, "Your rank" highlights, the first podium stripe. Used at ≤15% surface coverage — its rarity is the signal.
- **Light Gold** (`#F9DDA0`): Gold at reduced chroma. Hover states, focus ring on dark surfaces, the warm glow on hover CTAs.
- **Gold Pale** (`#FDF0CC`): Near-white gold. The step-label gradient tail, subtle warm accents inside light cards.
- **Deep Gold** (`#9A6A0A`): Gold pressed into darkness. Text-only: the "Your rank" stat number, the first podium rank label. Never used as a fill or border — only ink.

### Tertiary
- **Bronze** (`#A9763F`): Third-place podium color. Used only in podium context.
- **Silver** (`#98A2B0`): Second-place podium color. Used only in podium context.
- **Platinum** (`#6E7B8B`): Tertiary podium reference, used minimally.

### Neutral
- **Near-Black Ink** (`#12161F`): Body text. Slightly warmer than pure black — this is vellum ink, not digital black.
- **Warm Muted** (`#7C7768`): Secondary text, labels, metadata. Has a warm ochre undertone — stays in palette even at reduced intensity.
- **Parchment Line** (`#E7E0D2`): All borders and dividers. Warm, never cool-gray — the system has no neutral-gray surfaces.
- **Paper** (`#FFFFFF`): Card backgrounds, stat surfaces. Pure white for maximum contrast against ink.
- **Cream** (`#F8F6F2`): Partners strip background. Slightly warm off-white — separates from Paper without competing.
- **Page Warm White** (`#FDFCFA`): The page background. Imperceptibly warm — lighter than Cream but not neutral.

### Named Rules
**The One Voice Rule.** Gold (#F0BD5E) marks exactly one thing per context: the active state, the ranked leader, the live signal, the primary CTA. When two gold elements compete for attention on the same screen, one of them is wrong.

**The Warm Neutrals Rule.** No cool grays. Every neutral — from the page background to the divider line to secondary text — has a warm undertone. If a gray reads as "digital" or "cool", it is out of palette.

## Typography

**Display Font:** Archivo Black (sans-serif fallback)
**Serif/Data Font:** Playfair Display (Georgia, serif fallback)
**Label/Mono Font:** IBM Plex Mono (monospace fallback)
**Body Font:** Inter (system-ui, sans-serif fallback)

**Character:** A deliberate four-voice system where every role is non-negotiable. Archivo Black stamps identity; Playfair Display casts weight on numbers and headings that need to feel solid; IBM Plex Mono reads data as a ledger; Inter keeps the copy fast and undecorated. No font is interchangeable with another.

### Hierarchy
- **Display** (Black, clamp(50px–132px), line-height 0.86, tracking -0.035em): The wordmark only. Never used for section headings or body labels.
- **Headline** (Playfair Display 700, 33px, line-height 1.2): Section headings in the "How it Works" block. The serif lends editorial authority — a heading that feels written, not generated.
- **Title / Stat** (Playfair Display 700, 36px, line-height 1.0, tracking -0.02em): Large data numbers in stat cards. These numbers feel cast in metal, not printed on a screen.
- **Body** (Inter 400, 15px, line-height 1.5): All copy, metadata, table content, navigation labels. Measure: 65–75ch on prose; no max-width on tabular data.
- **Label** (IBM Plex Mono 500, 9.5–11px, tracking +0.1em, uppercase): Stat axis labels (dt), step numbers, rank positions, leaderboard column headers. The ledger voice — always uppercase, always measured.

### Named Rules
**The Three-Register Rule.** Playfair for editorial weight. IBM Plex Mono for data precision. Inter for everything readable. Archivo Black for the wordmark alone. Mixing these — using Mono for headings, or Playfair for body copy — breaks the register system.

**The Tracking Inversion Rule.** Display and title type tracks tightly (negative). Label type tracks openly (positive). Body type tracks neutrally. This inversion is structural: tight tracking = large and present; open tracking = small and precise.

## Layout

The page uses a single centered column at `max-width: 1180px` with 24px horizontal padding (18px on ≤640px, 14px on ≤420px). There is no multi-column page layout — all sections stack vertically with generous section gaps (60px desktop, 36–52px mobile).

The sticky header (`height: 56px`) is always visible and uses full-width navy — it is not contained. Below the header, a partners ticker strip spans full width before the contained hero section begins.

The stats grid is a `4-column CSS grid` (collapsing to 2 columns on mobile ≤640px) with `1px` gaps rendered via a background color technique — the grid background is `--line` and cells are white, producing hairline separators without border-box complications.

The podium uses a `3-column CSS grid`. The leaderboard below is a standard HTML table with sticky column headers.

Responsive breakpoints:
- **≤900px**: Burger menu appears, desktop nav hides
- **≤640px**: 2-column stats, reduced padding, mobile-specific hand positions
- **≤420px**: Further padding reduction, collapsed archived facts

## Elevation & Depth

This system is **flat by default**. Surfaces are white or cream with `1px solid --line` borders at rest — no ambient shadows, no glass effects. Depth is conveyed through the border color hierarchy (line → navy) and tonal background layering (paper → cream → gold-pale), not through z-axis lift.

Shadows appear only in response to state or structural elevation:

### Shadow Vocabulary
- **Whisper** (`0 1px 2px rgba(20,16,4,.04)`): On the Live pill at rest. Nearly imperceptible — more of a material hint than a shadow.
- **Float** (`0 1px 8px rgba(0,0,0,.05)`): Light card elevation, archived notes. The suggestion of lift.
- **Hover Lift** (`0 4px 18px rgba(20,16,4,.07)` or `rgba(0,0,0,.07)`): Cards (step, squad) on hover. The surface rises to meet the cursor.
- **Gold Haze** (`0 4px 18px rgba(200,158,20,.10)`): First-place podium card only. A warm glow beneath the gold border — the system's one chromatic shadow.
- **Strong Hover** (`0 6px 24px rgba(20,16,4,.07)`): Step cards at hover — slightly more pronounced than standard card hover.
- **FAB Elevation** (`0 4px 18px rgba(0,0,0,.45)`, `0 6px 24px rgba(0,0,0,.55)` hover): Settings panel FAB button. The one element that floats at full elevation by design.

### Named Rules
**The Flat-By-Default Rule.** Shadows exist only as a response to interaction (hover) or a structural hierarchy decision (the FAB, the first podium card). A shadow at rest is a hierarchy claim the element must earn.

**The Gold Haze Exception.** The first-place podium card earns a warm chromatic shadow. It is the only card with a colored shadow — all other hover shadows are near-black tinted warm. The exception is the rule.

## Shapes

The system uses two radii in rotation: **999px (pill)** for interactive controls (buttons, CTAs, season selectors, filter chips, tags), and **14–18px (large card)** for content containers. There is no middle-ground radius — no 8px input or 12px button. This binary creates a clear distinction: controls are fully rounded; containers are gently rounded.

Borders are all `1px solid --line` at rest, upgrading to `1.5px solid --navy` for active/selected states. The border-width change on selection (1px → 1.5px) communicates state without color change — typography handles the color shift (muted → ink/navy).

The three-step card uses a `3px top stripe` as its only decoration: gold for step 1, silver-gradient for step 2, bronze-gradient for step 3. This inherited the podium's metal hierarchy — the only place in the system where `::before` is used as a semantic decoration (rank signaling), not mere embellishment.

The hero wordmark uses `overflow:hidden` to animate letter entrance. The page itself uses `overflow:hidden` on the hero section to contain the absolute-positioned hand imagery and halftone canvas.

## Components

### Buttons

**Character:** Pill-shaped, always rounded to 999px. The primary CTA is gold-filled — the only filled element in the lighter surfaces. Ghost buttons are the workhorse; gold CTAs are the exception.

- **Shape:** 999px radius — fully rounded, never rectangular
- **Primary (Gold Fill):** Gold (`#F0BD5E`) background, deep-dark text (`#2A2004`), 700 weight, 13.5px, 8px 18px padding. Transition: filter + background + color at 0.16–0.20s.
- **Primary Hover:** Lighten via `filter:brightness(1.04)` — no background swap needed; the gold already draws attention.
- **Gold Gradient:** `linear-gradient(180deg, --gold-lt, --gold)` fill for larger secondary CTAs (copy referral link, etc.)
- **Ghost (Neutral):** `1px solid --line`, white background, ink text — used in board footer pagination, secondary actions.
- **Connected State:** Transparent background, `rgba(255,255,255,.18)` border, `--gold-lt` text — used when wallet is connected, indicating a passive confirmed state.

### Chips / Selectors

Pill-shaped (`999px`), 12.5px Inter, `--muted` text by default. Active: `1.5px solid --navy`, `--ink` text, 600 weight. Used for season selectors in the board header and view-mode segmented controls. The width change on active state (1px → 1.5px border) is the selection signal.

### Cards / Containers

**Stat Cards** — part of a 4-up CSS grid:
- Background: `--paper`
- Border: via grid gap technique (parent background = `--line`, 1px gap)
- Radius: 16px on the parent grid container
- Padding: 21px 23px
- The "me" variant adds a warm gold gradient background and a `3px solid --gold` left accent

**Podium Cards:**
- Background: `--paper` (second/third), gold warm gradient (first)
- Border: `1px solid --line` with gold accent border on first: `1px solid rgba(240,189,94,.5)`
- Radius: 14px
- Padding: 20px 22px 24px; first card: 24px 22px 28px
- Top stripe: `3px` gradient accent (gold / silver / bronze) via `::before`

**Step Cards (How it Works):**
- Background: `--paper`, `1px solid --line` border, 16px radius
- Top stripe: `3px ::before` in gold/silver/bronze gradient by step order
- Padding: 24px 22px (desktop), 20px 18px (mobile)
- Hover: `0 6px 24px` warm shadow, border lightens to `#cfc5b4`

**Board Container:**
- Background: `--paper`, `1px solid --line`, 18px radius — the largest card radius in the system
- Contains a sticky `thead` with `background: #FDFBF6` (between paper and cream)

### Navigation

**Desktop (>900px):** Inline flex row, centered, 14px Inter, `rgba(255,255,255,.6)` default, white hover/active, letter-spacing -0.025em. No underlines, no indicators — purely weight and color shift.

**Mobile (≤900px):** Full-height overlay below the 56px header. Navy background, 30px 700 Inter links, centered. Burger morphs to × via CSS transform on three spans. The header remains visible (sticky) while the nav slides down from below it.

**The Brand Block:** SVG logo mark + "StakeMyGold" wordmark. Brand text hides (not the logo) when the mobile menu is open, keeping the mark as spatial anchor while reducing visual competition.

### Leaderboard Table

- `thead`: IBM Plex Mono 500, 11.5px, uppercase, `--muted` text, warm near-white background (`#FDFBF6`)
- `tbody`: Inter 13.5–14.5px, with rank column in IBM Plex Mono
- `tr.you`: highlighted with gold-dp text on name, gold-pale left border (`3px`)
- Hover: `rgba(248,246,242,.8)` row tint — cream wash, not a hard highlight

### Signature: The Rank Podium

The three-card podium is the visual centerpiece of the leaderboard. The first-place card is larger, has a warm gold gradient background, a gold ambient haze shadow, and a `3px ::before` stripe in the gold-dark-to-light direction. Second and third cards get silver and bronze stripe gradients respectively. XP numbers use Playfair Display at 32–38px (desktop), reinforcing the "cast in metal" data register. This is the system's maximum expression of visual weight.

## Do's and Don'ts

### Do:
- **Do** use gold (#F0BD5E) at ≤15% visible surface coverage. It is a signal, not a theme.
- **Do** use IBM Plex Mono in uppercase with 0.1em letter-spacing for all data labels, rank positions, and axis labels.
- **Do** use Playfair Display for section headings and large data numbers — this is the "weight" register, not Inter Bold.
- **Do** keep all neutral colors warm-toned. If a gray doesn't have an ochre or amber undertone, it is out of palette.
- **Do** use 999px radius for all interactive controls (buttons, chips, tags) and 14–18px radius for content containers. No middle ground.
- **Do** let shadows appear only on hover, focus, or explicit structural elevation (podium first card, FAB). Surfaces are flat at rest.
- **Do** reserve the navy (#0E1729) for command surfaces: header, referral CTA block, mobile nav. Never use it for content cards.

### Don't:
- **Don't** use gradient text. Emphasis comes from size, weight, or the Playfair Display register — not a gradient fill on text.
- **Don't** add a colored `border-left` above 1px on general content cards. The `.stat.me` left accent (3px) is the single permitted exception, because it signals "your own data" — a semantic distinction, not decoration.
- **Don't** use Inter Bold or Inter Black for headings that should use Playfair Display. The serif register exists precisely to avoid Inter at display sizes.
- **Don't** use cool-toned grays. `#7C7768` (Warm Muted) is the floor for secondary text — anything cooler breaks the palette's thermal consistency.
- **Don't** apply box shadows to surfaces at rest. A shadow at rest is a hierarchy claim that erodes the system's flat-by-default integrity.
- **Don't** use Archivo Black for anything except the wordmark. It is the stamp; using it elsewhere dilutes it.
- **Don't** introduce a fourth neutral background color. The system has three: `--bg` (#FDFCFA), `--cream` (#F8F6F2), `--paper` (#FFFFFF). Adding another warm near-white creates ambiguity without distinction.
