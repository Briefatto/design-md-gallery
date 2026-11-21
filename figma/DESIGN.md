---
version: alpha
name: "Figma"
description: "Figma's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Figma."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(230, 230, 230)"
  foreground: "rgb(0, 0, 0)"
  muted: "oklch(0 0 0 / 0.54)"
  border: "oklch(0 0 0 / 0.16)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'figmaSans, "figmaSans Fallback", "SF Pro Display", system-ui, helvetica, sans-serif'
    fontSize: 86px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'figmaSans, "figmaSans Fallback", "SF Pro Display", system-ui, helvetica, sans-serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  heading:
    fontFamily: 'figmaSans, "figmaSans Fallback", "SF Pro Display", system-ui, helvetica, sans-serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  body:
    fontFamily: 'figmaSans, "figmaSans Fallback", "SF Pro Display", system-ui, helvetica, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: 'figmaSans, "figmaSans Fallback", "SF Pro Display", system-ui, helvetica, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: 0em
rounded:
  control: 8px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
  section: 78px
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

# Figma DESIGN.md

## Overview

An open collaborative canvas: spare black typography, white space and playful modular color sit beside precise product comparison tables.

Built from [/](https://figma.com/) and [/pricing](https://figma.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(230, 230, 230)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `oklch(0 0 0 / 0.54)` | Supporting text |
| border | `oklch(0 0 0 / 0.16)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

The source uses CSS Color Level 4 declarations that this Google linter version cannot parse. Equivalent OKLCH notation, including zero hue for achromatic colors, preserves the color gamut and opacity; tokens.json retains each original computed declaration and conversion provenance.

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | figmaSans | 86px | 400 | 0.95 | -0.02em |
| display-mobile | figmaSans | 56px | 400 | 1 | -0.01em |
| heading | figmaSans | 36px | 400 | 1.2 | -0.01em |
| body | figmaSans | 16px | 400 | 1.4 | 0em |
| action | figmaSans | 16px | 400 | 1.45 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: figmaSans; src: url("https://www.figma.com/_netlify/_next/static/media/7c42ed55a7834032-s.p.woff2") format("woff2"); font-display: swap; font-weight: 320; }
@font-face{font-family:figmaSans;src:url("https://www.figma.com/_netlify/_next/static/media/7c42ed55a7834032-s.p.woff2") format("woff2");font-display:swap;font-weight:320}
```

The full fallback stacks are in the front matter.

## Layout

Use broad editorial fields and a compact top navigation. Pricing shifts into a tightly aligned seat matrix with fine vertical rules; mobile stacks the plan cards and retains compact product tabs.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 36px, section 78px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 78.3906px high, with 0px left and 0px right padding. The sampled nav is static, 39.1875px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `329px` with gap `normal`; `329px` with gap `normal`; `329px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `901.333px`, `840px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `oklch(0 0 none / 0.16) 0px 0px 0px 1px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Black filled calls to action and thin black outlines anchor the interface. Rounded 8px controls, small mono labels and pale green feature highlights give the dense tables a clear hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 46.3906px, horizontal padding 22px / 22px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Pair editable canvas and interface imagery with abstract pastel panels and occasional vivid product colors; keep text and controls outside the media.

**Motion.** Observed CSS transition declarations include `background 0.4s`, `background, box-shadow 0.18s, 0.18s`, `all 0.2s`, `background 2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, creative and concise, with large plain statements and short practical labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
