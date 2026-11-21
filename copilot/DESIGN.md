---
version: alpha
name: "Copilot"
description: "Copilot's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Copilot."
colors:
  primary: "rgb(16, 17, 20)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(246, 247, 249)"
  foreground: "rgb(16, 17, 20)"
  muted: "rgb(107, 112, 121)"
  border: "rgb(232, 233, 236)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"PP Mori", system-ui, sans-serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: '"PP Mori", system-ui, sans-serif'
    fontSize: 40.714px
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: -0.03em
  heading:
    fontFamily: '"PP Mori", system-ui, sans-serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.12
    letterSpacing: -0.02em
  body:
    fontFamily: '"PP Mori", system-ui, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0em
  action:
    fontFamily: '"PP Mori", system-ui, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 8px
  card: 14px
spacing:
  xs: 4px
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

# Copilot DESIGN.md

## Overview

The requested Copilot domain now presents Assembly's current identity: minimal PP Mori typography, white space, faint structural rules and almost-black actions.

Built from [/](https://copilot.app/) and [/pricing](https://copilot.app/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(16, 17, 20)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(246, 247, 249)` | Panels and cards |
| foreground | `rgb(16, 17, 20)` | Primary text |
| muted | `rgb(107, 112, 121)` | Supporting text |
| border | `rgb(232, 233, 236)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "PP Mori" | 56px | 400 | 1.02 | -0.03em |
| display-mobile | "PP Mori" | 40.714px | 400 | 1.02 | -0.03em |
| heading | "PP Mori" | 36px | 400 | 1.12 | -0.02em |
| body | "PP Mori" | 16px | 400 | 1.55 | 0em |
| action | "PP Mori" | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "PP Mori"; src: url("https://assembly.com/fonts/PPMori-Regular.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "PP Mori"; src: url("https://assembly.com/fonts/PPMori-SemiBold.otf") format("opentype"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face{font-family:PP Mori;src:url("https://assembly.com/fonts/PPMori-Regular.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:PP Mori;src:url("https://assembly.com/fonts/PPMori-SemiBold.otf")format("opentype");font-weight:500;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use an airy split desktop hero above an inset product demonstration, with subtle vertical grid lines in the background. Pricing centers its heading and segmented billing selector above four aligned plan columns; mobile stacks the content and expands actions.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 0px left and 0px right padding. The sampled nav is static, 32px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `65.5156px` with gap `normal`; `65.5156px` with gap `normal`; `320px 736px` with gap `24px 64px`. Build them as a fluid grid. Sampled container maximum widths: `512px`, `576px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `14px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Compact dark filled actions and quiet outlined alternatives use small rounded corners. Thin gray rules divide plan features; small uppercase badges and subtle surface changes create hierarchy without heavy shadows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Neutral client portal and CRM demonstrations dominate, with occasional soft pastel gradient illustrations and tiny application icons.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.45s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `background-color, color, opacity 0.15s`, `opacity 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear and composed, with short practical labels and a client-experience focus.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
