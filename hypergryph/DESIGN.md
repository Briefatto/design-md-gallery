---
version: alpha
name: "Hypergryph"
description: "Hypergryph's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Hypergryph."
colors:
  primary: "rgb(255, 250, 0)"
  background: "rgb(0, 0, 0)"
  surface: "rgba(51, 51, 51, 0.88)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(255, 255, 255)"
  border: "rgb(243, 255, 0)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'Times'
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Times'
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  heading:
    fontFamily: 'Times'
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'SourceHanSans-Bold'
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  action:
    fontFamily: 'SourceHanSans-Regular'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
rounded:
  control: 0px
  card: 0px
spacing:
  xs: 6px
  sm: 6px
  md: 13.5px
  lg: 31.5px
  xl: 31.5px
  section: 31.5px
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

# Hypergryph DESIGN.md

## Overview

An industrial studio site uses black rectangular information panels, compact white text, sharp geometry, and thin acid-yellow markers over a faceted monochrome backdrop. The Endfield product route is a distinct, brighter game world with dense rail navigation and image-led character composition.

Built from [/](https://www.hypergryph.com/) and [/](https://endfield.hypergryph.com/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 250, 0)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 0)` | Page canvas |
| surface | `rgba(51, 51, 51, 0.88)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(255, 255, 255)` | Supporting text |
| border | `rgb(243, 255, 0)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Times | 80px | 400 | 1 | 0em |
| display-mobile | Times | 80px | 400 | 1 | 0em |
| heading | Times | 80px | 400 | 1 | 0em |
| body | SourceHanSans-Bold | 16px | 700 | 1 | 0em |
| action | SourceHanSans-Regular | 16px | 400 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face{font-family:SourceHanSans-Regular;font-style:normal;font-weight:400;;src: url("https://web-ipv6.hycdn.cn/hypergryph/official/assets/fonts/SourceHanSans-Regular.b67a96.woff2") format("woff2"); }
@font-face{font-family:SourceHanSans-Bold;font-style:normal;font-weight:400;;src: url("https://web-ipv6.hycdn.cn/hypergryph/official/assets/fonts/SourceHanSans-Bold.8b011a.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Place small rectangular information groups asymmetrically over a large environmental backdrop on desktop. Mobile reorders them into a vertical stack. The game route uses a slim utility rail, a full-bleed visual chapter, and dense supporting content; preserve that as a separate product context.

Spacing scale: xs 6px, sm 6px, md 13.5px, lg 31.5px, xl 31.5px, section 31.5px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 72px high, with 0px left and 0px right padding. The sampled header is absolute, 125px high, with 0px left and 0px right padding.

 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgb(0, 0, 0) 0px 0px 15px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use sharp panel edges, thin accent rules, compact utility links, small square markers, and minimal chrome. Avoid converting the studio presentation into soft SaaS cards.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original cinematic environments and geometric interface accents. Do not reproduce characters, game footage, or franchise marks.

**Motion.** Observed CSS transition declarations include `color 0.3s`, `color, background-color, border-radius 0.2s, 0.2s, 0.2s`, `background-color 0.2s`, `transform, width 0.3s, 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Atmospheric but concise; keep functional labels immediately understandable.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
