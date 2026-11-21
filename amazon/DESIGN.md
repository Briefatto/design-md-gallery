---
version: alpha
name: "Amazon"
description: "Amazon's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Amazon."
colors:
  primary: "rgb(255, 216, 20)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(243, 243, 243)"
  foreground: "rgb(15, 17, 17)"
  muted: "rgb(86, 89, 89)"
  border: "rgb(213, 217, 217)"
  on-primary: "rgb(15, 17, 17)"
typography:
  display:
    fontFamily: 'Arial, sans-serif'
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.22
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Arial, sans-serif'
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.22
    letterSpacing: 0em
  heading:
    fontFamily: '"Amazon Ember Modern Display", "Amazon Ember", Arial, sans-serif'
    fontSize: 31.5447px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'Arial, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  action:
    fontFamily: 'Arial, sans-serif'
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.46
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 31.5px
  section: 31.5px
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

# Amazon DESIGN.md

## Overview

A retail interface prioritizes search, browsing density, and fast access to useful product information.

Built from [/](https://www.amazon.com/) and [/amazonprime](https://www.amazon.com/amazonprime), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 216, 20)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(243, 243, 243)` | Panels and cards |
| foreground | `rgb(15, 17, 17)` | Primary text |
| muted | `rgb(86, 89, 89)` | Supporting text |
| border | `rgb(213, 217, 217)` | Quiet separators and outlines |
| on-primary | `rgb(15, 17, 17)` | Text on the primary action |

Use yellow for priority actions, dark ink for retail reading text, and white for product groupings. The captured holiday campaign temporarily turns the header and hero orange; Prime adds a distinct blue feature world. Treat these campaign surfaces as separate contexts. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Arial | 36px | 700 | 1.22 | 0em |
| display-mobile | Arial | 36px | 700 | 1.22 | 0em |
| heading | "Amazon Ember Modern Display" | 31.5447px | 700 | 1 | 0em |
| body | Arial | 14px | 400 | 1.2 | 0em |
| action | Arial | 13px | 400 | 1.46 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face{font-family:'Amazon Ember Modern Display';src:url("https://m.media-amazon.com/images/S/sash/kIK54mwNKcOchue.woff2") format("woff2");font-weight:700}
@font-face{font-family:'Amazon Ember Modern Display';src:url("https://m.media-amazon.com/images/S/sash/XtYPxL00dpeeCh-.woff2") format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Keep the navigation/search band compact and highly visible. Use repeated merchandising sections and consistent gutters rather than a sparse editorial layout.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 31.5px, section 31.5px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 99px high, with 0px left and 0px right padding. The sampled nav is fixed, 111px high, with 20px left and 20px right padding.

Measured desktop grid tracks: `117.656px 117.672px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `420px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use practical search fields, compact action buttons, category links, and cards that separate imagery from factual metadata.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 38px, radius 8px, background rgba(0, 0, 0, 0), and border 0px rgb(17, 17, 17). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use licensed product photography and simple utility icons; do not copy product listings or site imagery.

**Motion.** Observed CSS transition declarations include `all 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Concrete, transactional, and focused on choices and outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
