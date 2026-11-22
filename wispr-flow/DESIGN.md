---
version: alpha
name: "Wispr Flow"
description: "Wispr Flow's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Wispr Flow."
colors:
  primary: "rgb(240, 215, 255)"
  background: "rgb(255, 255, 235)"
  surface: "rgb(255, 253, 249)"
  foreground: "rgb(26, 26, 26)"
  muted: "rgba(26, 26, 26, 0.7)"
  border: "rgb(228, 228, 208)"
  on-primary: "rgb(26, 26, 26)"
  accent: "rgb(3, 79, 70)"
typography:
  display:
    fontFamily: '"Eb garamond", Arial, sans-serif'
    fontSize: 96px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: '"Eb garamond", Arial, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  heading:
    fontFamily: '"Eb garamond", Arial, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  body:
    fontFamily: 'Figtree, Arial, sans-serif'
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0em
  action:
    fontFamily: 'Figtree, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0em
rounded:
  control: 8px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 55px
components:
  accent-text:
    textColor: "{colors.accent}"
  primary-button:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.control}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.card}"
    padding: "{spacing.lg}"
    typography: "{typography.body}"
  caption:
    textColor: "{colors.muted}"
  separator:
    backgroundColor: "{colors.border}"
---

# Wispr Flow DESIGN.md

## Overview

A voice-product site combines a pale yellow-cream canvas, very large EB Garamond editorial headings, italic emphasis, and compact sans-serif controls. Pale lavender download actions, deep green chapters, loose annotation, and a winding text-ribbon motif give the interface a warm human character.

Built from [/](https://wisprflow.ai/) and [/pricing](https://wisprflow.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(240, 215, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 235)` | Page canvas |
| surface | `rgb(255, 253, 249)` | Panels and cards |
| foreground | `rgb(26, 26, 26)` | Primary text |
| muted | `rgba(26, 26, 26, 0.7)` | Supporting text |
| border | `rgb(228, 228, 208)` | Quiet separators and outlines |
| on-primary | `rgb(26, 26, 26)` | Text on the primary action |
| accent | `rgb(3, 79, 70)` | Selective emphasis in headings, graphics, and small signals |



Use cream as the primary canvas, lavender for the prominent download action and selected controls, charcoal for text and alternate pricing actions, and deep green for substantial contrasting chapters. These roles are distinct from the small orange campaign or tier badges. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Eb garamond" | 96px | 400 | 0.95 | -0.03em |
| display-mobile | "Eb garamond" | 48px | 400 | 0.95 | -0.03em |
| heading | "Eb garamond" | 40px | 400 | 1 | -0.03em |
| body | Figtree | 20px | 500 | 1.3 | 0em |
| action | Figtree | 16px | 600 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Figtree; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd674912f33a67c2e346_Figtree-Bold.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: Figtree; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd6763ee33a2be0ffd05_Figtree-Medium.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: Figtree; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd676708c4fa3708edc8_Figtree-SemiBold.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; }
@font-face { font-family: "Eb garamond"; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbe57a719a4ebf1fb56d5_EBGaramond-Regular.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Figtree; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/683dcde1184812754ee64894_Figtree-Regular.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "Eb garamond"; src: url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/68d3db1d34da60ddf73ff544_683b1349ca0a0ddd3d6a7cd3_EBGaramond-Italic.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face{font-family:Figtree;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd674912f33a67c2e346_Figtree-Bold.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:Figtree;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd6763ee33a2be0ffd05_Figtree-Medium.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:Figtree;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbd676708c4fa3708edc8_Figtree-SemiBold.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap}
@font-face{font-family:Eb garamond;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/682fbe57a719a4ebf1fb56d5_EBGaramond-Regular.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Figtree;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/683dcde1184812754ee64894_Figtree-Regular.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Eb garamond;src:url("https://cdn.prod.website-files.com/682f84b3838c89f8ff7667db/68d3db1d34da60ddf73ff544_683b1349ca0a0ddd3d6a7cd3_EBGaramond-Italic.woff2")format("woff2");font-weight:400;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Float a compact bordered navigation within the cream page. Center a large two-line serif statement and a download action above an open visual field. Continue with dark or green product chapters, lifestyle sections, and generous spacing. Pricing uses a centered introduction and a row of outlined plan panels with small badge-like labels, stacked on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 55px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 48.3281px high, with 0px left and 0px right padding. The sampled nav is relative, 48.3281px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `354.094px 321.906px` with gap `32px`; `354.094px 321.906px` with gap `32px`; `354.094px 321.906px` with gap `32px`. Build them as a fluid grid. Sampled container maximum widths: `1238.4px`, `1440px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact lavender actions, thin dark outlined companions, softly rounded feature panels, small segmented switches, and tall plan cards with delicate rules. Pricing uses serif prices, small uppercase category labels, and visible included-feature checks. Preserve the balance between expressive headings and functional utility text.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48.3281px, horizontal padding 14px / 14px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 42px, radius 8px, background rgb(255, 255, 235), and border 1px rgb(228, 227, 222). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original lifestyle photography, neutral workflow illustrations, simple waveform motifs, loose hand-drawn accents, and an original winding text path using new wording.

**Motion.** Observed CSS transition declarations include `color 0.3s`, `transform, color 0.2s, 0.3s`, `opacity 0.3s`, `opacity 0.22s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Conversational, helpful, and easy to read.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
