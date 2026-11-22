---
version: alpha
name: "Mixpanel"
description: "Mixpanel's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Mixpanel."
colors:
  primary: "rgb(31, 32, 35)"
  background: "rgb(250, 250, 250)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(31, 32, 35)"
  muted: "rgb(98, 98, 102)"
  border: "rgb(233, 233, 233)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Garnett Medium", "Garnett Medium Placeholder", sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: '"Garnett Medium", "Garnett Medium Placeholder", sans-serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  heading:
    fontFamily: '"Garnett Medium", "Garnett Medium Placeholder", sans-serif'
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Garnett Regular", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0.02em
  action:
    fontFamily: 'Garnett, "Apercu Pro", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.68
    letterSpacing: 0.02em
rounded:
  control: 100px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 14px
  lg: 14px
  xl: 14px
  section: 14px
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

# Mixpanel DESIGN.md

## Overview

A product-intelligence system combines compact Garnett headings, small interface typography and a near-white canvas with expressive lavender, coral and deep-purple gradient fields.

Built from [/](https://mixpanel.com/) and [/pricing](https://mixpanel.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(31, 32, 35)` | Priority actions and selected emphasis |
| background | `rgb(250, 250, 250)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(31, 32, 35)` | Primary text |
| muted | `rgb(98, 98, 102)` | Supporting text |
| border | `rgb(233, 233, 233)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Garnett Medium" | 48px | 400 | 1.2 | -0.02em |
| display-mobile | "Garnett Medium" | 36px | 400 | 1.2 | -0.02em |
| heading | "Garnett Medium" | 22px | 400 | 1.2 | 0em |
| body | "Garnett Regular" | 16px | 400 | 1.6 | 0.02em |
| action | Garnett | 12px | 400 | 1.68 | 0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Garnett Medium"; src: url("https://framerusercontent.com/assets/rEHnEvAsgbukh0QUeqSHBvG6PnI.woff2"); font-display: swap; font-style: italic; font-weight: 500; }
@font-face { font-family: "Garnett Regular"; src: url("https://framerusercontent.com/assets/v6eZbzgEth8Leebqk8eQxltDlKQ.woff2"); font-display: swap; font-style: italic; font-weight: 400; }
@font-face { font-family: "Garnett Medium"; src: url("https://framerusercontent.com/assets/rEHnEvAsgbukh0QUeqSHBvG6PnI.woff2"); font-display: swap; }
@font-face { font-family: "Garnett Regular"; src: url("https://framerusercontent.com/assets/v6eZbzgEth8Leebqk8eQxltDlKQ.woff2"); font-display: swap; }
```

The full fallback stacks are in the front matter.

For action, the captured first-choice font was unavailable on the public source pages and no resolvable loading reference was observed. The generic preview starts those roles at Helvetica Neue, an available fallback from the captured CSS stack; other roles retain their observed families. The guide and tokens retain the original declared stacks and measured metrics. Preview font substitution is an adaptation.

## Layout

Use an open hero above a large analytics demonstration, alternating neutral explanatory content with richly colored feature bands. Pricing centers the statement above three tall white plans laid over a vertical gradient; mobile stacks plans.

Spacing scale: xs 4px, sm 8px, md 14px, lg 14px, xl 14px, section 14px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 64px high, with 0px left and 0px right padding. The sampled nav is relative, 64px high, with 0px left and 0px right padding.

 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `100px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Small pill actions, light card borders, colored check icons, compact tabs and softly elevated demonstration panels give dense data a friendly frame. Keep the strongest gradient color outside the main text columns.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 28px, horizontal padding 14px / 6px, and gap 2px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 16px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(31, 32, 35). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Analytics charts, AI explanations, replay and experiment interfaces carry the narrative; customer logos and small portrait clusters add proof.

**Motion.** No non-zero transition was exposed in the sampled component styles. Static screenshots do not establish entrance choreography, hover behavior, or video timing. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct and analytical, connecting behavior data to practical product decisions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
