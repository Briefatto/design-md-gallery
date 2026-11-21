---
version: alpha
name: "Ramp"
description: "Ramp's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Ramp."
colors:
  primary: "lab(92.1406 -20.4979 84.7726)"
  background: "lab(100 0 0)"
  surface: "lab(95.604 0.426412 1.20401)"
  foreground: "lab(2.83994 0.367254 0.969091)"
  muted: "lab(2.83994 0.367254 0.969091 / 0.6)"
  border: "oklab(0.2145 0.00152552 0.000480294 / 0.1)"
  on-primary: "lab(2.83994 0.367254 0.969091)"
typography:
  display:
    fontFamily: 'Lausanne, Arial, sans-serif'
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Lausanne, Arial, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: 0em
  heading:
    fontFamily: 'Lausanne, Arial, sans-serif'
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: 0em
  body:
    fontFamily: 'Lausanne, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0em
  action:
    fontFamily: 'Lausanne, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 8px
  card: 0px
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

# Ramp DESIGN.md

## Overview

A precise financial interface pairs Lausanne typography, warm white surfaces and nearly black text with a sharp acid-yellow priority color.

Built from [/](https://ramp.com/) and [/pricing](https://ramp.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `lab(92.1406 -20.4979 84.7726)` | Priority actions and selected emphasis |
| background | `lab(100 0 0)` | Page canvas |
| surface | `lab(95.604 0.426412 1.20401)` | Panels and cards |
| foreground | `lab(2.83994 0.367254 0.969091)` | Primary text |
| muted | `lab(2.83994 0.367254 0.969091 / 0.6)` | Supporting text |
| border | `oklab(0.2145 0.00152552 0.000480294 / 0.1)` | Quiet separators and outlines |
| on-primary | `lab(2.83994 0.367254 0.969091)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Lausanne | 64px | 400 | 1 | 0em |
| display-mobile | Lausanne | 40px | 400 | 1.05 | 0em |
| heading | Lausanne | 28px | 400 | 1.14 | 0em |
| body | Lausanne | 16px | 400 | 1.38 | 0em |
| action | Lausanne | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Lausanne; font-style: normal; font-weight: 300; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-300/TWKLausanne-300.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: italic; font-weight: 300; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-300/TWKLausanne-300Italic.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: normal; font-weight: 350; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-350/TWKLausanne-350.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: italic; font-weight: 350; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-350/TWKLausanne-350Italic.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: normal; font-weight: 400; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-400/TWKLausanne-400.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: italic; font-weight: 400; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-400/TWKLausanne-400Italic.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: normal; font-weight: 700; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-700/TWKLausanne-700.woff2") format("woff2"); }
@font-face { font-family: Lausanne; font-style: italic; font-weight: 700; font-display: swap; src: url("https://assets.ramp.com/fonts/lausanne/lausanne-700/TWKLausanne-700Italic.woff2") format("woff2"); }
@font-face{font-family:Lausanne;font-style:normal;font-weight:300;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-300/TWKLausanne-300.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:italic;font-weight:300;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-300/TWKLausanne-300Italic.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:normal;font-weight:350;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-350/TWKLausanne-350.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:italic;font-weight:350;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-350/TWKLausanne-350Italic.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:normal;font-weight:400;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-400/TWKLausanne-400.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:italic;font-weight:400;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-400/TWKLausanne-400Italic.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:normal;font-weight:700;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-700/TWKLausanne-700.woff2")format("woff2")}
@font-face{font-family:Lausanne;font-style:italic;font-weight:700;font-display:swap;src:url("https://assets.ramp.com/fonts/lausanne/lausanne-700/TWKLausanne-700Italic.woff2")format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Use an airy homepage statement above an inline email-and-action group and a large inset financial workflow demonstration. Fine dotted grids and tiny operational counters create a technical backdrop. Pricing centers the introduction above three tall plans, with the middle plan outlined in yellow; mobile stacks the cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 102px high, with 0px left and 0px right padding. The sampled nav is static, 102px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `1440px` with gap `normal`; `162.875px 162.875px 162.875px 162.875px 162.875px 162.875px 162.875px 162.875px` with gap `1px`; `644px 644px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `1050px`, `656px`, `755px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Yellow filled actions, quiet neutral secondary controls, lightly rounded inputs and thin warm-gray rules keep dense financial content legible. Small plan labels sit across the card's top border; reserve dark fills for enterprise emphasis.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 52px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 52px, radius 10px, background rgba(0, 0, 0, 0), and border 0px rgba(33, 33, 33, 0.1). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Invoices, transaction panels and operational workflow demonstrations dominate, with occasional workplace photography. Keep imagery framed and secondary to the clear interface structure.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.3s`, `color 0.24s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `transform, box-shadow 0.4s, 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Concise and practical, emphasizing efficiency, control and financial outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
