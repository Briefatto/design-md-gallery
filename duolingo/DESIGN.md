---
version: alpha
name: "Duolingo"
description: "Duolingo's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Duolingo."
colors:
  primary: "rgb(88, 204, 2)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(75, 75, 75)"
  muted: "rgb(119, 119, 119)"
  border: "rgb(229, 229, 229)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'duolingo-sans, sans-serif'
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'duolingo-sans, sans-serif'
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: 'feather, sans-serif'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: 'duolingo-sans, sans-serif'
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.41
    letterSpacing: 0em
  action:
    fontFamily: 'duolingo-sans, sans-serif'
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0.053em
rounded:
  control: 12px
  card: 12px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 70px
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

# Duolingo DESIGN.md

## Overview

A playful learning interface uses lively accent color, bold approachable type, and tactile controls with clear action hierarchy.

Built from [/](https://www.duolingo.com/) and [/super](https://www.duolingo.com/super), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(88, 204, 2)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(75, 75, 75)` | Primary text |
| muted | `rgb(119, 119, 119)` | Supporting text |
| border | `rgb(229, 229, 229)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

The homepage uses white surfaces, bright green emphasis, and dark gray reading text. Super marketing uses a separate deep-navy world with white type and spectral green/blue/purple artwork; the portable preview follows the main light site. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | duolingo-sans | 32px | 700 | 1.2 | 0em |
| display-mobile | duolingo-sans | 32px | 700 | 1.2 | 0em |
| heading | feather | 48px | 700 | 1.2 | 0em |
| body | duolingo-sans | 17px | 400 | 1.41 | 0em |
| action | duolingo-sans | 15px | 700 | 1.2 | 0.053em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-family: "duolingo-sans"; src: url("https://d35aaqx5ub95lt.cloudfront.net/vendor/f2331bbfd902cdf8971c4d3184a44283.woff2") format("woff2"); font-style: normal; font-weight: 100 900; }
@font-face { font-family: "duolingo-sans"; src: url("https://d35aaqx5ub95lt.cloudfront.net/vendor/3bbe299f41d8289a47d91773fee0cb6a.woff2") format("woff2"); font-style: italic; font-weight: 100 900; }
@font-face { font-family: "feather"; src: url("https://d35aaqx5ub95lt.cloudfront.net/vendor/68d22534874c554b0c9ebabea379fc60.woff2") format("woff2"); font-style: normal; font-weight: 700; }
@font-face { font-family: "feather"; src: url("https://d35aaqx5ub95lt.cloudfront.net/vendor/f2331bbfd902cdf8971c4d3184a44283.woff2") format("woff2"); font-style: normal; font-weight: 900; }
```

The full fallback stacks are in the front matter.

## Layout

Balance a friendly visual introduction with a compact text block. Group account and learning actions and keep later sections easy to scan.

Spacing scale: xs 3px, sm 8px, md 16px, lg 24px, xl 32px, section 70px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 900px high, with 0px left and 0px right padding. The sampled nav is static, 70px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `14px 1002px 14px` with gap `30px`; `22px 916px 22px` with gap `22px`. Build them as a fluid grid. Sampled container maximum widths: `988px`, `1090px`, `480px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use substantial rounded actions, clear outlines, friendly feature blocks, and consistent icon proportions. The primary homepage action has a visible lower edge that gives it a tactile pressable quality; keep that restrained depth distinct from a soft floating shadow.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 50px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original simple illustrations with rounded geometry; never reproduce the mascot or character artwork.

**Motion.** Observed CSS transition declarations include `filter 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Encouraging, energetic, and easy to understand.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
