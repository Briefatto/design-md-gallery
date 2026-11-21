---
version: alpha
name: "Datadog"
description: "Datadog's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Datadog."
colors:
  primary: "rgb(99, 44, 166)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(33, 37, 41)"
  muted: "rgb(85, 85, 85)"
  border: "rgb(238, 238, 238)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'NationalWeb, Helvetica, Arial, sans-serif'
    fontSize: 68px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'NationalWeb, Helvetica, Arial, sans-serif'
    fontSize: 38px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: 0em
  heading:
    fontFamily: 'NationalWeb, Helvetica, Arial, sans-serif'
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: 0em
  body:
    fontFamily: 'NationalWeb, Helvetica, Arial, sans-serif'
    fontSize: 22px
    fontWeight: 300
    lineHeight: 1.36
    letterSpacing: 0em
  action:
    fontFamily: 'NationalWeb, Helvetica, Arial, sans-serif'
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.22
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 68px
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

# Datadog DESIGN.md

## Overview

An observability platform combines white enterprise layouts, NationalWeb typography, and assertive purple actions. The restrained opening gives way to saturated violet and dark technical storytelling; pricing uses a pale lavender introduction and dense factual comparisons.

Built from [/](https://www.datadoghq.com/) and [/pricing/](https://www.datadoghq.com/pricing/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(99, 44, 166)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(33, 37, 41)` | Primary text |
| muted | `rgb(85, 85, 85)` | Supporting text |
| border | `rgb(238, 238, 238)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | NationalWeb | 68px | 600 | 1 | 0em |
| display-mobile | NationalWeb | 38px | 600 | 1.11 | 0em |
| heading | NationalWeb | 36px | 600 | 1.11 | 0em |
| body | NationalWeb | 22px | 300 | 1.36 | 0em |
| action | NationalWeb | 18px | 700 | 1.22 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: nationalweb;  font-weight: 200; font-style: normal; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Light.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 200; font-style: italic; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-LightItalic.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 500; font-style: normal; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Medium.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 600; font-style: normal; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Semibold.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 700; font-style: normal; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Bold.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 300; font-style: normal; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Book.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-weight: 300; font-style: italic; font-stretch: normal; font-display: swap; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-BookItalic.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 100; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Thin.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 200; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Light.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 300; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Book.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 400; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Regular.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 600; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Semibold.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: normal; font-stretch: normal; font-weight: 700; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Bold.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-weight: 300; font-style: italic; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-BookItalic.woff2") format("woff2"); }
@font-face { font-family: nationalweb;  font-display: swap; font-style: italic; font-stretch: normal; font-weight: 400; ;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-RegularItalic.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:200;font-style:normal;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Light.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:200;font-style:italic;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-LightItalic.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:500;font-style:normal;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Medium.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:600;font-style:normal;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Semibold.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:700;font-style:normal;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Bold.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:300;font-style:normal;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Book.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-weight:300;font-style:italic;font-stretch:normal;font-display:swap;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-BookItalic.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:100;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Thin.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:200;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Light.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:300;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Book.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:400;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Regular.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:600;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Semibold.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:normal;font-stretch:normal;font-weight:700;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-Bold.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-weight:300;font-style:italic;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-BookItalic.woff2") format("woff2"); }
@font-face{font-family:nationalweb;font-display:swap;font-style:italic;font-stretch:normal;font-weight:400;src: url("https://www.datadoghq.com/fonts/web-fonts/NationalWeb-RegularItalic.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Use a thin announcement strip, a broad desktop navigation with a centered identity position, and a centered hero above an angled product frame. Pricing introduces a category rail beside comparison columns. Collapse categories into compact selectors and stack tiers on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 68px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 1049.8px high, with 0px left and 0px right padding. The sampled nav is fixed, 130px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px` with gap `12px`; `98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px 98.3281px` with gap `12px`; `120px 120px 120px 120px 120px 120px 120px 120px 120px 120px 120px 120px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `1342px`, `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.07) 0px 0px 8px 8px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular purple actions with uppercase labels, thin purple outlined alternatives, economical nav links, category selectors, and clearly aligned comparison rows. Keep corner rounding modest and distinguish dense pricing content with fine rules and whitespace.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 50px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 49px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(33, 37, 41). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original monitoring charts, infrastructure diagrams, and generic dashboard geometry. Some chapters may use bright violet glows and dimensional technical scenes. Avoid copied metrics, product screens, mascot artwork, and customer identities.

**Motion.** Observed CSS transition declarations include `height 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Specific, explanatory, and technically grounded.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
