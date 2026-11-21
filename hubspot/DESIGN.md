---
version: alpha
name: "HubSpot"
description: "HubSpot's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with HubSpot."
colors:
  primary: "rgb(255, 72, 0)"
  background: "rgb(252, 252, 250)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(31, 31, 31)"
  muted: "rgba(0, 0, 0, 0.62)"
  border: "rgba(0, 0, 0, 0.11)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"HubSpot Serif", serif'
    fontSize: 65px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"HubSpot Serif", serif'
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: 0em
  heading:
    fontFamily: '"HubSpot Serif", serif'
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: 0em
  body:
    fontFamily: '"HubSpot Sans", sans-serif'
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.75
    letterSpacing: 0em
  action:
    fontFamily: '"HubSpot Sans", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.75
    letterSpacing: 0em
rounded:
  control: 8px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
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

# HubSpot DESIGN.md

## Overview

Warm, people-centered business software combines a literary serif hero with clear sans-serif product information and orange conversion controls.

Built from [/](https://hubspot.com/) and [/pricing](https://hubspot.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 72, 0)` | Priority actions and selected emphasis |
| background | `rgb(252, 252, 250)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(31, 31, 31)` | Primary text |
| muted | `rgba(0, 0, 0, 0.62)` | Supporting text |
| border | `rgba(0, 0, 0, 0.11)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "HubSpot Serif" | 65px | 300 | 1.2 | 0em |
| display-mobile | "HubSpot Serif" | 40px | 300 | 1.05 | 0em |
| heading | "HubSpot Serif" | 40px | 300 | 1.1 | 0em |
| body | "HubSpot Sans" | 16px | 300 | 1.75 | 0em |
| action | "HubSpot Sans" | 16px | 500 | 1.75 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-display: swap; font-family: "HubSpot Sans"; font-weight: 300 400; src: url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSans-Book.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: "HubSpot Sans"; font-weight: 500 600; src: url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSans-Medium.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: "HubSpot Serif"; font-weight: 400 600; src: url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSerif-Medium.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: "HubSpot Serif"; font-weight: 300; src: url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSerif-Book.woff2") format("woff2"); }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Light-Normal.woff2") format("woff2"); font-weight: 300; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Light-Italic.woff2") format("woff2"); font-weight: 300; font-style: italic; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Book-Normal.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Book-Italic.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Medium-Normal.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Medium-Italic.woff2") format("woff2"); font-weight: 500; font-style: italic; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Bold-Normal.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Sans"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Bold-Italic.woff2") format("woff2"); font-weight: 700; font-style: italic; font-display: swap; }
@font-face { font-family: "HubSpot Serif"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Book-Normal.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Serif"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Book-Italic.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: "HubSpot Serif"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Medium-Normal.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: "HubSpot Serif"; src: url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Medium-Italic.woff2") format("woff2"); font-weight: 500; font-style: italic; font-display: swap; }
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Light-Normal.woff2") format("woff2");font-weight:300;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Light-Italic.woff2") format("woff2");font-weight:300;font-style:italic;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Book-Normal.woff2") format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Book-Italic.woff2") format("woff2");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Medium-Normal.woff2") format("woff2");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Medium-Italic.woff2") format("woff2");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Bold-Normal.woff2") format("woff2");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Sans;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSans-Bold-Italic.woff2") format("woff2");font-weight:700;font-style:italic;font-display:swap}
@font-face{font-family:HubSpot Serif;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Book-Normal.woff2") format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Serif;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Book-Italic.woff2") format("woff2");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:HubSpot Serif;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Medium-Normal.woff2") format("woff2");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:HubSpot Serif;src:url("https://static.hsappstatic.net/ui-fonts/static-1.718/fonts/HubSpotSerif-Medium-Italic.woff2") format("woff2");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-display:swap;font-family:HubSpot Sans;font-weight:300 400;src:url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSans-Book.woff2") format("woff2")}
@font-face{font-display:swap;font-family:HubSpot Sans;font-weight:500 600;src:url("https://www.hubspot.com/hubfs/assets/hs-components/v4/fonts/hubspot-2025/HubSpotSans-Medium.woff2") format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage statement above a row of tall photographic tiles. Pricing uses a persistent product sidebar, horizontal plan comparison and denser stacked mobile panels.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 128px high, with 0px left and 0px right padding. The sampled nav is static, 52px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `236px` with gap `normal`; `24px 397.953px 24px` with gap `normal 20px`. Build them as a fluid grid. Sampled container maximum widths: `520px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use orange filled and orange outline actions, softly rounded imagery and white plan cards on light gray. The pricing page uses pill controls while the homepage favors modest button corners.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 42px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 34.375px, radius 4px, background rgba(0, 0, 0, 0), and border 0px rgb(31, 31, 31). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Human portrait and workplace photography supplies warmth; product interface panels and restrained peach gradients explain the platform.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color 0.15s, 0.15s, 0.15s`, `background-color, color 0.15s, 0.15s`, `all 0.3s`, `flex 0.35s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident and welcoming, centered on customer relationships and practical business outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
