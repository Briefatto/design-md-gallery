---
version: alpha
name: "Astral"
description: "Astral's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Astral."
colors:
  primary: "rgb(38, 18, 48)"
  background: "rgb(244, 244, 241)"
  surface: "rgb(244, 244, 241)"
  foreground: "rgb(38, 18, 48)"
  muted: "rgb(111, 93, 111)"
  border: "rgb(229, 231, 235)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(215, 255, 100)"
typography:
  display:
    fontFamily: '"Alliance Platt", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, monospace, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 100px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: '"Alliance Platt", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, monospace, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.01em
  heading:
    fontFamily: '"Alliance Platt", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, monospace, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.01em
  body:
    fontFamily: '"Alliance Platt", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, monospace, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.1em
  action:
    fontFamily: '"Alliance Platt", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, monospace, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.08em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 4px
  md: 16px
  lg: 24px
  xl: 32px
  section: 64px
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

# Astral DESIGN.md

## Overview

A Python tooling brand pairs giant uppercase sans-serif type, deep plum ink, electric lime accents and stepped blocks on warm white. Dense monospace product details contrast with broad display messages and muted sage or pale pink sections.

Built from [/](https://astral.sh/) and [/about](https://astral.sh/about), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(38, 18, 48)` | Priority actions and selected emphasis |
| background | `rgb(244, 244, 241)` | Page canvas |
| surface | `rgb(244, 244, 241)` | Panels and cards |
| foreground | `rgb(38, 18, 48)` | Primary text |
| muted | `rgb(111, 93, 111)` | Supporting text |
| border | `rgb(229, 231, 235)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(215, 255, 100)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Alliance Platt" | 100px | 500 | 1.05 | -0.01em |
| display-mobile | "Alliance Platt" | 56px | 500 | 1.05 | -0.01em |
| heading | "Alliance Platt" | 48px | 500 | 1.05 | -0.01em |
| body | "Alliance Platt" | 14px | 500 | 1.5 | 0.1em |
| action | "Alliance Platt" | 14px | 500 | 1.5 | 0.08em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `uppercase` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Alliance Platt"; src: url("https://astral.sh/_next/static/media/Alliance-PlattMedium.0vl0ro_iu237y.woff2") format("woff2"), url("https://astral.sh/_next/static/media/Alliance-PlattMedium.0gind4x~hac~q.woff") format("woff"); font-weight: 500; font-style: normal; font-display: block; }
@font-face { font-family: "Alliance Platt"; src: url("https://astral.sh/_next/static/media/Alliance-PlattRegular.0yly-mlezfvta.woff2") format("woff2"), url("https://astral.sh/_next/static/media/Alliance-PlattRegular.14hk8fi7exi5t.woff") format("woff"); font-weight: 400; font-style: normal; font-display: block; }
@font-face{font-family:Alliance Platt;src:url("https://astral.sh/_next/static/media/Alliance-PlattMedium.0vl0ro_iu237y.woff2")format("woff2"),url("https://astral.sh/_next/static/media/Alliance-PlattMedium.0gind4x~hac~q.woff")format("woff");font-weight:500;font-style:normal;font-display:block}
@font-face{font-family:Alliance Platt;src:url("https://astral.sh/_next/static/media/Alliance-PlattRegular.0yly-mlezfvta.woff2")format("woff2"),url("https://astral.sh/_next/static/media/Alliance-PlattRegular.14hk8fi7exi5t.woff")format("woff");font-weight:400;font-style:normal;font-display:block}
```

The full fallback stacks are in the front matter.

## Layout

Center a large desktop headline over a bold pixel-like graphic and compact paired actions. Use stepped section boundaries and broad alternating color bands. The company page combines a kinetic character headline, backer strip and numbered mission panels; mobile stacks these roles while retaining the strong geometry.

Spacing scale: xs 4px, sm 4px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 160px high, with 0px left and 0px right padding. The sampled nav is static, 119px high, with 64px left and 0px right padding.

Measured desktop grid tracks: `1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px` with gap `80px`; `1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px` with gap `80px`; `1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px 1.65625px` with gap `80px`. Build them as a fluid grid. Sampled container maximum widths: `672px`, `768px`, `1520px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular plum actions, lightly outlined companions, small uppercase navigation labels, numbered technical rows and block-like panels. Keep lime accents purposeful and preserve the contrast between display lettering and monospace detail.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses pixel geometry, kinetic characters and technical code panels. Create original stepped shapes and generic tooling diagrams without copying the wordmark, partner marks or source illustrations.

**Motion.** Observed CSS transition declarations include `all 0.2s`, `opacity 0.2s`. These prove declared timing, not that a particular animation was watched end to end. The company headline was captured during a glyph-scramble transition. These snapshots establish a kinetic typographic motif, not its final wording or exact choreography; validate motion timing and reduced-motion behavior separately.

**Voice.** Concise, technical and optimistic, with clear capability names and practical next steps.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
