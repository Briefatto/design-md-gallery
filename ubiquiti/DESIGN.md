---
version: alpha
name: "Ubiquiti"
description: "Ubiquiti's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Ubiquiti."
colors:
  primary: "rgb(0, 111, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(249, 250, 250)"
  foreground: "rgb(33, 35, 39)"
  muted: "rgb(103, 111, 121)"
  border: "rgb(222, 224, 227)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"UI Sans", Lato, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"UI Sans", Lato, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
    letterSpacing: 0em
  heading:
    fontFamily: '"UI Sans", Lato, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"UI Sans", Lato, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  action:
    fontFamily: '"UI Sans", Lato, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 4px
  card: 15px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 32px
  section: 48px
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

# Ubiquiti DESIGN.md

## Overview

A networking hardware presentation uses clean white fields, UI Sans typography, electric blue interface accents, and highly legible product groupings. Product chapters can switch to dark blue studio settings while preserving a precise, economical UI layer.

Built from [/](https://ui.com/) and [/us/en/cloud-gateways](https://ui.com/us/en/cloud-gateways), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 111, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(249, 250, 250)` | Panels and cards |
| foreground | `rgb(33, 35, 39)` | Primary text |
| muted | `rgb(103, 111, 121)` | Supporting text |
| border | `rgb(222, 224, 227)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "UI Sans" | 42px | 700 | 1.2 | 0em |
| display-mobile | "UI Sans" | 36px | 700 | 1.11 | 0em |
| heading | "UI Sans" | 42px | 700 | 1.2 | 0em |
| body | "UI Sans" | 16px | 400 | 1.25 | 0em |
| action | "UI Sans" | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { src: url("https://ui.com/uicom/fonts/ui-sans-v10-regular.woff2") format("woff2"); font-family: "UI Sans"; font-style: normal; font-weight: normal; }
@font-face { src: url("https://ui.com/uicom/fonts/ui-sans-v10-bold.woff2") format("woff2"); font-family: "UI Sans"; font-style: normal; font-weight: bold; }
@font-face { src: url("https://ui.com/uicom/fonts/ui-sans-v10-light.woff2") format("woff2"); font-family: "UI Sans"; font-style: normal; font-weight: 300; }
```

The full fallback stacks are in the front matter.

## Layout

Use a slim category navigation and centered chapter headings above very large hardware or interface frames. Place compact category pills directly below the title. Continue with spacious product capabilities and aligned device comparison groups; collapse the nav and stack descriptions on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 20px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is absolute, 48px high, with 0px left and 0px right padding. The sampled nav is fixed, 48px high, with 16px left and 16px right padding.

 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.05) 0px -1px 0px 0px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `15px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small blue priority actions, lightly outlined pills, compact product navigation, very subtle gray tile backgrounds, and concise technical labels. Let product imagery carry depth rather than adding heavy interface shadows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 39px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 39px, radius 4px, background rgb(255, 255, 255), and border 1px rgb(219, 220, 225). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original hardware silhouettes, licensed neutral studio photography, or original topology diagrams. Blue technical linework and restrained atmospheric light can support dark product chapters. Never copy device renders, source dashboards, or marks.

**Motion.** Observed CSS transition declarations include `background 0.3s`, `background 0.15s`, `background-color 0.3s`, `background 0.25s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Concise, technical, and product-focused.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

