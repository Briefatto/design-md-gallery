---
version: alpha
name: "Cloudflare"
description: "Cloudflare's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Cloudflare."
colors:
  primary: "rgb(255, 112, 56)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(253, 253, 252)"
  foreground: "rgb(31, 31, 31)"
  muted: "oklab(0.268617 0.000012286 0.00000536442 / 0.7)"
  border: "oklab(0.268617 0.000012286 0.00000536442 / 0.1)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: '"STK Bureau Sans", sans-serif'
    fontSize: 56px
    fontWeight: 500
    lineHeight: 0.99
    letterSpacing: -0.025em
  display-mobile:
    fontFamily: '"STK Bureau Sans", sans-serif'
    fontSize: 40px
    fontWeight: 600
    lineHeight: 0.99
    letterSpacing: -0.025em
  heading:
    fontFamily: '"STK Bureau Sans", sans-serif'
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  body:
    fontFamily: '"STK Bureau Sans", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.002em
  action:
    fontFamily: '"STK Bureau Sans", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: -0.02em
rounded:
  control: 33554400px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 72px
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

# Cloudflare DESIGN.md

## Overview

A modern infrastructure site uses clean white surfaces, medium-weight geometric headlines, a vivid orange introductory field, and faint technical grid framing. Dense product information stays quiet and highly structured.

Built from [/](https://www.cloudflare.com/) and [/plans/](https://www.cloudflare.com/plans/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 112, 56)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(253, 253, 252)` | Panels and cards |
| foreground | `rgb(31, 31, 31)` | Primary text |
| muted | `oklab(0.268617 0.000012286 0.00000536442 / 0.7)` | Supporting text |
| border | `oklab(0.268617 0.000012286 0.00000536442 / 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "STK Bureau Sans" | 56px | 500 | 0.99 | -0.025em |
| display-mobile | "STK Bureau Sans" | 40px | 600 | 0.99 | -0.025em |
| heading | "STK Bureau Sans" | 32px | 500 | 1 | -0.025em |
| body | "STK Bureau Sans" | 16px | 400 | 1.2 | -0.002em |
| action | "STK Bureau Sans" | 14px | 400 | 1.14 | -0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "STK Bureau Sans"; src: url("https://www.cloudflare.com/fonts/STKBureauSans-Book.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "STK Bureau Sans"; src: url("https://www.cloudflare.com/fonts/STKBureauSans-Book-Italic.otf") format("opentype"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: "STK Bureau Sans"; src: url("https://www.cloudflare.com/fonts/STKBureauSans-Regular.otf") format("opentype"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face{font-family:STK Bureau Sans;src:url("https://www.cloudflare.com/fonts/STKBureauSans-Book.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:STK Bureau Sans;src:url("https://www.cloudflare.com/fonts/STKBureauSans-Book-Italic.otf")format("opentype");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:STK Bureau Sans;src:url("https://www.cloudflare.com/fonts/STKBureauSans-Regular.otf")format("opentype");font-weight:500;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a compact header, a broad orange hero, and generous white reading chapters aligned to faint grid lines. Pricing uses a centered introduction, a compact category selector, four comparable desktop plans, and a long factual comparison table; mobile stacks the plans.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 72px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 72px high, with 0px left and 0px right padding. The sampled nav is relative, 36px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `453.359px 477.266px 453.375px` with gap `12px`; `399.328px 399.328px 399.344px` with gap `normal`; `746px 160px` with gap `24px 48px`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `1080px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.2) 1px 6px 6px 0px inset, rgba(255, 255, 255, 0.35) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0.02) 0px 4px 12px 0px, rgba(0, 0, 0, 0.02) 0px 0px 0px 0px, rgba(0, 0, 0, 0.03) 0px 2px 12px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `16px`. Treat the very large computed control radius as a full-pill strategy, not an element size. Small content panels use a quieter shape, while the large framing grid remains visually open.

## Components

Use pill-like actions, a contrasting white action on the orange hero, compact orange active selectors, and restrained plan panels. Keep fine grid and separator treatments lighter than the text hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 50px, horizontal padding 24px / 24px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original abstract network diagrams, point grids, and restrained technical illustrations. The orange atmosphere can be suggested with original CSS geometry; do not reproduce maps, product screens, or the cloud mark.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.3s`, `width, color, background-color, border-color, transform, translate 0.3s`, `border-color, color 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, factual, and explicit about the next step.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

