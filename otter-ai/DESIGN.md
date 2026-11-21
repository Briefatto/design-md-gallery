---
version: alpha
name: "Otter.ai"
description: "Otter.ai's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Otter.ai."
colors:
  primary: "rgb(20, 79, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 247, 247)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(105, 105, 105)"
  border: "rgb(255, 255, 255)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Circular, Arial, sans-serif'
    fontSize: 58.4825px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'Circular, Arial, sans-serif'
    fontSize: 42px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  heading:
    fontFamily: 'Circular, Arial, sans-serif'
    fontSize: 46.786px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.01em
  body:
    fontFamily: 'Circular, Arial, sans-serif'
    fontSize: 15.5953px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'Circular, Arial, sans-serif'
    fontSize: 13.008px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0.01em
rounded:
  control: 2px
  card: 0px
spacing:
  xs: 3.89883px
  sm: 7.79767px
  md: 15.5953px
  lg: 23.393px
  xl: 31.1907px
  section: 62.3813px
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

# Otter.ai DESIGN.md

## Overview

A meeting-assistant site uses light, open Circular display typography, bright blue actions and expansive white surfaces. Soft gradient media panels and darker feature sections add contrast without crowding the interface.

Built from [/](https://otter.ai/) and [/pricing](https://otter.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(20, 79, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 247, 247)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(105, 105, 105)` | Supporting text |
| border | `rgb(255, 255, 255)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Circular | 58.4825px | 300 | 1.1 | -0.02em |
| display-mobile | Circular | 42px | 300 | 1.1 | -0.02em |
| heading | Circular | 46.786px | 300 | 1.2 | -0.01em |
| body | Circular | 15.5953px | 400 | 1.5 | 0em |
| action | Circular | 13.008px | 600 | 1.2 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f9a0d91f84e8916884_CircularStd-BookItalic.otf") format("opentype"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f94caae67a65453e87_CircularStd-BoldItalic.otf") format("opentype"); font-weight: 700; font-style: italic; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f9a28756e5b5ac6840_CircularStd-Bold.otf") format("opentype"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f93527c760552e6dfe_CircularStd-Book.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d031ba7e15a7aa80ee517b_CircularStd-Light.otf") format("opentype"); font-weight: 300; font-style: normal; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d031bbb38588fe0a474ded_CircularStd-Light%20Italic.otf") format("opentype"); font-weight: 300; font-style: italic; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d046125a63de090937f8d5_CircularStd-MediumItalic.otf") format("opentype"); font-weight: 500; font-style: italic; font-display: swap; }
@font-face { font-family: Circular; src: url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d0461137ca12a2c8a0cac4_CircularStd-Medium.otf") format("opentype"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f9a0d91f84e8916884_CircularStd-BookItalic.otf")format("opentype");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f94caae67a65453e87_CircularStd-BoldItalic.otf")format("opentype");font-weight:700;font-style:italic;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f9a28756e5b5ac6840_CircularStd-Bold.otf")format("opentype");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d030f93527c760552e6dfe_CircularStd-Book.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d031ba7e15a7aa80ee517b_CircularStd-Light.otf")format("opentype");font-weight:300;font-style:normal;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d031bbb38588fe0a474ded_CircularStd-Light%20Italic.otf")format("opentype");font-weight:300;font-style:italic;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d046125a63de090937f8d5_CircularStd-MediumItalic.otf")format("opentype");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-family:Circular;src:url("https://cdn.prod.website-files.com/618e9316785b3582a5178502/67d0461137ca12a2c8a0cac4_CircularStd-Medium.otf")format("opentype");font-weight:500;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column desktop introduction with copy and actions beside a large media panel, followed by product sections and proof content. Pricing centers a blue heading above billing controls and a finely divided plan comparison. Mobile stacks the hero and plan columns into a vertical flow.

Spacing scale: xs 3.89883px, sm 7.79767px, md 15.5953px, lg 23.393px, xl 31.1907px, section 62.3813px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 122.766px high, with 0px left and 0px right padding. The sampled nav is relative, 49.1094px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `560.5px 673.125px` with gap `62.3813px`; `101.938px 102.172px 101.844px 88.7344px 65.5625px` with gap `23.393px 15.5953px`; `126.219px 59.375px 24.3906px 124.391px` with gap `23.393px 15.5953px`. Build them as a fluid grid. Sampled container maximum widths: `1491.3px`, `659.877px`, `792.438px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `2px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use bright blue filled actions, blue outlined companions, modestly rounded media panels, compact billing switches, quiet discount badges and thin comparison rules. Keep large display text light and body or feature labels compact and readable.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 41.6094px, horizontal padding 10px / 10px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses meeting portraits, product demonstrations and soft color fields. Use original licensed portraits or abstract meeting diagrams, excluding source people, recordings, screenshots and customer marks.

**Motion.** Observed CSS transition declarations include `background-color, transform, border-color, color, opacity 0.3s, 0.3s, 0.3s, 0.3s, 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, efficient and practical, with clear meeting, knowledge and workflow labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
