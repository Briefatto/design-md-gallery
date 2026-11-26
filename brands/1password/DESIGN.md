---
version: alpha
name: "1Password"
description: "1Password's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with 1Password."
colors:
  primary: "rgb(20, 95, 228)"
  background: "rgb(29, 29, 33)"
  surface: "rgb(29, 29, 33)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.8)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'agileSans, "agileSans Fallback", sans-serif'
    fontSize: 88px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'agileSans, "agileSans Fallback", sans-serif'
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  heading:
    fontFamily: 'agileSans, "agileSans Fallback", sans-serif'
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  body:
    fontFamily: 'agileSans, "agileSans Fallback", sans-serif'
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: -0.02em
  action:
    fontFamily: 'agileSans, "agileSans Fallback", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.02em
rounded:
  control: 4px
  card: 25px
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

# 1Password DESIGN.md

## Overview

A secure-access system uses light agileSans headings, deep charcoal foundations, blue emphasis and crisp white product surfaces.

Built from [/](https://1password.com/) and [/pricing](https://1password.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(20, 95, 228)` | Priority actions and selected emphasis |
| background | `rgb(29, 29, 33)` | Page canvas |
| surface | `rgb(29, 29, 33)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.8)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | agileSans | 88px | 300 | 1.1 | -0.02em |
| display-mobile | agileSans | 48px | 300 | 1.1 | -0.02em |
| heading | agileSans | 40px | 300 | 1.1 | -0.02em |
| body | agileSans | 16px | 300 | 1.5 | -0.02em |
| action | agileSans | 16px | 400 | 1.5 | -0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: agileSans; src: url("https://1password.com/_next/static/media/9e5180a7add93a09-s.p.woff2?dpl=dpl_A6k2RcmdsK95Ce9vHnQnQLX63sUQ") format("woff2"); font-display: swap; }
@font-face{font-family:agileSans;src:url("https://1password.com/_next/static/media/9e5180a7add93a09-s.p.woff2?dpl=dpl_A6k2RcmdsK95Ce9vHnQnQLX63sUQ") format("woff2");font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Place the homepage statement and paired calls to action above a broad application demonstration on a blue-to-charcoal ground. Follow with alternating dark statements and light product panels. Pricing switches to a white, fine-ruled enterprise comparison with a large audience selector; mobile stacks the plan content.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 1344.59px high, with 24px left and 24px right padding. The sampled nav is relative, 132px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `188px 188px 188px 188px 188px 188px` with gap `24px`; `144.219px` with gap `normal`; `144.219px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `1392px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `25px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Pill actions, quiet outlines, thin column dividers and restrained card rounding give complex access products a clear hierarchy. Use blue for conversion and selected labels, white reversed actions within dark hero fields, and neutral surfaces for detailed product information.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Admin console, access and vault demonstrations provide the main visual proof, supported by compact company logos and minimal interface illustrations.

**Motion.** Observed CSS transition declarations include `background-size 0.3s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.3s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm, clear and assured, balancing technical access terminology with readable benefit statements.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
