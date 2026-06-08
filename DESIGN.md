---
name: Energy+ Offer Audit
description: A deep-navy, champagne-accented diagnostic that turns an energy pro's coverage gaps into market access.
colors:
  navy: "#0a1622"
  navy-mid: "#0f1f2e"
  navy-light: "#16293b"
  navy-card: "#0c1a28"
  navy-hero: "#122438"
  navy-deep: "#060f17"
  amber: "#c2a368"
  amber-light: "#d8bf8a"
  amber-pale: "#ead7ab"
  white: "#fbfbf8"
  cream: "#e7e6e0"
  mid: "#afc1cf"
  muted: "#8597a6"
  green: "#57bf98"
  red: "#d6796d"
typography:
  display:
    fontFamily: "Spectral, Georgia, serif"
    fontSize: "clamp(2.8rem, 1.5rem + 5.2vw, 5.25rem)"
    fontWeight: 300
    lineHeight: 1.12
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Spectral, Georgia, serif"
    fontSize: "clamp(2rem, 1.45rem + 2.5vw, 3.4rem)"
    fontWeight: 400
    lineHeight: 1.12
    letterSpacing: "normal"
  title:
    fontFamily: "Spectral, Georgia, serif"
    fontSize: "clamp(1.25rem, 1.05rem + 0.95vw, 1.65rem)"
    fontWeight: 500
    lineHeight: 1.32
    letterSpacing: "normal"
  body:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: "normal"
  label:
    fontFamily: "Barlow Condensed, system-ui, sans-serif"
    fontSize: "0.72rem"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "0.12em"
rounded:
  none: "0"
  sm: "2px"
spacing:
  s-1: "0.25rem"
  s-2: "0.5rem"
  s-3: "0.75rem"
  s-4: "1rem"
  s-5: "1.5rem"
  s-6: "2rem"
  s-7: "3rem"
  s-8: "4rem"
components:
  button-primary:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.navy}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "16px 32px"
  button-primary-hover:
    backgroundColor: "{colors.amber-light}"
    textColor: "{colors.navy}"
  button-ghost:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.cream}"
    rounded: "{rounded.sm}"
    padding: "16px 32px"
  tag:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.navy}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "4px 10px"
  card:
    backgroundColor: "{colors.navy-card}"
    textColor: "{colors.cream}"
    rounded: "{rounded.none}"
    padding: "32px"
---

# Design System: Energy+ Offer Audit

## 1. Overview

**Creative North Star: "The Field Engineer's Audit Report"**

This is a genuine diagnostic that happens to close a sale. The surface reads like a serious deliverable an operator would respect: a deep-navy field of charged information, hairline-ruled and numbered like a real coverage report, warmed only by champagne accent and a Spectral serif. The diagnostic earns its conversion by looking and behaving like the real thing. Sharp and consultative first; warm enough in the findings that a gap lands as an invitation, never a verdict.

Warmth is deliberate and rationed. It comes from the champagne accent and the serif type, **never** from a tinted or cream background. The page is dark because the work is serious and the markets are big; the heat is the accent, used sparingly so it always means something. The emotional arc the visuals serve is two beats: a small sting (money and market access left on the table), then immediate relief (the path forward is on the same screen).

This system explicitly rejects four things. It is **not** a cheesy quiz: no score-reveal theatrics, no confetti, no playful illustration. It is **not** a generic SaaS template: no cream/sand background, no tracked-uppercase eyebrow over every section, no identical icon-card grid. It is **not** a pushy lead-capture funnel: no popups, countdowns, or gated walls; the CTA is earned by the findings. And it is **not** sterile corporate navy-and-gray: a real person (Daniel) with real expertise stands behind it.

**Key Characteristics:**
- Deep-navy surface, champagne as the single rationed accent
- Spectral serif for display and headings; Barlow for body, Barlow Condensed for labels and numerals
- Hairline rules and a numbered/index feel borrowed from real audit reports
- WCAG AA contrast as a floor, not a target
- Motion that confirms and reveals, never performs

## 2. Colors

A deep-navy ramp carrying the surface, with champagne as the only accent and green/red reserved strictly for the with/without comparison.

### Primary
- **Champagne** (`#c2a368`): The only accent and the heat of the page. Primary buttons, hairline rules, the 01–12 numerals, uppercase labels, tags, and the focus ring. Used sparingly; rarity is what makes it read as valuable.
- **Champagne Light** (`#d8bf8a`): Champagne for use *as text or links on dark* and for hover states, where the base champagne would be too dim. Also the focus-ring color.
- **Champagne Pale** (`#ead7ab`): Reserved for italic Spectral pull-quotes.

