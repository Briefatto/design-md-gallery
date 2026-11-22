---
version: alpha
name: "Proton"
description: "Proton's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Proton."
colors:
  primary: "rgb(109, 74, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(55, 37, 128)"
  muted: "oklch(0.446 0.03 256.802)"
  border: "oklab(0.872 -0.00202137 -0.00979357 / 0.6)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'ProtonSerif, ProtonSerifFallback, ProtonScript, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1.06
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'ProtonSerif, ProtonSerifFallback, ProtonScript, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.04em
  heading:
    fontFamily: 'ProtonSerif, ProtonSerifFallback, ProtonScript, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: -0.04em
  body:
    fontFamily: 'ProtonSans, ProtonSansFallback, ProtonScript, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.63
    letterSpacing: 0em
  action:
    fontFamily: 'ProtonSans, ProtonSansFallback, ProtonScript, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.57
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
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

# Proton DESIGN.md

## Overview

A privacy suite combines white and faint lavender surfaces with deep violet serif headings, bright violet pill actions, and a tidy grid of product entry points. ProtonSerif gives the marketing hierarchy a humane editorial character while the utility layer stays compact and practical.

Built from [/](https://proton.me/) and [/pricing](https://proton.me/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(109, 74, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(55, 37, 128)` | Primary text |
| muted | `oklch(0.446 0.03 256.802)` | Supporting text |
| border | `oklab(0.872 -0.00202137 -0.00979357 / 0.6)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | ProtonSerif | 60px | 400 | 1.06 | -0.04em |
| display-mobile | ProtonSerif | 36px | 400 | 1.11 | -0.04em |
| heading | ProtonSerif | 36px | 400 | 1.16 | -0.04em |
| body | ProtonSans | 16px | 400 | 1.63 | 0em |
| action | ProtonSans | 14px | 600 | 1.57 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: ProtonSans; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://proton.me/fonts/inter/InterVariable.en.woff2") format("woff2"); }
@font-face { font-family: ProtonSans; font-style: italic; font-weight: 100 900; font-display: swap; src: url("https://proton.me/fonts/inter/InterVariable-Italic.en.woff2") format("woff2"); }
@font-face { font-family: ProtonSerif; font-style: normal; font-weight: 200 700; font-display: swap; src: url("https://proton.me/fonts/arizona/ABCArizonaFlareVariable.en.woff2") format("woff2"); }
@font-face { font-family: ProtonSerif; font-style: italic; font-weight: 200 700; font-display: swap; src: url("https://proton.me/fonts/arizona/ABCArizonaFlareVariable.en.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Use a simple product navigation and a centered introduction above a small product-tile matrix. Follow with alternating text and product panels, generous open space, and a clearly grouped suite structure. Pricing adds category tabs, a billing toggle, and aligned plan cards that stack on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 20px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 48px high, with 64px left and 64px right padding. The sampled nav is static, 33.9688px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `592px 592px` with gap `48px 96px`; `592px 592px` with gap `48px 96px`; `592px 592px` with gap `48px 96px`. Build them as a fluid grid. Sampled container maximum widths: `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `24px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use violet filled pill actions and outlined companions, thin gray-violet tile outlines, softly rounded product panels, and pricing cards with a full-width recommended-tier banner. Keep navigation and feature labels in the sans-serif reading family.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 29.9688px, horizontal padding 12px / 12px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 22px, radius 0px, background rgb(255, 255, 255), and border 0px oklch(0.446 0.03 256.802). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original soft violet gradient geometry, simple privacy diagrams, and generic product frames. Small dimensional functional icons can distinguish product categories without copying product marks. Do not reuse source portraits, product illustrations, or campaign artwork.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, box-shadow 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Reassuring, practical, and explicit about what an action does.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
