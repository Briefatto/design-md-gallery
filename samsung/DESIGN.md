---
version: alpha
name: "Samsung"
description: "Samsung's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Samsung."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 247, 247)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(20, 40, 160)"
  border: "rgb(221, 221, 221)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'SamsungSharpSans, arial, sans-serif'
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'SamsungSharpSans, arial, sans-serif'
    fontSize: 34.6667px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: 'SamsungSharpSans, arial, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.33
    letterSpacing: 0em
  body:
    fontFamily: 'SamsungOne, arial, sans-serif'
    fontSize: 17.3333px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0em
  action:
    fontFamily: 'SamsungSharpSansMedium, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 20px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 24px
  section: 42px
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

# Samsung DESIGN.md

## Overview

A consumer electronics site uses confident display typography, broad product imagery, and precise monochrome controls.

Built from [/us/](https://www.samsung.com/us/) and [/us/smartphones/](https://www.samsung.com/us/smartphones/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 247, 247)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(20, 40, 160)` | Supporting text |
| border | `rgb(221, 221, 221)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Use monochrome controls and white reading surfaces as the reusable foundation. Large promotional chapters invert to light text over dark or colored product imagery. The blue cookie-consent action is consent chrome, not the main product-action token. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | SamsungSharpSans | 60px | 700 | 1.2 | 0em |
| display-mobile | SamsungSharpSans | 34.6667px | 700 | 1.2 | 0em |
| heading | SamsungSharpSans | 40px | 700 | 1.33 | 0em |
| body | SamsungOne | 17.3333px | 400 | 1.33 | 0em |
| action | SamsungSharpSansMedium | 14px | 400 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-display: swap; font-family: SamsungSharpSansMedium; font-weight: 500;  ;src: url("https://www.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-common/resources/fonts/SamsungSharpSansMd.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: SamsungOne; font-weight: 400;  ;src: url("https://www.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-common/resources/fonts/SamsungOne-400.woff2") format("woff2"); }
@font-face{font-display:swap;font-family:SamsungOne;font-style:normal;font-weight:400;;src: url("https://resources.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-site/resources/us/font/SamsungOneLatinWeb-400.woff2") format("woff2"); }
@font-face{font-display:swap;font-family:SamsungOne;font-style:normal;font-weight:700;;src: url("https://resources.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-site/resources/us/font/SamsungOneLatinWeb-700.woff2") format("woff2"); }
@font-face{font-display:swap;font-family:SamsungSharpSans;font-style:normal;font-weight:700;;src: url("https://resources.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-site/resources/us/font/SamsungSharpSansBd.woff2") format("woff2"); }
@font-face{font-display:swap;font-family:SamsungSharpSans;font-style:normal;font-weight:400;;src: url("https://resources.samsung.com/etc.clientlibs/samsung/clientlibs/consumer/global/clientlib-site/resources/us/font/SamsungSharpSansBd.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Use a dense product-aware header above full-width promotional chapters. The smartphone route adds a horizontal model taxonomy, large media-led sections, and later white product/information modules. Keep text and actions aligned within each media chapter.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 24px, section 42px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 106px high, with 0px left and 0px right padding. The sampled nav is relative, 106px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `1440px`, `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `20px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use strong rounded actions, compact product tabs, and substantial product tiles with minimal decorative framing.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 23px / 23px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original studio product imagery or generic device silhouettes; do not copy product renders, campaigns, or marks.

**Motion.** Observed CSS transition declarations include `background-color 0.5s`, `opacity, transform, -webkit-transform 0.5s, 1.5s, 1.5s`, `opacity, transform, -webkit-transform 0.2s, 0.5s, 0.5s`, `color, background-color, border-color, border-bottom-color 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, concise, and oriented around useful product features.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
