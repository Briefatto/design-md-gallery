---
version: alpha
name: "Nothing"
description: "Nothing's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Nothing."
colors:
  primary: "rgb(4, 4, 4)"
  background: "rgb(244, 244, 244)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(4, 4, 4)"
  muted: "rgb(89, 90, 90)"
  border: "rgb(216, 217, 217)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'NType82-Regular, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'NType82-Regular, sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  heading:
    fontFamily: 'NType82-Regular, sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: '"Geist Mono Variable", monospace'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  action:
    fontFamily: '"Geist Mono Variable", monospace'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
rounded:
  control: 4px
  card: 8px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 16px
  xl: 40px
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

# Nothing DESIGN.md

## Overview

A consumer technology presentation pairs NType82 editorial serif headings with dot-matrix technical labels, pale gray surfaces, and large studio product compositions. Black and white form the reusable interface; a saturated yellow appears in the captured region-selection controls.

Built from [/](https://nothing.tech/) and [/products/phone-4a-pro](https://nothing.tech/products/phone-4a-pro), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(4, 4, 4)` | Priority actions and selected emphasis |
| background | `rgb(244, 244, 244)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(4, 4, 4)` | Primary text |
| muted | `rgb(89, 90, 90)` | Supporting text |
| border | `rgb(216, 217, 217)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | NType82-Regular | 48px | 400 | 1 | 0em |
| display-mobile | NType82-Regular | 32px | 400 | 1 | 0em |
| heading | NType82-Regular | 32px | 400 | 1 | 0em |
| body | "Geist Mono Variable" | 14px | 400 | 1.25 | 0em |
| action | "Geist Mono Variable" | 12px | 400 | 1.25 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/X_5orZeX.woff2")format("woff2-variations");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/DiZS0aHC.woff2")format("woff2-variations");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/CO5SzqOn.woff2")format("woff2-variations");unicode-range:U+2000-2001,U+2004-2008,U+200A,U+23B8-23BD,U+2500-259F}
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/DadHysG0.woff2")format("woff2-variations");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/Bwz-egvJ.woff2")format("woff2-variations");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Geist Mono Variable;font-style:normal;font-display:swap;font-weight:100 900;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/XN7g48iV.woff2")format("woff2-variations");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:NType82-Regular;src:url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/DVQYVosZ.woff2")format("woff2"),url("https://cdn.shopify.com/oxygen-v2/43495/38485/80939/5152537/assets/B472M_4I.woff")format("woff");font-weight:400;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Give broad product photography and sparse promotional headings room. Follow with a category grid, alternating full-width product chapters, compact technical metadata, and a dark information footer. The product page interleaves small editorial tiles with large device details.

Spacing scale: xs 8px, sm 8px, md 16px, lg 16px, xl 40px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 100.156px high, with 8px left and 8px right padding. The sampled nav is static, 22.4062px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px` with gap `8px`; `111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px 111.328px` with gap `8px`; `708px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `58%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use restrained rectangular monochrome actions, compact technical labels, economical navigation, and softly rounded image tiles. Keep the dot-matrix treatment for short utility text and the serif face for editorial hierarchy; do not apply the display texture to long paragraphs.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 48px, radius 4px, background rgba(60, 60, 60, 0.6), and border 0px rgb(229, 231, 235). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original monochrome or neutral studio photography, macro material details, and generic device silhouettes. Precise cutouts can sit on pale fields. Do not reproduce device renders, campaign photographs, portraits, or marks.

**Motion.** Observed CSS transition declarations include `transform 0.501s`, `all 0.2s`, `opacity 0.15s`, `opacity 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Brief, confident, and slightly technical.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
