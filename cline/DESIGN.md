---
version: alpha
name: "Cline"
description: "Cline's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Cline."
colors:
  primary: "oklch(0.49 0.22 278)"
  background: "oklch(0.99 0.002 32)"
  surface: "oklch(0.98 0.004 32)"
  foreground: "oklch(0.22 0.008 29)"
  muted: "oklch(0.4 0.007 29)"
  border: "oklch(0.91 0.009 31)"
  on-primary: "oklch(0.98 0.03 280)"
  accent: "oklch(0.9 0.05 278)"
typography:
  display:
    fontFamily: 'stackSansHeadline, "stackSansHeadline Fallback", Inter, system-ui, sans-serif, "Stack Sans Headline", system-ui, sans-serif'
    fontSize: 54px
    fontWeight: 340
    lineHeight: 1.2
    letterSpacing: 0.01em
  display-mobile:
    fontFamily: 'stackSansHeadline, "stackSansHeadline Fallback", Inter, system-ui, sans-serif, "Stack Sans Headline", system-ui, sans-serif'
    fontSize: 39.375px
    fontWeight: 340
    lineHeight: 1.2
    letterSpacing: 0.014em
  heading:
    fontFamily: 'stackSansHeadline, "stackSansHeadline Fallback", Inter, system-ui, sans-serif, "Stack Sans Headline", system-ui, sans-serif'
    fontSize: 27px
    fontWeight: 420
    lineHeight: 1.4
    letterSpacing: 0em
  body:
    fontFamily: 'GeistMono, ui-monospace, SFMono-Regular, "Roboto Mono", Menlo, Monaco, "Liberation Mono", "DejaVu Sans Mono", "Courier New", monospace, "Geist Mono Variable", ui-monospace, monospace'
    fontSize: 14.4px
    fontWeight: 560
    lineHeight: 1.25
    letterSpacing: 0.002em
  action:
    fontFamily: 'Inter, "Inter Fallback", "Inter Variable", system-ui, sans-serif'
    fontSize: 14.4px
    fontWeight: 560
    lineHeight: 1.25
    letterSpacing: 0.002em
rounded:
  control: 7px
  card: 0px
spacing:
  xs: 4.5px
  sm: 9px
  md: 15.75px
  lg: 22.5px
  xl: 36px
  section: 63px
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

# Cline DESIGN.md

## Overview

An open-source coding-agent site uses warm white surfaces, dark soft-edged display lettering, monospace navigation and pastel folder-like product panels. Violet actions and technical grid lines provide selective emphasis.

Built from [/](https://cline.bot/) and [/pricing](https://cline.bot/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `oklch(0.49 0.22 278)` | Priority actions and selected emphasis |
| background | `oklch(0.99 0.002 32)` | Page canvas |
| surface | `oklch(0.98 0.004 32)` | Panels and cards |
| foreground | `oklch(0.22 0.008 29)` | Primary text |
| muted | `oklch(0.4 0.007 29)` | Supporting text |
| border | `oklch(0.91 0.009 31)` | Quiet separators and outlines |
| on-primary | `oklch(0.98 0.03 280)` | Text on the primary action |
| accent | `oklch(0.9 0.05 278)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | stackSansHeadline | 54px | 340 | 1.2 | 0.01em |
| display-mobile | stackSansHeadline | 39.375px | 340 | 1.2 | 0.014em |
| heading | stackSansHeadline | 27px | 420 | 1.4 | 0em |
| body | GeistMono | 14.4px | 560 | 1.25 | 0.002em |
| action | Inter | 14.4px | 560 | 1.25 | 0.002em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/ba9851c3c22cd980-s.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/21350d82a1f187e9-s.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/c5fe6dc8356a8c31-s.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/19cfc7226ec3afaa-s.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/df0a9ae256c0569c-s.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/8e9860b6e62d6359-s.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://cline.bot/_next/static/media/e4af272ccee01ff0-s.p.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: GeistMono; src: url("https://cline.bot/_next/static/media/5b01f339abf2f1a5.p.woff2") format("woff2"); font-display: swap; font-weight: 100 900; }
@font-face { font-family: stackSansHeadline; src: url("https://cline.bot/_next/static/media/64a452275b1968c2-s.p.woff2") format("woff2"); font-display: swap; font-weight: 200 700; font-style: normal; }
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/ba9851c3c22cd980-s.woff2") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/21350d82a1f187e9-s.woff2") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/c5fe6dc8356a8c31-s.woff2") format("woff2");unicode-range:u+1f??}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/19cfc7226ec3afaa-s.woff2") format("woff2");unicode-range:u+0370-0377,u+037a-037f,u+0384-038a,u+038c,u+038e-03a1,u+03a3-03ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/df0a9ae256c0569c-s.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/8e9860b6e62d6359-s.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c4,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cline.bot/_next/static/media/e4af272ccee01ff0-s.p.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-family:GeistMono;src:url("https://cline.bot/_next/static/media/5b01f339abf2f1a5.p.woff2") format("woff2");font-display:swap;font-weight:100 900}
@font-face{font-family:stackSansHeadline;src:url("https://cline.bot/_next/static/media/64a452275b1968c2-s.p.woff2") format("woff2");font-display:swap;font-weight:200 700;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction above a modular platform grid with tab-shaped panel headings and product demonstrations. Pricing simplifies the layout into two spacious plan cards with repeated feature lists. Mobile stacks the platform panels and plan cards.

Spacing scale: xs 4.5px, sm 9px, md 15.75px, lg 22.5px, xl 36px, section 63px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is fixed, 133.5px high, with 0px left and 0px right padding. The sampled nav is static, 509px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `180px 180px 180px 180px` with gap `normal`; `180px 180px 180px 180px 180px` with gap `normal`; `63px 63px 63px 63px 63px 63px 63px 63px 63px 63px 63px 63px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `689px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `7px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small rounded violet platform actions, dark pricing actions, quiet outlined cards, pastel badges and fine grid lines. Keep display, body and monospace technical roles distinct; the folder-tab shape belongs to platform panels rather than every container.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 11.25px / 11.25px, and gap 9px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 44px, radius 0px, background rgba(0, 0, 0, 0), and border 0px oklch(0.28 0.16 278). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses product interface demonstrations, technical grids and a small agent symbol. Create original generic agent workflows and neutral UI diagrams without copying screenshots, logos or example content.

**Motion.** Observed CSS transition declarations include `scale, translate 0.12s, 0.12s`, `scale, translate, transform 0.12s, 0.12s, 0.14s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, practical and developer-aware, with clear platform labels and concise integration descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
