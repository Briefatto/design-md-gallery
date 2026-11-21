---
version: alpha
name: "Netflix"
description: "Netflix's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Netflix."
colors:
  primary: "rgb(229, 9, 20)"
  background: "rgb(0, 0, 0)"
  surface: "rgba(22, 22, 22, 0.7)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.7)"
  border: "rgb(229, 9, 20)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Netflix Sans", "Helvetica Neue", "Segoe UI", Roboto, Ubuntu, sans-serif'
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Netflix Sans", "Helvetica Neue", "Segoe UI", Roboto, Ubuntu, sans-serif'
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: 0em
  heading:
    fontFamily: '"Netflix Sans", "Helvetica Neue", "Segoe UI", Roboto, Ubuntu, sans-serif'
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Netflix Sans", "Helvetica Neue", "Segoe UI", Roboto, Ubuntu, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  action:
    fontFamily: '"Netflix Sans", "Helvetica Neue", "Segoe UI", Roboto, Ubuntu, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 4px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 80px
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

# Netflix DESIGN.md

## Overview

A cinematic subscription interface sets bright action color and large, confident headings against dark entertainment imagery.

Built from [/](https://www.netflix.com/) and [/en/](https://about.netflix.com/en/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(229, 9, 20)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 0)` | Page canvas |
| surface | `rgba(22, 22, 22, 0.7)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.7)` | Supporting text |
| border | `rgb(229, 9, 20)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Netflix Sans" | 56px | 700 | 1.25 | 0em |
| display-mobile | "Netflix Sans" | 32px | 700 | 1.25 | 0em |
| heading | "Netflix Sans" | 24px | 500 | 1.2 | 0em |
| body | "Netflix Sans" | 16px | 400 | 1.2 | 0em |
| action | "Netflix Sans" | 16px | 400 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 100; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Th.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Th.woff") format("woff"); }
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 300; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Lt.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Lt.woff") format("woff"); }
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 400; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Rg.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Rg.woff") format("woff"); }
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 500; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Md.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Md.woff") format("woff"); }
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 700; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Bd.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Bd.woff") format("woff"); }
@font-face { font-display: optional; font-family: "Netflix Sans"; font-weight: 900; src: url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Blk.woff2") format("woff2"), url("https://assets.nflxext.com/ffe/siteui/fonts/netflix-sans/v3/NetflixSans_W_Blk.woff") format("woff"); }
```

The full fallback stacks are in the front matter.

## Layout

Give the leading message strong central emphasis, place conversion controls together, then organize benefits and frequently asked questions into clear bands. The corporate page expands the same dark/red vocabulary into oversized editorial headings and vertical red light bands; keep that treatment distinct from the subscription form.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 80px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 88px high, with 0px left and 0px right padding. The sampled header is fixed, 100px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `100%`, `1440px`, `1160px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use assertive filled actions, dark input surfaces, clear section separators, and substantial content panels.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 56px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 56px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgba(0, 0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Describe cinematic full-bleed photography without copying stills, posters, faces, or the wordmark.

**Motion.** Observed CSS transition declarations include `background-color, border-color 0.25s`, `transform 0.2s`, `background-color, box-shadow 0.3s, 0.3s`, `all 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, confident, and conversion-focused; make the next action obvious.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

