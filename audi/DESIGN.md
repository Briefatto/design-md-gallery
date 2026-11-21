---
version: alpha
name: "Audi"
description: "Audi's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Audi."
colors:
  primary: "rgb(252, 252, 253)"
  background: "rgb(16, 19, 25)"
  surface: "rgba(24, 29, 37, 0.6)"
  foreground: "rgb(252, 252, 253)"
  muted: "rgba(252, 252, 253, 0.698)"
  border: "rgb(44, 52, 63)"
  on-primary: "rgb(16, 19, 25)"
typography:
  display:
    fontFamily: '"Audi Type Variable", Verdana, Geneva, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Audi Type Variable", Verdana, Geneva, sans-serif'
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
  heading:
    fontFamily: '"Audi Type Variable", Verdana, Geneva, sans-serif'
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  body:
    fontFamily: '"Audi Type Variable", Verdana, Geneva, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Audi Type Variable", Verdana, Geneva, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 999px
  card: 20px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 56px
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

# Audi DESIGN.md

## Overview

A dark automotive editorial language combines monochrome precision, light-weight display typography, large imagery, and disciplined reading blocks.

Built from [/en/](https://www.audi.com/en/) and [/en/technology-235](https://www.audi.com/en/technology-235), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(252, 252, 253)` | Priority actions and selected emphasis |
| background | `rgb(16, 19, 25)` | Page canvas |
| surface | `rgba(24, 29, 37, 0.6)` | Panels and cards |
| foreground | `rgb(252, 252, 253)` | Primary text |
| muted | `rgba(252, 252, 253, 0.698)` | Supporting text |
| border | `rgb(44, 52, 63)` | Quiet separators and outlines |
| on-primary | `rgb(16, 19, 25)` | Text on the primary action; observed ink reassigned for legibility |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Audi Type Variable" | 40px | 400 | 1.5 | 0em |
| display-mobile | "Audi Type Variable" | 28px | 400 | 1.43 | 0em |
| heading | "Audi Type Variable" | 24px | 400 | 1.5 | 0em |
| body | "Audi Type Variable" | 16px | 400 | 1.5 | 0em |
| action | "Audi Type Variable" | 14px | 400 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face{font-family:Audi Type Variable;src:local("_x_"),url("https://static.audi.com/assets/fonts/AudiTypeVF_4.033-EJMP5BQZ.woff2") format("woff2");font-weight:400;font-style:normal;font-stretch:normal}
```

The full fallback stacks are in the front matter.

## Layout

Alternate expansive visual sections with narrower text columns. Give the header room and align feature information to a consistent content edge.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 56px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 72px high, with 96px left and 84px right padding. The sampled nav is static, 40px high, with 96px left and 96px right padding.

Measured desktop grid tracks: `882.688px 259.312px` with gap `normal 56px`; `16px 280.656px 32px 50px 16px` with gap `normal`; `16px 707.328px 32px 50px 16px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `2112px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `999px`; the reusable card treatment uses `20px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use restrained pill-shaped actions, sparse navigation, and image-led editorial tiles. Separate functional chrome from the large product and technology visuals.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 50px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 46px, radius 999px, background rgba(24, 29, 37, 0.6), and border 1px rgba(219, 223, 230, 0.6). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original product or architectural photography with controlled lighting; do not reproduce vehicle imagery or marks.

**Motion.** Observed CSS transition declarations include `all, outline, outline-offset 0.35s, 0s, 0s`, `all, outline, outline-offset 0.25s, 0s, 0s`, `all, outline, outline-offset 0.07s, 0s, 0s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Measured, polished, and technically specific.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

