---
version: alpha
name: "Glean"
description: "Glean's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Glean."
colors:
  primary: "rgb(52, 60, 237)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(251, 246, 244)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(111, 111, 111)"
  border: "rgb(216, 217, 222)"
  on-primary: "rgb(254, 254, 254)"
  accent: "rgb(216, 253, 73)"
typography:
  display:
    fontFamily: '"Polysans Neutral", Arial, sans-serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 0.96
    letterSpacing: -0.043em
  display-mobile:
    fontFamily: '"Polysans Neutral", Arial, sans-serif'
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  heading:
    fontFamily: '"Polysans Neutral", Arial, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.04em
  body:
    fontFamily: '"Polysans Neutral", Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: '"Polysans Neutral", Arial, sans-serif'
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
rounded:
  control: 64px
  card: 10px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 24px
  section: 52px
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

# Glean DESIGN.md

## Overview

An enterprise AI site combines tightly tracked Polysans display type, bright blue actions, pale editorial surfaces and vivid abstract product imagery. Lime signals and precise technical diagrams add selective emphasis.

Built from [/](https://glean.com/) and [/platform](https://glean.com/platform), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(52, 60, 237)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(251, 246, 244)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(111, 111, 111)` | Supporting text |
| border | `rgb(216, 217, 222)` | Quiet separators and outlines |
| on-primary | `rgb(254, 254, 254)` | Text on the primary action |
| accent | `rgb(216, 253, 73)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Polysans Neutral" | 56px | 400 | 0.96 | -0.043em |
| display-mobile | "Polysans Neutral" | 28px | 400 | 1 | -0.02em |
| heading | "Polysans Neutral" | 40px | 400 | 1.04 | -0.04em |
| body | "Polysans Neutral" | 16px | 400 | 1.4 | 0em |
| action | "Polysans Neutral" | 24px | 400 | 1.25 | -0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Polysans Neutral"; src: url("https://cdn.prod.website-files.com/6127a84dfe068e153ef20572/66b4a66d22e2c49832621144_PolySans-Neutral.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "Polysans Neutral"; src: url("https://cdn.prod.website-files.com/6127a84dfe068e153ef20572/698a0f27df2a85d9811bdee0_PolySans%20Neutral%20Italic.woff") format("woff"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face{font-family:Polysans Neutral;src:url("https://cdn.prod.website-files.com/6127a84dfe068e153ef20572/66b4a66d22e2c49832621144_PolySans-Neutral.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Polysans Neutral;src:url("https://cdn.prod.website-files.com/6127a84dfe068e153ef20572/698a0f27df2a85d9811bdee0_PolySans%20Neutral%20Italic.woff")format("woff");font-weight:400;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction and paired actions above a large search demonstration framed by colorful media. The platform route introduces a compact title above a broad architecture diagram and repeated feature sections. Mobile stacks the diagram modules and retains a narrow reading flow.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 24px, section 52px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 124.891px high, with 0px left and 0px right padding. The sampled header is relative, 68.7969px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `312px 312px 312px 312px` with gap `0px`; `587px` with gap `48px`; `564px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `560px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `64px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use blue pill actions, quiet text companions, rounded search fields, small technical labels, fine section rules and restrained product cards. Keep dense architecture modules distinct from the more spacious marketing introduction.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 43.1875px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(10, 2, 39). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source combines luminous abstract textures, search demonstrations and technical architecture diagrams. Create original textures and generic enterprise-workflow diagrams without copying screenshots, artwork or integration marks.

**Motion.** Observed CSS transition declarations include `all 0.6s`, `opacity, transform, visibility 0.25s, 0.25s, 0.25s`, `background-color 0.2s`, `transform, color, background-color, stroke, stroke-width 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, confident and practical, with precise enterprise context, search and workflow terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
