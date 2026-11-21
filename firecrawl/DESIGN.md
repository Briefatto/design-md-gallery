---
version: alpha
name: "Firecrawl"
description: "Firecrawl's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Firecrawl."
colors:
  primary: "oklch(0.692480443099 0.241152256705 38.595631554678)"
  background: "oklch(0.982117953213 0 180)"
  surface: "oklch(0.982117953213 0 180)"
  foreground: "oklch(0.268618690045 0 180)"
  muted: "oklch(0.268618690045 0 180 / 0.721569)"
  border: "oklch(0 0 0 / 0.05098)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'suisse, "suisse Fallback", system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: -0.005em
  display-mobile:
    fontFamily: 'suisse, "suisse Fallback", system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.01em
  heading:
    fontFamily: 'suisse, "suisse Fallback", system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.01em
  body:
    fontFamily: 'suisse, "suisse Fallback", system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'suisse, "suisse Fallback", system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 8px
  card: 10px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 34px
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

# Firecrawl DESIGN.md

## Overview

A developer infrastructure site uses a pale technical canvas, confident Swiss-style sans-serif hierarchy, vivid orange emphasis, and fine point/grid framing. The interface stays light and structured around clear starting actions and technical examples.

Built from [/](https://www.firecrawl.dev/) and [/pricing](https://www.firecrawl.dev/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `oklch(0.692480443099 0.241152256705 38.595631554678)` | Priority actions and selected emphasis |
| background | `oklch(0.982117953213 0 180)` | Page canvas |
| surface | `oklch(0.982117953213 0 180)` | Panels and cards |
| foreground | `oklch(0.268618690045 0 180)` | Primary text |
| muted | `oklch(0.268618690045 0 180 / 0.721569)` | Supporting text |
| border | `oklch(0 0 0 / 0.05098)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

The source uses CSS Color Level 4 functional declarations that this Google linter version cannot parse. Equivalent OKLCH notation preserves the color gamut and opacity; tokens.json retains each original computed declaration and conversion provenance.

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | suisse | 60px | 500 | 1.07 | -0.005em |
| display-mobile | suisse | 36px | 500 | 1.11 | -0.01em |
| heading | suisse | 30px | 500 | 1.13 | -0.01em |
| body | suisse | 16px | 400 | 1.5 | 0em |
| action | suisse | 16px | 450 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: suisse; src: url("https://www.firecrawl.dev/_next/static/immutable/media/400-s.p.0sbn468ex08t1.woff2") format("woff2"); font-display: swap; font-weight: 400; }
@font-face { font-family: suisse; src: url("https://www.firecrawl.dev/_next/static/immutable/media/450-s.p.2jy4yjhmp31zd.woff2") format("woff2"); font-display: swap; font-weight: 450; }
@font-face { font-family: suisse; src: url("https://www.firecrawl.dev/_next/static/immutable/media/500-s.p.249nb8ln_m5fq.woff2") format("woff2"); font-display: swap; font-weight: 500; }
@font-face { font-family: suisse; src: url("https://www.firecrawl.dev/_next/static/immutable/media/600-s.p.191yv5eplyndz.woff2") format("woff2"); font-display: swap; font-weight: 600; }
@font-face { font-family: suisse; src: url("https://www.firecrawl.dev/_next/static/immutable/media/700-s.p.3sdvx8ommpt9n.woff2") format("woff2"); font-display: swap; font-weight: 700; }
@font-face{font-family:suisse;src:url("https://www.firecrawl.dev/_next/static/immutable/media/400-s.p.0sbn468ex08t1.woff2")format("woff2");font-display:swap;font-weight:400}
@font-face{font-family:suisse;src:url("https://www.firecrawl.dev/_next/static/immutable/media/450-s.p.2jy4yjhmp31zd.woff2")format("woff2");font-display:swap;font-weight:450}
@font-face{font-family:suisse;src:url("https://www.firecrawl.dev/_next/static/immutable/media/500-s.p.249nb8ln_m5fq.woff2")format("woff2");font-display:swap;font-weight:500}
@font-face{font-family:suisse;src:url("https://www.firecrawl.dev/_next/static/immutable/media/600-s.p.191yv5eplyndz.woff2")format("woff2");font-display:swap;font-weight:600}
@font-face{font-family:suisse;src:url("https://www.firecrawl.dev/_next/static/immutable/media/700-s.p.3sdvx8ommpt9n.woff2")format("woff2");font-display:swap;font-weight:700}
```

The full fallback stacks are in the front matter.

## Layout

Use a framed content grid with a centered introduction, grouped actions, and a compact query/demo surface. Pricing follows the same grid with a prominent usage selector and aligned plan columns; mobile stacks the control and plan hierarchy.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 34px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 100px high, with 0px left and 0px right padding. The sampled nav is relative, 32px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `247.266px 505.453px 247.281px` with gap `normal`; `519px 519px` with gap `normal`; `556px 556px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `600px`, `650px`, `820px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `color(display-p3 0.9804 0.1127 0.098 / 0.2) 0px -6px 12px 0px inset, color(display-p3 0.9804 0.3647 0.098 / 0.12) 0px 2px 4px 0px, color(display-p3 0.9804 0.3647 0.098 / 0.12) 0px 1px 1px 0px, color(display-p3 0.9804 0.3647 0.098 / 0.16) 0px 0.5px 0.5px 0px, color(display-p3 0.9804 0.3647 0.098 / 0.2) 0px 0.25px 0.25px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact orange priority actions, quiet gray companions, restrained rounded input surfaces, subtle technical frames, and small capability/status controls. Keep the grid lighter than the reading text.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 6px / 6px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(229, 231, 235). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original fine grids, simple data-flow geometry, and synthetic code/markup specimens. Do not reproduce product screenshots, copied examples, mascot artwork, or the flame mark.

**Motion.** Observed CSS transition declarations include `all, scale, box-shadow 0.2s, 0.1s, 0.1s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.2s`, `background-color, transform 0.2s`, `all 0.05s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Straightforward and developer-oriented, with brief action labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

