---
version: alpha
name: "Airtable"
description: "Airtable's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Airtable."
colors:
  primary: "rgb(24, 29, 38)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(248, 250, 252)"
  foreground: "rgb(51, 56, 64)"
  muted: "rgba(4, 14, 32, 0.69)"
  border: "rgb(224, 226, 230)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Haas, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Haas, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  heading:
    fontFamily: 'Haas, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  body:
    fontFamily: 'Haas, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: 0.01em
  action:
    fontFamily: 'Haas, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0em
rounded:
  control: 12px
  card: 0px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
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

# Airtable DESIGN.md

## Overview

A restrained enterprise canvas pairs Haas sans-serif headings with ample white space, dark compact actions and selectively colored workflow panels.

Built from [/](https://airtable.com/) and [/pricing](https://airtable.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(24, 29, 38)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(248, 250, 252)` | Panels and cards |
| foreground | `rgb(51, 56, 64)` | Primary text |
| muted | `rgba(4, 14, 32, 0.69)` | Supporting text |
| border | `rgb(224, 226, 230)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Haas | 40px | 400 | 1.2 | 0em |
| display-mobile | Haas | 32px | 400 | 1.25 | 0em |
| heading | Haas | 32px | 400 | 1.3 | 0em |
| body | Haas | 16px | 400 | 1.35 | 0.01em |
| action | Haas | 16px | 500 | 1.3 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-55Roman-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-55Roman-Web.woff") format("woff"); font-weight: 400; font-style: normal; }
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-56Italic-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-56Italic-Web.woff") format("woff"); font-weight: 400; font-style: italic; }
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-65Medium-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-65Medium-Web.woff") format("woff"); font-weight: 500; font-style: normal; }
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-66MediumItalic-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-66MediumItalic-Web.woff") format("woff"); font-weight: 500; font-style: italic; }
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-75Bold-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-75Bold-Web.woff") format("woff"); font-weight: 700; font-style: normal; }
@font-face { font-family: Haas; font-display: swap; src: url("https://static.airtable.com/font/NeueHaasGrotTextRound-76BoldItalic-Web.woff2") format("woff2"), url("https://static.airtable.com/font/NeueHaasGrotTextRound-76BoldItalic-Web.woff") format("woff"); font-weight: 700; font-style: italic; }
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-55Roman-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-55Roman-Web.woff")format("woff");font-weight:400;font-style:normal}
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-56Italic-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-56Italic-Web.woff")format("woff");font-weight:400;font-style:italic}
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-65Medium-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-65Medium-Web.woff")format("woff");font-weight:500;font-style:normal}
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-66MediumItalic-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-66MediumItalic-Web.woff")format("woff");font-weight:500;font-style:italic}
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-75Bold-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-75Bold-Web.woff")format("woff");font-weight:700;font-style:normal}
@font-face{font-family:Haas;font-display:swap;src:url("https://static.airtable.com/font/NeueHaasGrotTextRound-76BoldItalic-Web.woff2")format("woff2"),url("https://static.airtable.com/font/NeueHaasGrotTextRound-76BoldItalic-Web.woff")format("woff");font-weight:700;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use a thin announcement strip and a clean horizontal navigation above centered introductory copy. Alternate large feature panels with balanced text blocks. Pricing uses tall four-column plans with subtle blue emphasis; mobile stacks the comparison.

Spacing scale: xs 8px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 120.984px high, with 0px left and 0px right padding. The sampled nav is relative, 120.984px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `836.141px 603.859px` with gap `0px`; `68px 976px 204px` with gap `normal`; `85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px 85.3281px` with gap `32px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`, `1536px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Dark filled actions and thin dark outlines use comfortably rounded corners. Fine gray dividers, pale blue featured plans and tightly aligned lists keep the enterprise content orderly.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 54.7969px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Workflow and application demonstrations sit inside large colored fields; muted peach, blue, green and cream panels provide variety without changing the neutral interface foundation.

**Motion.** Observed CSS transition declarations include `all 0.15s`, `all 0.25s`, `all 0.2s`, `background-color, border-color, color, box-shadow 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm and practical, focused on connected teams, workflows and enterprise capability.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