### Neutral (surfaces — the deep-navy ramp)
- **Navy** (`#0a1622`): The page background. The default field everything sits on.
- **Navy Mid** (`#0f1f2e`): Alternating section background, for rhythm between beats.
- **Navy Card** (`#0c1a28`): Card and panel surface at rest.
- **Navy Light** (`#16293b`): Card hover / lift state.
- **Navy Hero** (`#122438`): Mid-stop of the hero gradient.
- **Navy Deep** (`#060f17`): Footer and deepest sections.

### Neutral (text)
- **White** (`#fbfbf8`): Headlines only.
- **Cream** (`#e7e6e0`): Body text. ~14:1 on navy.
- **Mid** (`#afc1cf`): Leads and brighter secondary text. ~9:1 on navy.
- **Muted** (`#8597a6`): Supporting text and captions. ~5.5:1 on navy. The dimmest grey permitted.

### Tertiary (status — comparison only)
- **Green** (`#57bf98`): The "with Energy+" / positive side of the comparison.
- **Red** (`#d6796d`): The "without" / negative side of the comparison.

### Lines
- **Champagne hairline** (`rgba(194,163,104,0.22)`): The accented dividing rule.
- **Neutral hairline** (`rgba(255,255,255,0.06)`): Grid gaps and quiet dividers.

### Named Rules
**The Rationed Heat Rule.** Champagne is the only accent and it is used sparingly. If champagne is doing more than ~10% of a screen, it has stopped being the heat and started being the wallpaper. Cut it back.

**The Filled-Accent-Goes-Dark Rule.** Anything filled with champagne (buttons, tags) takes `color: var(--navy)` dark text (~6.5:1). White text on champagne is forbidden.

**The No-Dimmer-Grey Rule.** `--muted` (`#8597a6`) is the floor. Never introduce a greyer, dimmer text color on navy; it fails AA and reads as faint.

**The Comparison-Only Status Rule.** Green and red appear only in the with/without comparison. Never decorative, never as general UI color.

## 3. Typography

**Display Font:** Spectral (with Georgia, serif fallback)
**Body Font:** Barlow (with system-ui fallback)
**Label/Numeral Font:** Barlow Condensed

**Character:** A contrast pairing, not a similar-but-different one. Spectral's literary, slightly cool serif carries authority and the human warmth that the dark surface withholds; Barlow's clean grotesque keeps findings legible and matter-of-fact; Barlow Condensed gives labels and the 01–12 numerals a tight, report-index rhythm.

### Hierarchy
- **Display** (Spectral 300, `clamp(2.8rem, 1.5rem + 5.2vw, 5.25rem)`, line-height 1.12): Hero statement only. Thin weight is permitted *here and only here*.
- **Headline** (Spectral 400, `clamp(2rem, 1.45rem + 2.5vw, 3.4rem)`, 1.12): Section openers.
- **Subhead / H2** (Spectral 400–500, `clamp(1.55rem, 1.15rem + 1.9vw, 2.6rem)`, 1.32): Secondary section headings.
- **Title / H3** (Spectral 500, `clamp(1.25rem, 1.05rem + 0.95vw, 1.65rem)`, 1.32): Card and finding titles.
- **Lead** (Barlow 400, `1.2rem` / ~19px, 1.65, color `--mid`): Intro paragraphs under a heading.
- **Body** (Barlow 400, `1.0625rem` / 17px, 1.65, color `--cream`): Default running text. Cap measure at 65–75ch.
- **Secondary** (Barlow 400, `0.95rem` / 15px): Captions and supporting text. The smallest body size allowed.
- **Label** (Barlow Condensed 600, `0.72rem`, letter-spacing `0.12em`, uppercase): Short eyebrows, tags, ≤4 words. Champagne.

### Named Rules
**The 400-Floor Rule.** Body weight is 400, minimum 15px (`--t-sm`). Weight 300 is reserved exclusively for large Spectral display. Light-weight body on dark reads faint and is banned.

**The Serif-Is-The-Voice Rule.** Spectral carries every display and heading. Barlow never sets a headline; Spectral never sets running body. The pairing works because the roles never blur.

## 4. Elevation

Largely flat. Depth comes from the navy ramp (tonal layering) and hairline rules, not from drop shadows. Cards are distinguished by surface (`--navy-card`) and a hairline, lifting to `--navy-light` on hover. Shadows, if used at all, are a quiet response to state (hover/lift), never an ambient decoration at rest.

