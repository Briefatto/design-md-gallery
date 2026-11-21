---
version: alpha
name: "Modal"
description: "Modal's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Modal."
colors:
  primary: "rgb(227, 229, 225)"
  background: "rgb(4, 8, 4)"
  surface: "rgb(24, 24, 24)"
  foreground: "rgb(227, 229, 225)"
  muted: "rgb(168, 171, 166)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(16, 18, 15)"
  accent: "rgb(127, 238, 100)"
typography:
  display:
    fontFamily: '"ABC Diatype", "ABC Diatype Fallback", Arial, ui-sans-serif, system-ui, sans-serif'
    fontSize: 45px
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: '"ABC Diatype", "ABC Diatype Fallback", Arial, ui-sans-serif, system-ui, sans-serif'
    fontSize: 37px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.01em
  heading:
    fontFamily: '"ABC Diatype", "ABC Diatype Fallback", Arial, ui-sans-serif, system-ui, sans-serif'
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.01em
  body:
    fontFamily: '"ABC Diatype", "ABC Diatype Fallback", Arial, ui-sans-serif, system-ui, sans-serif'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.01em
  action:
    fontFamily: '"ABC Diatype", "ABC Diatype Fallback", Arial, ui-sans-serif, system-ui, sans-serif'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: 0.01em
rounded:
  control: 48px
  card: 10px
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

# Modal DESIGN.md

## Overview

An AI compute site uses a near-black green canvas, calm ABC Diatype text, pale priority actions, and a vivid green signal reserved for selected words and technical graphics. Generous negative space keeps the product and resource data readable.

Built from [/](https://modal.com/) and [/pricing](https://modal.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(227, 229, 225)` | Priority actions and selected emphasis |
| background | `rgb(4, 8, 4)` | Page canvas |
| surface | `rgb(24, 24, 24)` | Panels and cards |
| foreground | `rgb(227, 229, 225)` | Primary text |
| muted | `rgb(168, 171, 166)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(16, 18, 15)` | Text on the primary action |
| accent | `rgb(127, 238, 100)` | Selective emphasis in headings, graphics, and small signals |



Use pale neutral text and a pale filled priority action over the dark green-black canvas. Bright green is a selective heading/graphic accent, not the default long-form text color. The small card mirrors that distinction with a neutral button and a highlighted heading phrase. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "ABC Diatype" | 45px | 500 | 1.07 | -0.01em |
| display-mobile | "ABC Diatype" | 37px | 500 | 1.08 | -0.01em |
| heading | "ABC Diatype" | 38px | 500 | 1.16 | -0.01em |
| body | "ABC Diatype" | 15px | 400 | 1.33 | 0.01em |
| action | "ABC Diatype" | 15px | 400 | 1.47 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-regular.BllW8Pd3.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-medium.ghSlPuNU.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-bold.BcUodbYL.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-regular-italic.BPuPCIug.woff2")format("woff2");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-medium-italic.BIMSmTT8.woff2")format("woff2");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-family:ABC Diatype;src:url("https://modal.com/_app/immutable/assets/abc-diatype-bold-italic.DJEB1luV.woff2")format("woff2");font-weight:700;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a centered introduction and a large original geometric/point-field visual, followed by aligned technical product chapters. Pricing repeats the same atmosphere with simple resource sections, clear units, subtle separators, and vertically readable cost lists.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 65px high, with 0px left and 0px right padding. The sampled nav is static, 64px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `423.062px 465.875px 423.062px` with gap `normal`; `35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px` with gap `0px 20px`; `35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px 35.5px` with gap `0px 20px`. Build them as a fluid grid. Sampled container maximum widths: `607.5px`, `403.2px`, `1546px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(4, 8, 4, 0.4) 0px 1px 3px 0px, rgba(4, 8, 4, 0.5) 0px 2px 32px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `48px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small pill-shaped actions, subdued outlined companions, restrained dark information panels, quiet status tags, and readable technical rows. The primary button stays neutral while green provides selective emphasis.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 12px / 12px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original point fields, abstract compute geometry, and clear technical diagrams. Do not reproduce the animated geometric artwork, product screenshots, customer marks, or logo.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `opacity, translate 0.2s`, `color, background-color, border-color, -webkit-backdrop-filter, backdrop-filter 0.2s`, `transform, translate, scale, rotate 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Technical, concise, and explicit about capabilities.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
