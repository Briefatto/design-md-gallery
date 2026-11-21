---
version: alpha
name: "Toss"
description: "Toss's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Toss."
colors:
  primary: "rgb(49, 130, 246)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(245, 245, 245)"
  foreground: "rgb(28, 31, 37)"
  muted: "rgb(78, 83, 92)"
  border: "rgb(227, 227, 227)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: '"Toss Product Sans OTF", sans-serif'
    fontSize: 100px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: '"Toss Product Sans OTF", sans-serif'
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.03em
  heading:
    fontFamily: '"Toss Product Sans OTF", sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.28
    letterSpacing: 0em
  body:
    fontFamily: '"Toss Product Sans OTF", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  action:
    fontFamily: '"Toss Product Sans OTF", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
rounded:
  control: 12px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 24px
  section: 48px
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

# Toss DESIGN.md

## Overview

A financial product uses spacious composition, strong sans-serif hierarchy, and controlled blue emphasis.

Built from [/](https://toss.im/) and [/team](https://toss.im/team), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(49, 130, 246)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(245, 245, 245)` | Panels and cards |
| foreground | `rgb(28, 31, 37)` | Primary text |
| muted | `rgb(78, 83, 92)` | Supporting text |
| border | `rgb(227, 227, 227)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Toss Product Sans OTF" | 100px | 700 | 1 | -0.03em |
| display-mobile | "Toss Product Sans OTF" | 60px | 700 | 1 | -0.03em |
| heading | "Toss Product Sans OTF" | 40px | 700 | 1.28 | 0em |
| body | "Toss Product Sans OTF" | 16px | 500 | 1 | -0.02em |
| action | "Toss Product Sans OTF" | 16px | 500 | 1 | -0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face{src:url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Regular.woff2") format("woff2"),url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Regular.otf") format("opentype");font-display:swap;font-style:normal;font-weight:400;font-family:Toss Product Sans OTF}
@font-face{src:url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Medium.woff2") format("woff2"),url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Medium.otf") format("opentype");font-display:swap;font-style:normal;font-weight:500;font-family:Toss Product Sans OTF}
@font-face{src:url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Semibold.woff2") format("woff2"),url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Semibold.otf") format("opentype");font-display:swap;font-style:normal;font-weight:600;font-family:Toss Product Sans OTF}
@font-face{src:url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Bold.woff2") format("woff2"),url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Bold.otf") format("opentype");font-display:swap;font-style:normal;font-weight:700;font-family:Toss Product Sans OTF}
@font-face{src:url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Extrabold.woff2") format("woff2"),url("https://static.toss.im/assets/toss-im/font/TossProductSansOTF-Extrabold.otf") format("opentype");font-display:swap;font-style:normal;font-weight:800;font-family:Toss Product Sans OTF}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/bee7118203610aa4.woff2") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/ddc3e0e9f748bc4e.woff2") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/0cf46b173d5d4150.woff2") format("woff2");unicode-range:u+2000-2001,u+2004-2008,u+200a,u+23b8-23bd,u+2500-259f}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/f03ae0efb5d567c5.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/8dabd5c20013d1cb.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c4,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-family:Geist Mono;font-style:normal;font-weight:400;font-display:swap;src:url("https://static.toss.im/frontend/new.toss.im/toss-im-new/_next/static/media/190cd984471a34c4.p.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
```

The full fallback stacks are in the front matter.

## Layout

Use a compact white navigation band above a very large rounded photographic hero. Overlay the opening message near the lower edge of the image. The team page changes to large dark type, a pale blue atmospheric wash, fine rules, and spacious editorial rows.

Spacing scale: xs 4px, sm 8px, md 12px, lg 24px, xl 24px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 64px high, with 108px left and 108px right padding. The sampled nav is fixed, 132px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use calm rounded surfaces, strong filled actions, compact navigation, and spacious feature groupings.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 12px / 12px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original candid lifestyle photography and clean product compositions with generous rounded cropping. Do not reproduce photographed people, device screens, or brand marks from the source.

**Motion.** Observed CSS transition declarations include `background-color, backdrop-filter, -webkit-backdrop-filter 0.3s, 0.3s, 0.3s`, `opacity 0.2s`, `color 0.6s`, `color 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Reassuring, simple, and confident without unnecessary technical language.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
