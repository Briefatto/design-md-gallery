---
version: alpha
name: "Bun"
description: "Bun's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Bun."
colors:
  primary: "rgb(255, 31, 143)"
  background: "rgb(255, 255, 255)"
  surface: "rgba(246, 246, 246, 0.6)"
  foreground: "rgb(10, 10, 10)"
  muted: "rgb(112, 112, 112)"
  border: "rgb(226, 226, 226)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(255, 31, 143)"
typography:
  display:
    fontFamily: 'Archivo, "Archivo X Fallback", ui-sans-serif, system-ui, sans-serif'
    fontSize: 76.2917px
    fontWeight: 900
    lineHeight: 0.94
    letterSpacing: -0.015em
  display-mobile:
    fontFamily: 'Archivo, "Archivo X Fallback", ui-sans-serif, system-ui, sans-serif'
    fontSize: 49.7px
    fontWeight: 900
    lineHeight: 0.94
    letterSpacing: -0.015em
  heading:
    fontFamily: 'Archivo, "Archivo Fallback", ui-sans-serif, system-ui, sans-serif'
    fontSize: 41.6px
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: -0.02em
  body:
    fontFamily: 'ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif'
    fontSize: 17.92px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
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

# Bun DESIGN.md

## Overview

A high-contrast developer site combines oversized, tightly packed condensed display type, hot pink accents, square controls and black terminal panels. The playful hero becomes a disciplined documentation interface on the second route.

Built from [/](https://bun.sh/) and [/docs](https://bun.sh/docs), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 31, 143)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgba(246, 246, 246, 0.6)` | Panels and cards |
| foreground | `rgb(10, 10, 10)` | Primary text |
| muted | `rgb(112, 112, 112)` | Supporting text |
| border | `rgb(226, 226, 226)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(255, 31, 143)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Archivo | 76.2917px | 900 | 0.94 | -0.015em |
| display-mobile | Archivo | 49.7px | 900 | 0.94 | -0.015em |
| heading | Archivo | 41.6px | 800 | 0.92 | -0.02em |
| body | ui-sans-serif | 17.92px | 500 | 1.5 | 0em |
| action | ui-sans-serif | 12px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Archivo; font-style: normal; font-weight: 800 900; font-stretch: 62% 75%; font-display: swap; src: url("https://bun.sh/fonts/Archivo-display.core.woff2") format("woff2"); unicode-range: U+20-7E, U+A0, U+B7, U+D7, U+2013-2014, U+2018-2019, U+201C-201D, U+2022, U+2026, U+2191, U+2193, U+2212; }
@font-face { font-family: Archivo; font-style: normal; font-weight: 800 900; font-stretch: 62% 75%; font-display: swap; src: url("https://bun.sh/fonts/Archivo-display.ext.woff2") format("woff2"); unicode-range: U+A1-B6, U+B8-D6, U+D8-36F, U+201A, U+201E, U+2032-2044, U+20AC, U+2122, U+2215; }
@font-face { font-family: Archivo; font-style: italic; font-weight: 800 900; font-stretch: 62% 75%; font-display: swap; src: url("https://bun.sh/fonts/Archivo-display-italic.core.woff2") format("woff2"); unicode-range: U+20-7E, U+A0, U+B7, U+D7, U+2013-2014, U+2018-2019, U+201C-201D, U+2022, U+2026, U+2191, U+2193, U+2212; }
@font-face { font-family: Archivo; font-style: italic; font-weight: 800 900; font-stretch: 62% 75%; font-display: swap; src: url("https://bun.sh/fonts/Archivo-display-italic.ext.woff2") format("woff2"); unicode-range: U+A1-B6, U+B8-D6, U+D8-36F, U+201A, U+201E, U+2032-2044, U+20AC, U+2122, U+2215; }
@font-face{font-family:Archivo;font-style:normal;font-weight:800 900;font-stretch:62% 75%;font-display:swap;src:url("https://bun.sh/fonts/Archivo-display.core.woff2")format("woff2");unicode-range:U+20-7e,U+a0,U+b7,U+d7,U+2013-2014,U+2018-2019,U+201c-201d,U+2022,U+2026,U+2191,U+2193,U+2212}
@font-face{font-family:Archivo;font-style:normal;font-weight:800 900;font-stretch:62% 75%;font-display:swap;src:url("https://bun.sh/fonts/Archivo-display.ext.woff2")format("woff2");unicode-range:U+a1-b6,U+b8-d6,U+d8-36f,U+201a,U+201e,U+2032-2044,U+20ac,U+2122,U+2215}
@font-face{font-family:Archivo;font-style:italic;font-weight:800 900;font-stretch:62% 75%;font-display:swap;src:url("https://bun.sh/fonts/Archivo-display-italic.core.woff2")format("woff2");unicode-range:U+20-7e,U+a0,U+b7,U+d7,U+2013-2014,U+2018-2019,U+201c-201d,U+2022,U+2026,U+2191,U+2193,U+2212}
@font-face{font-family:Archivo;font-style:italic;font-weight:800 900;font-stretch:62% 75%;font-display:swap;src:url("https://bun.sh/fonts/Archivo-display-italic.ext.woff2")format("woff2");unicode-range:U+a1-b6,U+b8-d6,U+d8-36f,U+201a,U+201e,U+2032-2044,U+20ac,U+2122,U+2215}
```

The full fallback stacks are in the front matter.

## Layout

Use an asymmetric two-column hero with copy and installation commands beside a large graphic and benchmark panel. Documentation introduces a left navigation rail, a horizontal tool strip and a generous reading column; mobile collapses the rail and stacks feature cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 65px high, with 0px left and 0px right padding. The sampled nav is static, 33.75px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `431.078px 525.734px` with gap `normal`; `431.078px 525.734px` with gap `normal`; `431.078px 525.734px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `677.16px`, `498.96px`, `533.384px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Favor square filled pink actions, black command strips, outlined search fields, tabbed benchmark panels and thin-bordered documentation cards. Keep large headlines dense while body copy remains open and readable.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 20px / 20px, and gap 10px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Bold concentric pink geometry and a mascot carry the homepage illustration. Use original geometric motion motifs rather than copying the mascot, wordmark or benchmark artwork.

**Motion.** Observed CSS transition declarations include `background, color, box-shadow 0.15s`, `top 0.2s`, `opacity, transform 0.6s, 0.6s`, `transform 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Energetic, technical and direct, with short imperative actions and clear explanations.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
