---
version: alpha
name: "Ghost"
description: "Ghost's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Ghost."
colors:
  primary: "rgb(21, 23, 26)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(226, 232, 240)"
  foreground: "rgb(17, 34, 32)"
  muted: "rgb(107, 114, 128)"
  border: "rgb(229, 229, 229)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'InterVariable, sans-serif'
    fontSize: 96px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.025em
  display-mobile:
    fontFamily: 'InterVariable, sans-serif'
    fontSize: 25.35px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.025em
  heading:
    fontFamily: 'InterVariable, sans-serif'
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'InterVariable, sans-serif'
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'InterVariable, sans-serif'
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 6px
  card: 16px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 72px
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

# Ghost DESIGN.md

## Overview

An editorial publishing system uses strong InterVariable headings, expansive white space and near-black actions, with dark product demonstrations and selective bright accents.

Built from [/](https://ghost.org/) and [/pricing](https://ghost.org/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(21, 23, 26)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(226, 232, 240)` | Panels and cards |
| foreground | `rgb(17, 34, 32)` | Primary text |
| muted | `rgb(107, 114, 128)` | Supporting text |
| border | `rgb(229, 229, 229)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | InterVariable | 96px | 700 | 1 | -0.025em |
| display-mobile | InterVariable | 25.35px | 700 | 1 | -0.025em |
| heading | InterVariable | 36px | 700 | 1 | 0em |
| body | InterVariable | 20px | 400 | 1.5 | 0em |
| action | InterVariable | 15px | 500 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: InterVariable; font-style: normal; font-weight: 100 900; font-display: optional; src: url("https://ghost.org/fonts/InterVariable.woff2") format("woff2"); }
@font-face { font-family: InterVariable; font-style: italic; font-weight: 100 900; font-display: optional; src: url("https://ghost.org/fonts/InterVariable-Italic.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Center the large homepage statement above a wide inset dashboard demonstration. Alternate light reading sections with dark feature bands. Pricing adds an audience-size slider above a neat three-plan grid and a long ruled comparison; mobile stacks plans and keeps the audience selector prominent.

Spacing scale: xs 3px, sm 8px, md 16px, lg 24px, xl 32px, section 72px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 94px high, with 0px left and 0px right padding. The sampled nav is static, 22.5px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `50px 50px 50px 50px 50px 50px 50px 50px 50px 50px 50px 50px` with gap `72px`; `265.594px 265.594px 265.609px 265.594px 265.609px` with gap `16px`; `265.594px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `1152px`, `768px`, `576px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 0px 1px 0px, rgba(0, 0, 0, 0.03) 0px 2px 6px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Compact dark actions, small rounded corners, lightly elevated white pricing cards and fine gray separators create a clear hierarchy. Pink slider handles and small colored badges provide specific interaction signals.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 39px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 6px, radius 5px, background rgba(100, 116, 139, 0.2), and border 0px rgb(229, 231, 235). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Dashboard and publication demonstrations, a varied publication gallery and restrained colored feature panels show the product in context.

**Motion.** Observed CSS transition declarations include `all 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Independent, clear and creator-focused, with confident headings and practical feature explanations.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
