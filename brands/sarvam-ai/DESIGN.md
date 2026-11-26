---
version: alpha
name: "Sarvam AI"
description: "Sarvam AI's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Sarvam AI."
colors:
  primary: "rgb(42, 44, 51)"
  background: "rgb(252, 252, 252)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(31, 31, 31)"
  muted: "rgb(102, 102, 102)"
  border: "rgb(230, 230, 230)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Season Mix-3769fe463abea116", "Season Mix-3769fe463abea116 fallback: Arial", sans-serif'
    fontSize: 64px
    fontWeight: 425
    lineHeight: 1.05
    letterSpacing: -0.025em
  display-mobile:
    fontFamily: '"Season Mix-3769fe463abea116", "Season Mix-3769fe463abea116 fallback: Arial", sans-serif'
    fontSize: 44px
    fontWeight: 425
    lineHeight: 1.05
    letterSpacing: -0.025em
  heading:
    fontFamily: '"Season Mix-3769fe463abea116", "Season Mix-3769fe463abea116 fallback: Arial", sans-serif'
    fontSize: 36px
    fontWeight: 525
    lineHeight: 1.2
    letterSpacing: -0.02em
  body:
    fontFamily: 'Matter-b40cfa56c475acd1, "Matter-b40cfa56c475acd1 fallback: Arial", sans-serif'
    fontSize: 16px
    fontWeight: 425
    lineHeight: 1.6
    letterSpacing: 0em
  action:
    fontFamily: 'Matter-b40cfa56c475acd1, "Matter-b40cfa56c475acd1 fallback: Arial", sans-serif'
    fontSize: 16px
    fontWeight: 525
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 14.4px
spacing:
  xs: 6px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 64px
components:
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

# Sarvam AI DESIGN.md

## Overview

An AI platform uses Season Mix serif headlines with unusually precise intermediate weights, a near-white canvas, and restrained charcoal pill actions. Soft blue, violet, and orange atmosphere gives the opening and product diagrams a warm, crafted character without overwhelming the reading layer.

Built from [/](https://www.sarvam.ai/) and [/products/voice-agents](https://www.sarvam.ai/products/voice-agents), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(42, 44, 51)` | Priority actions and selected emphasis |
| background | `rgb(252, 252, 252)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(31, 31, 31)` | Primary text |
| muted | `rgb(102, 102, 102)` | Supporting text |
| border | `rgb(230, 230, 230)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Season Mix-3769fe463abea116" | 64px | 425 | 1.05 | -0.025em |
| display-mobile | "Season Mix-3769fe463abea116" | 44px | 425 | 1.05 | -0.025em |
| heading | "Season Mix-3769fe463abea116" | 36px | 525 | 1.2 | -0.02em |
| body | Matter-b40cfa56c475acd1 | 16px | 425 | 1.6 | 0em |
| action | Matter-b40cfa56c475acd1 | 16px | 525 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Matter-b40cfa56c475acd1; src: url("https://www.sarvam.ai/_astro/fonts/51f91abf4d5fa424.woff2") format("woff2"); font-display: swap; font-weight: 100 1000; font-style: normal; }
@font-face { font-family: "Season Mix-3769fe463abea116"; src: url("https://www.sarvam.ai/_astro/fonts/ed8cd4b03cbdf9e9.woff2") format("woff2"); font-display: swap; font-weight: 300 900; font-style: normal; }
```

The full fallback stacks are in the front matter.

## Layout

Use a thin announcement strip and compact navigation above a centered editorial introduction. Allow a large area of open space before customer proof and modular product chapters. The voice-agent page adds a horizontal use-case rail, paired starting actions, and a broad visual workflow panel. Mobile stacks these chapters and compacts the navigation.

Spacing scale: xs 6px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 104px high, with 0px left and 0px right padding. The sampled header is static, 151.5px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `595.984px 596px` with gap `8px`; `294px 294px` with gap `8px`; `193.328px 193.328px 193.328px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `896px`, `1400px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0.1) 0px 6px 70px 44px, rgba(20, 20, 20, 0.08) 0px 0px 18.6px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `14.4px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small pill actions, pale outlined companions, fine ruled rails, white workflow panels, and softly rounded information cards. Keep the serif hierarchy separate from compact functional sans-serif labels. Reuse subtle borders and limited elevation rather than heavy shadows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original soft gradient fields, abstract workflow diagrams, simple functional icons, and a restrained ornamental flourish. Diagrams may mix white panels with luminous violet elements.

**Motion.** Observed CSS transition declarations include `background-color, box-shadow, color, transform 0.35s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`, `color, border-color 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, explanatory, and developer-friendly.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
