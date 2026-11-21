---
version: alpha
name: "Craft"
description: "Craft's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Craft."
colors:
  primary: "rgb(3, 3, 2)"
  background: "rgb(252, 249, 247)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(3, 3, 2)"
  muted: "rgba(3, 3, 2, 0.65)"
  border: "oklab(0.0959089 -0.00155481 0.00499368 / 0.1)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(184, 202, 245)"
typography:
  display:
    fontFamily: '"Untitled Serif-d2ef79802246ca3a", "Untitled Serif-d2ef79802246ca3a fallback: Times New Roman", apple-system-ui-serif, ui-serif, Georgia, "serif"'
    fontSize: 66px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: '"Untitled Serif-d2ef79802246ca3a", "Untitled Serif-d2ef79802246ca3a fallback: Times New Roman", apple-system-ui-serif, ui-serif, Georgia, "serif"'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  heading:
    fontFamily: '"Untitled Serif-d2ef79802246ca3a", "Untitled Serif-d2ef79802246ca3a fallback: Times New Roman", apple-system-ui-serif, ui-serif, Georgia, "serif"'
    fontSize: 38px
    fontWeight: 400
    lineHeight: 0.99
    letterSpacing: -0.02em
  body:
    fontFamily: '"Untitled Sans-39d75ea677d0e81c", "Untitled Sans-39d75ea677d0e81c fallback: Arial", apple-system, Inter-d0c7129a07ebe9f6, "Inter-d0c7129a07ebe9f6 fallback: Arial", "system-ui", "Helvetica Neue", Helvetica, Arial, "sans-serif"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.02em
  action:
    fontFamily: '"Untitled Sans-39d75ea677d0e81c", "Untitled Sans-39d75ea677d0e81c fallback: Arial", apple-system, Inter-d0c7129a07ebe9f6, "Inter-d0c7129a07ebe9f6 fallback: Arial", "system-ui", "Helvetica Neue", Helvetica, Arial, "sans-serif"'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 2.44
    letterSpacing: -0.04em
rounded:
  control: 33554400px
  card: 24px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 60px
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

# Craft DESIGN.md

## Overview

A writing and productivity product combines a warm paper canvas, expressive Untitled Serif headlines, practical sans-serif controls, and tactile pastel collage. The tone is personal and editorial, with translucent navigation and soft depth around small actions.

Built from [/](https://www.craft.do/) and [/pricing](https://www.craft.do/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(3, 3, 2)` | Priority actions and selected emphasis |
| background | `rgb(252, 249, 247)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(3, 3, 2)` | Primary text |
| muted | `rgba(3, 3, 2, 0.65)` | Supporting text |
| border | `oklab(0.0959089 -0.00155481 0.00499368 / 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(184, 202, 245)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Untitled Serif-d2ef79802246ca3a" | 66px | 400 | 1 | -0.03em |
| display-mobile | "Untitled Serif-d2ef79802246ca3a" | 48px | 400 | 1 | -0.04em |
| heading | "Untitled Serif-d2ef79802246ca3a" | 38px | 400 | 0.99 | -0.02em |
| body | "Untitled Sans-39d75ea677d0e81c" | 16px | 400 | 1.4 | -0.02em |
| action | "Untitled Sans-39d75ea677d0e81c" | 18px | 400 | 2.44 | -0.04em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Untitled Sans-39d75ea677d0e81c"; src: url("https://www.craft.do/_astro/fonts/c8a444ca7e18cf43.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: "Untitled Sans-39d75ea677d0e81c"; src: url("https://www.craft.do/_astro/fonts/795a515e2ffadf7e.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: "Untitled Serif-d2ef79802246ca3a"; src: url("https://www.craft.do/_astro/fonts/e4ce2a394872d71d.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: "Untitled Serif-d2ef79802246ca3a"; src: url("https://www.craft.do/_astro/fonts/03692646d8666928.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: "Untitled Serif-d2ef79802246ca3a"; src: url("https://www.craft.do/_astro/fonts/c4ab86aeaefb6abe.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: "Untitled Serif-d2ef79802246ca3a"; src: url("https://www.craft.do/_astro/fonts/bce52696e5ea4c5b.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: italic; }
```

The full fallback stacks are in the front matter.

## Layout

Float a rounded navigation bar within a broad illustrated hero. Center a restrained serif headline above an original document frame, then alternate open editorial passages with pastel feature chapters. Pricing aligns softly rounded plan panels over the same collage atmosphere and stacks them on mobile.

Spacing scale: xs 8px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 52px high, with 0px left and 0px right padding. The sampled nav is static, 24px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `96.5156px 96.5156px 96.5156px 96.5156px 96.5156px` with gap `80px`; `164px 164px` with gap `32px 40px`; `55.5px 55.5px 55.5px 55.5px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `920px`, `100%`, `554px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0.01) 0px 50px 40px 0px, rgba(0, 0, 0, 0.02) 0px 50px 40px 0px, rgba(0, 0, 0, 0.05) 0px 20px 40px 0px, rgba(0, 0, 0, 0.08) 0px 3px 10px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `24px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact pill actions, translucent white navigation and toggles, subtly raised white controls, and rounded pastel document or plan panels. Keep serif type for editorial hierarchy and price emphasis; use clear sans-serif labels for utility information.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 14px / 14px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original torn-paper edges, grain, soft clouds, colored stationery layers, and generic document blocks. Small loose line drawings can make explanations approachable. Do not reuse the source collage, note templates, product screens, or wordmark.

**Motion.** Observed CSS transition declarations include `-webkit-backdrop-filter, backdrop-filter 0.1s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`, `all 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Warm, clear, and thoughtful, with brief functional labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

