---
version: alpha
name: "Ahrefs"
description: "Ahrefs's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Ahrefs."
colors:
  primary: "rgb(255, 136, 0)"
  background: "rgb(58, 87, 252)"
  surface: "rgb(58, 87, 252)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.7)"
  border: "rgba(0, 0, 0, 0.2)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'Ahrefs, sans-serif'
    fontSize: 92px
    fontWeight: 400
    lineHeight: 0.87
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Ahrefs, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 0.92
    letterSpacing: 0em
  heading:
    fontFamily: 'Ahrefs, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'Ahrefs, sans-serif'
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  action:
    fontFamily: 'Ahrefs'
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 0px
  card: 0px
spacing:
  xs: 4px
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

# Ahrefs DESIGN.md

## Overview

A marketing-data site uses a vivid blue foundation, distinctive wide display lettering, orange priority actions and crisp rectangular structure. White comparison panels and dark feature bands provide strong section contrast.

Built from [/](https://ahrefs.com/) and [/pricing](https://ahrefs.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 136, 0)` | Priority actions and selected emphasis |
| background | `rgb(58, 87, 252)` | Page canvas |
| surface | `rgb(58, 87, 252)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.7)` | Supporting text |
| border | `rgba(0, 0, 0, 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Ahrefs | 92px | 400 | 0.87 | 0em |
| display-mobile | Ahrefs | 48px | 400 | 0.92 | 0em |
| heading | Ahrefs | 40px | 400 | 1 | 0em |
| body | Ahrefs | 20px | 400 | 1.2 | 0em |
| action | Ahrefs | 20px | 700 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Ahrefs; font-style: normal; font-weight: 400; font-display: swap; src: url("https://ahrefs.com/assets/fonts/ahrefs_regular.woff2") format("woff2"); }
@font-face { font-family: Ahrefs; font-style: normal; font-weight: 700; font-display: swap; src: url("https://ahrefs.com/assets/fonts/ahrefs_bold.woff2") format("woff2"); }
@font-face{font-family:Ahrefs;font-style:normal;font-weight:400;font-display:swap;src:url("https://ahrefs.com/assets/fonts/ahrefs_regular.woff2") format("woff2")}
@font-face{font-family:Ahrefs;font-style:normal;font-weight:700;font-display:swap;src:url("https://ahrefs.com/assets/fonts/ahrefs_bold.woff2") format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Use a broad left-aligned homepage introduction above a large product demonstration, then alternate explanatory sections and examples. Pricing places its introduction and billing controls on blue above a dense row of white plan columns. Mobile retains horizontally browsable plan comparisons.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 68px high, with 40px left and 40px right padding. The sampled nav is static, 36px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `1440px` with gap `0px`; `869px 109.562px` with gap `24px`; `120px 725px` with gap `24px`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use square orange priority actions, outlined companions, thin plan dividers, compact billing switches and dense feature lists. Keep blue-section text light and white comparison-panel text dark; the portable blue card sample is an editorial adaptation of the wider palette.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 8px / 8px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses analytics demonstrations, colorful technical graphics and small product signals. Create original generic data specimens and diagrams without copying dashboards, source metrics, screenshots, logos or customer marks.

**Motion.** No non-zero transition was exposed in the sampled component styles. Static screenshots do not establish entrance choreography, hover behavior, or video timing. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, practical and data-oriented, with concise capability and usage descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
