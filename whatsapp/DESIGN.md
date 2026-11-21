---
version: alpha
name: "WhatsApp"
description: "WhatsApp's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with WhatsApp."
colors:
  primary: "rgb(37, 211, 102)"
  background: "rgb(252, 245, 235)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(17, 27, 33)"
  muted: "rgb(94, 94, 94)"
  border: "rgb(255, 255, 255)"
  on-primary: "rgb(28, 30, 33)"
typography:
  display:
    fontFamily: '"WhatsApp Sans Var", sans-serif'
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"WhatsApp Sans Var", sans-serif'
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
  heading:
    fontFamily: '"WhatsApp Sans Var", sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.19
    letterSpacing: 0em
  body:
    fontFamily: '"WhatsApp Sans Var", sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.39
    letterSpacing: 0em
  action:
    fontFamily: '"WhatsApp Sans Var", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 50px
  card: 25px
spacing:
  xs: 5px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 60px
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

# WhatsApp DESIGN.md

## Overview

A messaging product uses warm, friendly surfaces, high-contrast typography, and a clear green action signal.

Built from [/](https://www.whatsapp.com/) and [/features/](https://www.whatsapp.com/features/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(37, 211, 102)` | Priority actions and selected emphasis |
| background | `rgb(252, 245, 235)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(17, 27, 33)` | Primary text |
| muted | `rgb(94, 94, 94)` | Supporting text |
| border | `rgb(255, 255, 255)` | Quiet separators and outlines |
| on-primary | `rgb(28, 30, 33)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "WhatsApp Sans Var" | 80px | 400 | 1 | 0em |
| display-mobile | "WhatsApp Sans Var" | 44px | 400 | 1 | 0em |
| heading | "WhatsApp Sans Var" | 32px | 400 | 1.19 | 0em |
| body | "WhatsApp Sans Var" | 18px | 400 | 1.39 | 0em |
| action | "WhatsApp Sans Var" | 16px | 500 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-display: swap; font-family: "WhatsApp Sans Var"; font-style: normal; font-weight: 400; src: local("WhatsApp Sans Regular Var"), local("WhatsApp-Sans-Var-Regular"), url("https://static.whatsapp.net/rsrc.php/yN/r/fQtw5exLIdT.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: "WhatsApp Sans Var"; font-style: normal; font-weight: 500; src: local("WhatsApp Sans Medium Var"), local("WhatsApp-Sans-Var-Medium"), url("https://static.whatsapp.net/rsrc.php/yN/r/fQtw5exLIdT.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: "WhatsApp Sans Var"; font-style: normal; font-weight: 700; src: local("WhatsApp Sans Bold Var"), local("WhatsApp-Sans-Var-Bold"), url("https://static.whatsapp.net/rsrc.php/yN/r/fQtw5exLIdT.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Use a warm cream page ground, a broad rounded photographic hero with overlaid light text, and generous breathing room around simple feature pairs. The calling page pairs dark editorial text with a tall rounded visual on desktop and stacks them on mobile.

Spacing scale: xs 5px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 80px high, with 60px left and 60px right padding. The sampled header is sticky, 80px high, with 60px left and 60px right padding.

 Sampled container maximum widths: `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `50px`; the reusable card treatment uses `25px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use rounded action controls, simple navigation, and open feature sections rather than dense dashboard framing.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 19px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original candid lifestyle photography and simple conversational shapes; do not copy chat screenshots, people, or marks.

**Motion.** Observed CSS transition declarations include `background-color, color 0.33s, 0.33s`, `color, border-color, background-color 0.33s, 0.5s, 0.33s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Warm, personal, and plainspoken; emphasize useful actions with short labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
