---
version: alpha
name: "Appwrite"
description: "Appwrite's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Appwrite."
colors:
  primary: "rgb(253, 54, 110)"
  background: "rgb(25, 25, 28)"
  surface: "oklab(0.214707 0.00160658 -0.00560202 / 0.9)"
  foreground: "lab(98.26 0 0)"
  muted: "lab(65.6464 1.53497 -5.42429)"
  border: "rgb(45, 45, 49)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Aeonik Pro", -apple-system, "system-ui", "Segoe UI", Roboto, sans-serif'
    fontSize: 76px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.022em
  display-mobile:
    fontFamily: '"Aeonik Pro", -apple-system, "system-ui", "Segoe UI", Roboto, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.022em
  heading:
    fontFamily: '"Aeonik Pro", -apple-system, "system-ui", "Segoe UI", Roboto, sans-serif'
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.025em
  body:
    fontFamily: '-apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: 0em
  action:
    fontFamily: '-apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 8px
  card: 14px
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

# Appwrite DESIGN.md

## Overview

A developer cloud site combines a charcoal canvas, light Aeonik Pro typography, vivid pink emphasis, fine point-grid atmosphere, and quiet dark product panels. Its hierarchy feels technical without becoming visually dense.

Built from [/](https://appwrite.io/) and [/pricing](https://appwrite.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(253, 54, 110)` | Priority actions and selected emphasis |
| background | `rgb(25, 25, 28)` | Page canvas |
| surface | `oklab(0.214707 0.00160658 -0.00560202 / 0.9)` | Panels and cards |
| foreground | `lab(98.26 0 0)` | Primary text |
| muted | `lab(65.6464 1.53497 -5.42429)` | Supporting text |
| border | `rgb(45, 45, 49)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Use light neutral text on charcoal and pink for the main action and selected headline emphasis. Do not turn all reading text pink; the highlighted words and action surfaces carry the accent while long-form content stays neutral. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Aeonik Pro" | 76px | 400 | 1.04 | -0.022em |
| display-mobile | "Aeonik Pro" | 48px | 400 | 1.04 | -0.022em |
| heading | "Aeonik Pro" | 44px | 400 | 1 | -0.025em |
| body | -apple-system | 14px | 400 | 1.71 | 0em |
| action | -apple-system | 13px | 500 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Aeonik Pro;font-style:normal;font-weight:400;font-display:swap;src:local(Aeonik Pro),local(AeonikPro),url("https://cdn.appwrite.io/assets/AeonikPro-Regular-BkHrzXoz.woff2")format("woff2")}
@font-face{font-family:Aeonik Pro;font-style:normal;font-weight:500;font-display:swap;src:local(Aeonik Pro),local(AeonikPro),url("https://cdn.appwrite.io/assets/AeonikPro-Medium-BqHv4pGd.woff2")format("woff2")}
@font-face{font-family:Aeonik Pro;font-style:normal;font-weight:600;font-display:swap;src:local(Aeonik Pro),local(AeonikPro),url("https://cdn.appwrite.io/assets/AeonikPro-Bold-CS4_Sbsv.woff2")format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Use a centered introduction, grouped project/documentation actions, and a wide product demonstration below. Pricing repeats the same dark atmosphere with aligned plan columns, a subtly emphasized featured tier, and stacked mobile plans.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 56px high, with 16px left and 24px right padding. The sampled nav is static, 36px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `375.547px 632.906px 375.547px` with gap `8px`; `307.5px 307.5px 307.5px 307.5px` with gap `normal`; `375.547px 632.906px 375.547px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `1152px`, `1024px`, `768px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `14px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rounded actions, subtle dark borders, softly rounded product frames, small status chips, and clearly grouped plan details. Keep glow and pink emphasis selective.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 12px / 12px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original architecture diagrams and functional icons; avoid copying dashboards or branded graphics.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `all 0.15s`, `opacity, transform 0.2s`, `background-color, box-shadow 0.78s, 0.78s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, practical, and specific to developer tasks.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
