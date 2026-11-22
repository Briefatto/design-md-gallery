---
version: alpha
name: "Astro"
description: "Astro's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Astro."
colors:
  primary: "rgb(255, 255, 255)"
  background: "rgb(6, 9, 19)"
  surface: "rgb(23, 25, 30)"
  foreground: "rgb(242, 246, 250)"
  muted: "rgb(139, 144, 157)"
  border: "rgb(52, 56, 65)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(184, 69, 237)"
typography:
  display:
    fontFamily: 'Obviously, obviously-fallback, system-ui, sans-serif'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Obviously, obviously-fallback, system-ui, sans-serif'
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0em
  heading:
    fontFamily: 'Obviously, obviously-fallback, system-ui, sans-serif'
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
    letterSpacing: 0em
  body:
    fontFamily: 'ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 9999px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 48px
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

# Astro DESIGN.md

## Overview

A developer framework site pairs a dark foundation with luminous purple gradients and bold, friendly Obviously headlines. Pale actions and technical command strips sit within broad, carefully spaced sections.

Built from [/](https://astro.build/) and [/themes/](https://astro.build/themes/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 255, 255)` | Priority actions and selected emphasis |
| background | `rgb(6, 9, 19)` | Page canvas |
| surface | `rgb(23, 25, 30)` | Panels and cards |
| foreground | `rgb(242, 246, 250)` | Primary text |
| muted | `rgb(139, 144, 157)` | Supporting text |
| border | `rgb(52, 56, 65)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(184, 69, 237)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Obviously | 48px | 700 | 1.1 | 0em |
| display-mobile | Obviously | 30px | 700 | 1.1 | 0em |
| heading | Obviously | 24px | 700 | 1.33 | 0em |
| body | ui-sans-serif | 16px | 300 | 1.5 | 0em |
| action | ui-sans-serif | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Obviously; src: url("https://astro.build/fonts/Obviously.woff2?v=1") format("woff2-variations"); font-style: normal; font-display: swap; font-weight: 100 1000; }
@font-face{font-family:Obviously;src:url("https://astro.build/fonts/Obviously.woff2?v=1")format("woff2-variations");src:url("https://astro.build/fonts/Obviously.woff2?v=1") format("woff2") tech("variations");font-style:normal;font-display:swap;font-weight:100 1000;font-stretch:490 620}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction, stack a priority action and installation command, then use a wide social-proof band and alternating feature sections. The themes page introduces a fine background grid and a three-column gallery that becomes a single column on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 80px high, with 0px left and 0px right padding. The sampled nav is static, 80px high, with 32px left and 32px right padding.

Measured desktop grid tracks: `394.656px 394.656px 394.656px` with gap `16px`; `401.656px 401.672px` with gap `normal`; `277.875px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `1280px`, `912.384px`, `1024px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use pill-shaped priority actions and announcement badges, dark code strips, modestly rounded technical panels and theme cards with large previews and quiet metadata. Preserve the contrast between the bright hero and practical dark gallery surfaces.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 40px, radius 8px, background rgb(6, 9, 19), and border 1px rgb(35, 38, 45). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The captured site uses gradient atmosphere, technical diagrams and theme thumbnails. Use original gradient fields and generic interface diagrams, excluding source thumbnails, logos and illustrations.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, -webkit-backdrop-filter, backdrop-filter 0.15s`, `all 0.5s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.3s`, `transform 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Welcoming, concise and technically useful; explain capabilities without crowding the visual hierarchy.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
