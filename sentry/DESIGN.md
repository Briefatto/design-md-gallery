---
version: alpha
name: "Sentry"
description: "Sentry's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Sentry."
colors:
  primary: "rgb(255, 255, 255)"
  background: "rgb(31, 22, 51)"
  surface: "rgb(21, 15, 35)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.7)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(31, 22, 51)"
  accent: "rgb(253, 68, 176)"
typography:
  display:
    fontFamily: '"Dammit Sans", sans-serif'
    fontSize: 88px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Dammit Sans", sans-serif'
    fontSize: 50.1901px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: '"Dammit Sans", sans-serif'
    fontSize: 45px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: 0em
  body:
    fontFamily: 'Rubik, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'Rubik, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.014em
rounded:
  control: 8px
  card: 8px
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

# Sentry DESIGN.md

## Overview

A playful monitoring site pairs a deep purple ground with large, heavy display type, bright pink emphasis and lime signals. The pricing route carries the same purple identity into white comparison surfaces.

Built from [/](https://sentry.io/) and [/pricing](https://sentry.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 255, 255)` | Priority actions and selected emphasis |
| background | `rgb(31, 22, 51)` | Page canvas |
| surface | `rgb(21, 15, 35)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.7)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(31, 22, 51)` | Text on the primary action |
| accent | `rgb(253, 68, 176)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Dammit Sans" | 88px | 700 | 1.2 | 0em |
| display-mobile | "Dammit Sans" | 50.1901px | 500 | 1.2 | 0em |
| heading | "Dammit Sans" | 45px | 700 | 1.15 | 0em |
| body | Rubik | 16px | 400 | 1.5 | 0em |
| action | Rubik | 14px | 500 | 1 | 0.014em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Rubik;font-style:normal;font-weight:400;font-display:swap;src:url("https://sentry.io/astro-assets/fonts/rubik-latin-regular.woff2")format("woff2"),url("https://sentry.io/astro-assets/fonts/rubik-latin-regular.woff")format("woff");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Rubik;font-style:normal;font-weight:500;font-display:swap;src:url("https://sentry.io/astro-assets/fonts/rubik-latin-500.woff2")format("woff2"),url("https://sentry.io/astro-assets/fonts/rubik-latin-500.woff")format("woff");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Rubik;font-style:normal;font-weight:700;font-display:swap;src:url("https://sentry.io/astro-assets/fonts/rubik-latin-500.woff2")format("woff2"),url("https://sentry.io/astro-assets/fonts/rubik-latin-500.woff")format("woff");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Rubik;font-style:italic;font-weight:400;font-display:swap;src:url("https://sentry.io/astro-assets/fonts/rubik-latin-italic.woff2")format("woff2"),url("https://sentry.io/astro-assets/fonts/rubik-latin-italic.woff")format("woff");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Rubik;font-style:italic;font-weight:500;font-display:swap;src:url("https://sentry.io/astro-assets/fonts/rubik-latin-500italic.woff2")format("woff2"),url("https://sentry.io/astro-assets/fonts/rubik-latin-500italic.woff")format("woff");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Dammit Sans;src:url("https://sentry.io/astro-assets/fonts/dammitsansv0.3-bold.otf")format("opentype");font-weight:700;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage hero above a large illustrated product scene. Follow with broad feature bands and alternating demonstrations. Desktop pricing has aligned white plan cards, while mobile replaces the card row with a compact comparison grid and stacked content.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 72px high, with 0px left and 0px right padding. The sampled nav is static, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `520px 520px` with gap `48px`; `218.703px` with gap `20px normal`; `218.703px` with gap `20px normal`. Build them as a fluid grid. Sampled container maximum widths: `60%`, `1152px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.15) 0px 2px 10px 0px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small uppercase actions, modest rounded corners, thin outlines and vivid announcement chips. Keep the expressive hero distinct from the practical plan comparison, feature checks and billing toggle.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 16px / 16px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 42px, radius 6px, background rgb(255, 255, 255), and border 1px rgb(207, 207, 219). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses illustrated characters, cosmic textures and small neon product panels. Use original abstract technical scenes and simple icons; do not reproduce characters, wordmarks or screenshots.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`, `all 0.2s`, `background-position, outline-width 0.2s, 0.2s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Conversational, humorous and developer-aware, with clear practical labels for plans and monitoring features.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
