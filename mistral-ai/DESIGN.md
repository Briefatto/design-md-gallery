---
version: alpha
name: "Mistral AI"
description: "Mistral AI's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Mistral AI."
colors:
  primary: "rgb(255, 82, 41)"
  background: "rgb(251, 251, 248)"
  surface: "rgb(251, 251, 248)"
  foreground: "oklch(0.21 0.006 285.885)"
  muted: "oklch(0.552 0.016 285.938)"
  border: "oklab(0 0 0 / 0.1)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(255, 175, 1)"
typography:
  display:
    fontFamily: 'ALTMistral, sans-serif'
    fontSize: 96px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'ALTMistral, sans-serif'
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.01em
  heading:
    fontFamily: 'ALTMistral, sans-serif'
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.18
    letterSpacing: -0.01em
  body:
    fontFamily: 'ALTMistral, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'ALTMistral, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
rounded:
  control: 0px
  card: 0px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 24px
  section: 80px
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

# Mistral AI DESIGN.md

## Overview

An AI platform uses warm white surfaces, large geometric lettering, fine grid boundaries and vivid orange-to-yellow pixel graphics. Blue and dark navy product panels provide contrast within a modular, technical layout.

Built from [/](https://mistral.ai/) and [/products](https://mistral.ai/products), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 82, 41)` | Priority actions and selected emphasis |
| background | `rgb(251, 251, 248)` | Page canvas |
| surface | `rgb(251, 251, 248)` | Panels and cards |
| foreground | `oklch(0.21 0.006 285.885)` | Primary text |
| muted | `oklch(0.552 0.016 285.938)` | Supporting text |
| border | `oklab(0 0 0 / 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(255, 175, 1)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | ALTMistral | 96px | 500 | 1 | -0.02em |
| display-mobile | ALTMistral | 28px | 500 | 1.43 | -0.01em |
| heading | ALTMistral | 44px | 500 | 1.18 | -0.01em |
| body | ALTMistral | 16px | 500 | 1.5 | 0em |
| action | ALTMistral | 16px | 500 | 1.5 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Regular.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Regular.woff") format("woff"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Italic.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Italic.woff") format("woff"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Medium.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Medium.woff") format("woff"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-MediumItalic.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-MediumItalic.woff") format("woff"); font-weight: 500; font-style: italic; font-display: swap; }
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Semibold.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Semibold.woff") format("woff"); font-weight: 600; font-style: normal; font-display: swap; }
@font-face { font-family: ALTMistral; src: url("https://mistral.ai/fonts/alt-mistral/ALTMistral-SemiboldItalic.woff2") format("woff2"), url("https://mistral.ai/fonts/alt-mistral/ALTMistral-SemiboldItalic.woff") format("woff"); font-weight: 600; font-style: italic; font-display: swap; }
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Regular.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Regular.woff")format("woff");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Italic.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Italic.woff")format("woff");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Medium.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Medium.woff")format("woff");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-MediumItalic.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-MediumItalic.woff")format("woff");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Semibold.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-Semibold.woff")format("woff");font-weight:600;font-style:normal;font-display:swap}
@font-face{font-family:ALTMistral;src:url("https://mistral.ai/fonts/alt-mistral/ALTMistral-SemiboldItalic.woff2")format("woff2"),url("https://mistral.ai/fonts/alt-mistral/ALTMistral-SemiboldItalic.woff")format("woff");font-weight:600;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Give the homepage introduction broad whitespace above a stepped pixel landscape and a tightly divided customer strip. The product route organizes large colored demonstration tiles in a two-column grid with smaller supporting modules. Mobile stacks the tiles and reduces the pixel motif without losing the strong section boundaries.

Spacing scale: xs 8px, sm 8px, md 16px, lg 24px, xl 24px, section 80px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 49px high, with 0px left and 0px right padding. The sampled nav is static, 48px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `96px` with gap `normal`; `1019px` with gap `normal`; `1019px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `1728px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular or modestly rounded actions, small product badges, thin outlines and clear panel edges. Keep block-like pixel geometry distinct from functional controls and avoid turning every container into a pill.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses pixel characters, stepped landscapes and product demonstrations. Create original pixel geometry and generic AI-workflow diagrams without copying characters, logos, illustrations or screenshots.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, technical and confident, with concise product and deployment descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
