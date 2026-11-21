---
version: alpha
name: "Framer"
description: "Framer's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Framer."
colors:
  primary: "rgb(0, 153, 255)"
  background: "rgb(0, 0, 0)"
  surface: "rgb(17, 17, 17)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.6)"
  border: "rgb(48, 48, 48)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: '"GT Walsheim Medium", "GT Walsheim Medium Placeholder", sans-serif'
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: '"GT Walsheim Medium", "GT Walsheim Medium Placeholder", sans-serif'
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  heading:
    fontFamily: '"GT Walsheim Medium", "GT Walsheim Medium Placeholder", sans-serif'
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.04em
  body:
    fontFamily: '"Inter Variable", "Inter Variable Placeholder", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.007em
  action:
    fontFamily: '"Inter Variable", "Inter Variable Placeholder", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.007em
rounded:
  control: 8px
  card: 8px
spacing:
  xs: 7px
  sm: 8px
  md: 15px
  lg: 20px
  xl: 40px
  section: 60px
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

# Framer DESIGN.md

## Overview

A black creative canvas uses compact GT Walsheim headings, Inter reading text and restrained electric-blue highlights around rich website-building demonstrations.

Built from [/](https://framer.com/) and [/pricing](https://framer.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 153, 255)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 0)` | Page canvas |
| surface | `rgb(17, 17, 17)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.6)` | Supporting text |
| border | `rgb(48, 48, 48)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "GT Walsheim Medium" | 54px | 500 | 1 | -0.04em |
| display-mobile | "GT Walsheim Medium" | 36px | 500 | 1 | -0.04em |
| heading | "GT Walsheim Medium" | 44px | 500 | 1.1 | -0.04em |
| body | "Inter Variable" | 14px | 400 | 1.4 | -0.007em |
| action | "Inter Variable" | 14px | 400 | 1.4 | -0.007em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "GT Walsheim Medium"; src: url("https://framerusercontent.com/assets/6kEeNyQwxT59TY7SpLEnehG2fc.woff2"); font-display: swap; font-style: normal; font-weight: 500; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/mYcqTSergLb16PdbJJQMl9ebYm4.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/ZRl8AlxwsX1m7xS1eJCiSPbztg.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/nhSQpBRqFmXNUBY2p5SENQ8NplQ.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+1F00-1FFF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/DYHjxG0qXjopUuruoacfl5SA.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+370-3FF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/s7NH6sl7w4NU984r5hcmo1tPSYo.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/7lw0VWkeXrGYJT05oB3DsFy8BaY.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2070, U+2074-207E, U+2080-208E, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/wx5nfqEgOXnxuFaxB0Mn9OhmcZA.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/FMAZXZOvzvP9daUF2pk7jeNQE.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/XRXDXcGEcHEhj5vRoCcaNzLUII.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/WL8JiibS9vHU7Cb3NGaJKioRjQ.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+1F00-1FFF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/LfqxQLLXCFxnUuZS8fkv9AT0uI.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+370-3FF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/3IqofWpyruZr7Qc3kaedPmw7o.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/N9O1YBTY0ROZrE0GiMsoMSyPbQ.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2070, U+2074-207E, U+2080-208E, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/Qpek1Wzh1dJ3f8j88Vebg4yC92w.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Inter Variable"; src: url("https://framerusercontent.com/assets/7lw0VWkeXrGYJT05oB3DsFy8BaY.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
```

The full fallback stacks are in the front matter.

## Layout

Keep the navigation and main statement left aligned inside a broad centered container. Large framed product demonstrations dominate the homepage. Pricing presents a fine-ruled dark plan matrix that stacks into bordered cards on mobile.

Spacing scale: xs 7px, sm 8px, md 15px, lg 20px, xl 40px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 396.297px high, with 20px left and 20px right padding. The sampled header is relative, 96.8125px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `1200px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use white homepage conversion controls, blue featured-plan actions and dark secondary buttons. Small rounded corners, low-contrast borders, compact selectors and muted white supporting text create an application-like hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 34px, horizontal padding 14px / 14px, and gap 7px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Show detailed design-canvas and website previews inside dark frames; reserve blue glow and saturated imagery for the demonstrations instead of washing the entire interface in color.

**Motion.** No non-zero transition was exposed in the sampled component styles. Static screenshots do not establish entrance choreography, hover behavior, or video timing. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident and concise, aimed at professional design and publishing workflows.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
