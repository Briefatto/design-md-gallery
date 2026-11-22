---
version: alpha
name: "Synthesia"
description: "Synthesia's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Synthesia."
colors:
  primary: "rgb(9, 11, 34)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 247, 247)"
  foreground: "rgb(9, 11, 34)"
  muted: "rgb(104, 104, 106)"
  border: "rgb(218, 218, 221)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(62, 87, 218)"
typography:
  display:
    fontFamily: '"Basiersquare Webfont", sans-serif'
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.055em
  display-mobile:
    fontFamily: '"Basiersquare Webfont", sans-serif'
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.05em
  heading:
    fontFamily: '"Basiersquare Webfont", sans-serif'
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.05em
  body:
    fontFamily: '"Basiersquare Webfont", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
  action:
    fontFamily: '"Basiersquare Webfont", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
rounded:
  control: 8px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 18px
  xl: 32px
  section: 56px
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

# Synthesia DESIGN.md

## Overview

A business video platform uses deep navy typography, bright white surfaces, gently rounded controls and vivid media demonstrations. Blue and lavender gradients identify selected pricing tiers while the general interface remains restrained.

Built from [/](https://synthesia.io/) and [/pricing](https://synthesia.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(9, 11, 34)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 247, 247)` | Panels and cards |
| foreground | `rgb(9, 11, 34)` | Primary text |
| muted | `rgb(104, 104, 106)` | Supporting text |
| border | `rgb(218, 218, 221)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(62, 87, 218)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Basiersquare Webfont" | 56px | 500 | 1 | -0.055em |
| display-mobile | "Basiersquare Webfont" | 44px | 500 | 1.05 | -0.05em |
| heading | "Basiersquare Webfont" | 44px | 500 | 1.05 | -0.05em |
| body | "Basiersquare Webfont" | 16px | 400 | 1.38 | -0.01em |
| action | "Basiersquare Webfont" | 16px | 400 | 1.38 | -0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Basiersquare Webfont"; src: url("https://cdn.prod.website-files.com/65e89895c5a4b8d764c0d710/65e89895c5a4b8d764c0e21d_6527f9cf2cfe9fad38bd66bc_basiersquare-regular-webfont.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "Basiersquare Webfont"; src: url("https://cdn.prod.website-files.com/65e89895c5a4b8d764c0d710/65e89895c5a4b8d764c0e21e_6527f9cf2cfe9fad38bd66bd_basiersquare-medium-webfont.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face{font-family:Basiersquare Webfont;src:url("https://cdn.prod.website-files.com/65e89895c5a4b8d764c0d710/65e89895c5a4b8d764c0e21d_6527f9cf2cfe9fad38bd66bc_basiersquare-regular-webfont.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Basiersquare Webfont;src:url("https://cdn.prod.website-files.com/65e89895c5a4b8d764c0d710/65e89895c5a4b8d764c0e21e_6527f9cf2cfe9fad38bd66bd_basiersquare-medium-webfont.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction over a large prompt-entry panel and a wide media gallery. Pricing places audience and billing controls above a multi-column comparison with distinct plan summaries and feature groups; mobile keeps horizontally browsable plans.

Spacing scale: xs 4px, sm 8px, md 16px, lg 18px, xl 32px, section 56px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is sticky, 72px high, with 0px left and 0px right padding. The sampled nav is relative, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `592px 592px` with gap `0px 32px`; `592px 592px` with gap `0px 32px`; `592px 592px` with gap `0px 32px`. Build them as a fluid grid. Sampled container maximum widths: `1216px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(16, 24, 40, 0.08) 0px 2px 10px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use navy filled actions, quiet outlined companions, spacious rounded prompt fields, small suggestion chips, segmented selectors and softly bordered pricing panels. Credit summaries and feature groups use subtle inset surfaces rather than heavy shadows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 38px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses video, avatar demonstrations and colorful media tiles. Use original licensed media and generic video-interface diagrams without copying people, recordings, avatars, screenshots or customer marks.

**Motion.** Observed CSS transition declarations include `background-color, box-shadow, top 0.3s`, `filter 0.1s`, `box-shadow, background-color 0.2s, 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, helpful and business-oriented, with concise creation and plan-selection labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
