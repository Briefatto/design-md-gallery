---
version: alpha
name: "Zed"
description: "Zed's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Zed."
colors:
  primary: "lab(36.3314 31.1715 -81.0014)"
  background: "rgb(238, 231, 231)"
  surface: "rgb(250, 250, 250)"
  foreground: "lab(2.75381 0 0)"
  muted: "rgb(88, 88, 90)"
  border: "rgb(223, 223, 224)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'plexSerif, "plexSerif Fallback"'
    fontSize: 25.6px
    fontWeight: 390
    lineHeight: 1.25
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'plexSerif, "plexSerif Fallback"'
    fontSize: 25.6px
    fontWeight: 390
    lineHeight: 1.25
    letterSpacing: 0em
  heading:
    fontFamily: 'plexSerif, "plexSerif Fallback"'
    fontSize: 25.6px
    fontWeight: 390
    lineHeight: 1.25
    letterSpacing: 0em
  body:
    fontFamily: 'writer, "writer Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'writer, "writer Fallback"'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
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

# Zed DESIGN.md

## Overview

An editorial developer-tool site combines warm paper-like surfaces, small serif headings, monospaced supporting text, fine technical grids, and sharply framed product actions. Its current company homepage presents multiple products rather than a single oversized editor pitch.

Built from [/](https://zed.dev/) and [/pricing](https://zed.dev/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `lab(36.3314 31.1715 -81.0014)` | Priority actions and selected emphasis |
| background | `rgb(238, 231, 231)` | Page canvas |
| surface | `rgb(250, 250, 250)` | Panels and cards |
| foreground | `lab(2.75381 0 0)` | Primary text |
| muted | `rgb(88, 88, 90)` | Supporting text |
| border | `rgb(223, 223, 224)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Use paper tones, near-black text, and the Zed blue action signal for the editor context. The homepage also presents Delta with a separate red identity; keep that product accent distinct rather than blending red and blue indiscriminately. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | plexSerif | 25.6px | 390 | 1.25 | 0em |
| display-mobile | plexSerif | 25.6px | 390 | 1.25 | 0em |
| heading | plexSerif | 25.6px | 390 | 1.25 | 0em |
| body | writer | 14px | 400 | 1.43 | 0em |
| action | writer | 12px | 400 | 1.33 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: writer; src: url("https://zed.dev/_next/static/media/iAWriterQuattroS_Regular-s.p.3c4k0xaq54g87.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: writer; src: url("https://zed.dev/_next/static/media/iAWriterQuattroS_Italic-s.p.1u_8o2prgvf9l.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: writer; src: url("https://zed.dev/_next/static/media/iAWriterQuattroS_Bold-s.p.3--jbvwxe31d9.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: normal; }
@font-face { font-family: writer; src: url("https://zed.dev/_next/static/media/iAWriterQuattroS_BoldItalic-s.p.0d61w09qncs_3.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: italic; }
@font-face { font-family: plexSerif; src: url("https://zed.dev/_next/static/media/IBMPlexSerif_Var-s.p.0gdo7oqri9smw.woff2") format("woff2"); font-display: swap; font-weight: 300 700; font-style: normal; }
@font-face { font-family: plexSerif; src: url("https://zed.dev/_next/static/media/IBMPlexSerif_Var_Italic-s.p.03ivqla8dchl7.woff2") format("woff2"); font-display: swap; font-weight: 300 700; font-style: italic; }
@font-face{font-family:writer;src:url("https://zed.dev/_next/static/media/iAWriterQuattroS_Regular-s.p.3c4k0xaq54g87.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:writer;src:url("https://zed.dev/_next/static/media/iAWriterQuattroS_Italic-s.p.1u_8o2prgvf9l.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:writer;src:url("https://zed.dev/_next/static/media/iAWriterQuattroS_Bold-s.p.3--jbvwxe31d9.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:writer;src:url("https://zed.dev/_next/static/media/iAWriterQuattroS_BoldItalic-s.p.0d61w09qncs_3.woff2")format("woff2");font-display:swap;font-weight:700;font-style:italic}
@font-face{font-family:plexSerif;src:url("https://zed.dev/_next/static/media/IBMPlexSerif_Var-s.p.0gdo7oqri9smw.woff2")format("woff2");font-display:swap;font-weight:300 700;font-style:normal}
@font-face{font-family:plexSerif;src:url("https://zed.dev/_next/static/media/IBMPlexSerif_Var_Italic-s.p.03ivqla8dchl7.woff2")format("woff2");font-display:swap;font-weight:300 700;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use a restrained company masthead and aligned product introductions with serif titles and compact technical descriptions. The pricing route adds a consistent navigation scaffold, centered introduction, comparable plan columns, and fine grid framing; mobile stacks the product and plan sections.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 57px high, with 0px left and 0px right padding. The sampled nav is relative, 56px high, with 14px left and 12px right padding.

Measured desktop grid tracks: `373.328px 373.328px 373.344px` with gap `normal`; `157.328px 157.328px 157.328px 157.344px 157.328px 157.328px` with gap `16px`; `504px 504px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `1080px`, `512px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgb(5, 55, 148) 0px -2px 0px 0px inset, rgb(230, 239, 254) 0px 1px 3px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular actions, thin outlined companions, small technical labels, quiet plan boundaries, and a deliberate serif/monospace contrast. Avoid inflated pill geometry or heavy floating-card shadows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 10px / 6px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgb(255, 255, 255), and border 0px lab(44.0605 29.0279 -86.0352). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original editor-like diagrams, restrained grids, and neutral code specimens. The subtle paper/technical atmosphere can be suggested with original CSS geometry; do not copy product screenshots or marks.

**Motion.** No non-zero transition was exposed in the sampled component styles. Static screenshots do not establish entrance choreography, hover behavior, or video timing. Use restrained feedback, respect reduced-motion preferences, and verify live interactions before claiming an exact motion system.

**Voice.** Direct, specific, and comfortable with developer terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

