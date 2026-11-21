---
version: alpha
name: "Attio"
description: "Attio's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Attio."
colors:
  primary: "lab(12.7212 0.103362 -2.22102)"
  background: "rgba(255, 255, 255, 0.8)"
  surface: "rgba(255, 255, 255, 0.8)"
  foreground: "rgb(16, 17, 18)"
  muted: "rgba(0, 0, 0, 0.63)"
  border: "rgb(230, 231, 234)"
  on-primary: "lab(96.1596 -0.0828803 -1.13571)"
typography:
  display:
    fontFamily: 'interDisplay, "interDisplay Fallback"'
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07
    letterSpacing: -0.015em
  display-mobile:
    fontFamily: 'interDisplay, "interDisplay Fallback"'
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.01em
  heading:
    fontFamily: 'interDisplay, "interDisplay Fallback"'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  body:
    fontFamily: 'inter, "inter Fallback"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.01em
  action:
    fontFamily: 'inter, "inter Fallback"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.005em
rounded:
  control: 12px
  card: 10px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 58px
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

# Attio DESIGN.md

## Overview

A refined CRM site uses white space, medium-weight Inter Display headings, cool gray supporting text, and exceptionally fine interface borders. Charcoal priority actions establish a calm hierarchy, while blue highlights product states and a featured pricing tier.

Built from [/](https://attio.com/) and [/pricing](https://attio.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `lab(12.7212 0.103362 -2.22102)` | Priority actions and selected emphasis |
| background | `rgba(255, 255, 255, 0.8)` | Page canvas |
| surface | `rgba(255, 255, 255, 0.8)` | Panels and cards |
| foreground | `rgb(16, 17, 18)` | Primary text |
| muted | `rgba(0, 0, 0, 0.63)` | Supporting text |
| border | `rgb(230, 231, 234)` | Quiet separators and outlines |
| on-primary | `lab(96.1596 -0.0828803 -1.13571)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | interDisplay | 56px | 600 | 1.07 | -0.015em |
| display-mobile | interDisplay | 32px | 500 | 1.13 | -0.01em |
| heading | interDisplay | 40px | 500 | 1.1 | -0.01em |
| body | inter | 14px | 500 | 1.43 | -0.01em |
| action | inter | 14px | 500 | 1.43 | -0.005em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: inter; src: url("https://attio.com/_next/static/immutable/media/inter_regular-s.p.2bb4e2w2f8b5l.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: inter; src: url("https://attio.com/_next/static/immutable/media/inter_medium-s.p.34qksex-rl00o.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: inter; src: url("https://attio.com/_next/static/immutable/media/inter_semibold-s.p.09gosfwumfywy.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: normal; }
@font-face { font-family: inter; src: url("https://attio.com/_next/static/immutable/media/inter_bold-s.p.381ms9a343v0r.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: normal; }
@font-face { font-family: interDisplay; src: url("https://attio.com/_next/static/immutable/media/inter_display_medium-s.p.07iq05yz_unj-.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: interDisplay; src: url("https://attio.com/_next/static/immutable/media/inter_display_semibold-s.p.36u5fws9cofop.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: normal; }
@font-face { font-family: interDisplay; src: url("https://attio.com/_next/static/immutable/media/inter_display_bold-s.p.2k3a9i_yln7se.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: normal; }
@font-face{font-family:inter;src:url("https://attio.com/_next/static/immutable/media/inter_regular-s.p.2bb4e2w2f8b5l.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:inter;src:url("https://attio.com/_next/static/immutable/media/inter_medium-s.p.34qksex-rl00o.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:inter;src:url("https://attio.com/_next/static/immutable/media/inter_semibold-s.p.09gosfwumfywy.woff2")format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:inter;src:url("https://attio.com/_next/static/immutable/media/inter_bold-s.p.381ms9a343v0r.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:interDisplay;src:url("https://attio.com/_next/static/immutable/media/inter_display_medium-s.p.07iq05yz_unj-.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:interDisplay;src:url("https://attio.com/_next/static/immutable/media/inter_display_semibold-s.p.36u5fws9cofop.woff2")format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:interDisplay;src:url("https://attio.com/_next/static/immutable/media/inter_display_bold-s.p.2k3a9i_yln7se.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Place a black announcement strip above a pale navigation, then a centered headline and compact paired actions. A wide product frame sits over a subtle pale-blue vertical glow. Continue with aligned feature chapters and evenly sized pricing columns; stack plans and offer a direct email action on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 58px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 116px high, with 0px left and 0px right padding. The sampled nav is static, 67px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `subgrid [] [] [] [] [] [] []` with gap `normal`; `248.891px 95.1094px` with gap `8px`; `1440px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `896px`, `926px`, `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(99.9987 0.0337958 0.000309944) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact short-radius actions, light outlined companions, subtly rounded product frames, small pill announcements, and pricing cards with thin cool-gray rules. Use blue selectively for active or recommended states, not every primary action. Forms use a restrained rounded outline and clear labels.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 13px / 13px, and gap normal 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 40px, radius 12px, background lab(99.9987 0.0337958 0.000309944), and border 1px lab(86.0989 -0.77799 -4.0961). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original CRM-like diagrams, neutral tables, and generic data relationships. Faint vertical lines and blue atmospheric gradients may support product frames. Do not reproduce customer marks, source screens, or the wordmark.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.25s`, `color, border-color, --button-primary-bg-from, --button-primary-bg-to 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm, precise, and benefit-led without decorative jargon.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