### Named Rules
**The Tonal-Depth Rule.** Layer with the navy ramp and hairlines, not shadows. If a surface needs to feel raised, change its navy step or add a champagne hairline before reaching for a shadow.

## 5. Components

### Buttons
- **Shape:** Sharp-edged (`0`–`2px` radius). Editorial, not pill-shaped. *(Radius is provisional; confirm at implementation.)*
- **Primary:** Champagne fill (`--amber`), navy text (`--navy`), Barlow Condensed uppercase label, padding ~`16px 32px`. Hover → `--amber-light`. This is the close; it carries the heat.
- **Ghost / Secondary:** Navy background, cream text, champagne hairline border. For lower-priority actions so the primary stays singular.
- **Focus:** Champagne-light focus ring (`--amber-light`), always visible.

### Tags / Chips
- **Style:** Champagne fill, navy text, Barlow Condensed uppercase, small padding. Same filled-accent-goes-dark rule as buttons.

### Cards / Panels
- **Corner Style:** Sharp (`0`). Hairline-defined, report-like.
- **Background:** `--navy-card` at rest, `--navy-light` on hover.
- **Border:** Champagne hairline (`--border`) or neutral hairline (`--border-sub`) for grid gaps.
- **Shadow Strategy:** None at rest (see Elevation).
- **Internal Padding:** `--s-6` (`2rem`) typical.

### Inputs / Fields (audit flow)
- **Style:** Navy surface, hairline border, cream text, sharp corners.
- **Focus:** Champagne-light ring; border shifts to champagne. No glow.
- **Selected answer:** Champagne hairline or champagne text marks the chosen option; avoid heavy filled blocks that turn the flow into a quiz.

### The With/Without Comparison (signature component)
The only place green and red appear. Two columns or paired rows: the "without" state in `--red`, the "with Energy+" state in `--green`. This is where the sting becomes relief made literal. Keep it sober and tabular, like a real findings comparison, not a celebratory before/after.

### Numerals / Index (signature detail)
The 01–12 numerals set in Barlow Condensed, champagne, as a real catalog/index sequence (questions, solutions, sections that genuinely *are* ordered). Numbers are earned by actual sequence, never sprinkled as decoration.

## 6. Do's and Don'ts

### Do:
- **Do** keep the background deep navy and let warmth come from champagne accent + Spectral serif only.
- **Do** ration champagne to ≤~10% of any screen; it is the heat.
- **Do** give every champagne-filled element dark navy text (~6.5:1).
- **Do** set body at weight 400, 15px minimum; reserve weight 300 for large Spectral display.
- **Do** keep text contrast within the ramp: body `--cream` (~14:1), leads `--mid` (~9:1), supporting `--muted` (~5.5:1).
- **Do** use `--ease-out` (ease-out-quint) as the only curve; ~100–150ms for micro-interactions, 200–450ms for reveals.
- **Do** ship one orchestrated hero entrance and stagger list reveals (`--i * 55ms`); gate reveals behind a `.js` class so content shows if JS fails.
- **Do** include a `@media (prefers-reduced-motion: reduce)` block that zeroes durations and reveals all content.
- **Do** restrict imagery (if any) to commercial/industrial infrastructure and schematics, duotone or grayscale-warm.

### Don't:
- **Don't** use a cream, beige, sand, or any tinted near-white background. (Anti-reference: generic SaaS template.)
- **Don't** use yellow-gold; champagne only. No gradient text. No glassmorphism by default.
- **Don't** put a tiny tracked-uppercase eyebrow above every section, or numbered markers as section scaffolding. Numbers are allowed only for a real sequence or a catalog index. (Anti-reference: generic SaaS template.)
- **Don't** use `border-left`/`border-right` greater than 1px as a colored side-stripe accent.
- **Don't** add quiz theatrics: no score-reveal animation, confetti, or playful illustration. (Anti-reference: cheesy quiz / BuzzFeed.)
- **Don't** add popups, countdowns, or gated walls; the CTA is earned by the findings. (Anti-reference: pushy lead-capture funnel.)
- **Don't** let it read as sterile corporate navy-and-gray; the champagne, serif, and Daniel's voice keep it human. (Anti-reference: corporate / sterile enterprise.)
- **Don't** use Cormorant Garamond (Spectral is the chosen serif) or emoji as icons.
- **Don't** use sunsets, leaves, residential-roof installers, handshakes, or SaaS 3D blobs in imagery.
- **Don't** introduce a grey dimmer than `--muted`, or white text on champagne.
- **Don't** use green/red anywhere but the with/without comparison.
