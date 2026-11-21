---
version: alpha
name: "Perplexity"
description: "Perplexity's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Perplexity."
colors:
  primary: "rgb(0, 66, 65)"
  background: "rgb(252, 252, 249)"
  surface: "oklch(0.988087611616 0 0)"
  foreground: "rgb(11, 40, 51)"
  muted: "oklch(0.260731937441 0.039802832431 226.507388280927 / 0.75)"
  border: "oklch(0.260731937441 0.039802832431 226.507388280927 / 0.15)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'pplxSans, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.005em
  display-mobile:
    fontFamily: 'pplxSans, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.005em
  heading:
    fontFamily: 'pplxSans, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.005em
  body:
    fontFamily: 'pplxSans, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'pplxSans, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 2
    letterSpacing: 0em
rounded:
  control: 40px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 30px
  section: 30px
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

# Perplexity DESIGN.md

## Overview

A calm knowledge interface uses warm off-white surfaces, dark blue-green ink, and restrained controls. The public search landing uses practical sans-serif type and a persistent utility rail; enterprise marketing introduces editorial serif headlines and spacious image/text compositions.

Built from [/](https://www.perplexity.ai/) and [/enterprise](https://www.perplexity.ai/enterprise), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 66, 65)` | Priority actions and selected emphasis |
| background | `rgb(252, 252, 249)` | Page canvas |
| surface | `oklch(0.988087611616 0 0)` | Panels and cards |
| foreground | `rgb(11, 40, 51)` | Primary text |
| muted | `oklch(0.260731937441 0.039802832431 226.507388280927 / 0.75)` | Supporting text |
| border | `oklch(0.260731937441 0.039802832431 226.507388280927 / 0.15)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

The source uses CSS Color Level 4 functional declarations that this Google linter version cannot parse. Equivalent OKLCH notation preserves the color gamut and opacity; tokens.json retains each original computed declaration and conversion provenance.

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | pplxSans | 26px | 400 | 1.5 | -0.005em |
| display-mobile | pplxSans | 26px | 400 | 1.5 | -0.005em |
| heading | pplxSans | 26px | 400 | 1.5 | -0.005em |
| body | pplxSans | 14px | 400 | 1.43 | 0em |
| action | pplxSans | 14px | 500 | 2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: pplxSans; src: url("https://frontend-cdn.perplexity.ai/_agi_assets/fonts/Curious-Sans-1.002-VF.woff2") format("woff2"); font-weight: 300 900; font-style: oblique 0deg 6deg; font-display: swap; }
@font-face { font-family: pplxSans; src: url("https://frontend-cdn.perplexity.ai/_agi_assets/fonts/Curious-Sans-Devanagari-1.002-VF.woff2") format("woff2"); font-weight: 300 900; font-style: oblique 0deg 6deg; font-display: swap; unicode-range: U+900-97F, U+1CD0-1CFF, U+A8E0-A8FF; }
@font-face{font-family:pplxSans;src:url("https://frontend-cdn.perplexity.ai/_agi_assets/fonts/Curious-Sans-1.002-VF.woff2")format("woff2");font-weight:300 900;font-style:oblique 0deg 6deg;font-display:swap}
@font-face{font-family:pplxSans;src:url("https://frontend-cdn.perplexity.ai/_agi_assets/fonts/Curious-Sans-Devanagari-1.002-VF.woff2")format("woff2");font-weight:300 900;font-style:oblique 0deg 6deg;font-display:swap;unicode-range:U+900-97F,U+1CD0-1CFF,U+A8E0-A8FF}
```

The full fallback stacks are in the front matter.

## Layout

On the search landing, center the question entry surface beside a narrow left utility rail. Enterprise marketing uses a split hero, generous cream margins, a horizontal trust row, and modular feature sections. Keep these two layout contexts distinct.

Spacing scale: xs 4px, sm 8px, md 16px, lg 20px, xl 30px, section 30px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 900px high, with 0px left and 0px right padding. The sampled nav is relative, 64px high, with 20px left and 20px right padding.

Measured desktop grid tracks: `320.188px` with gap `normal`; `24px` with gap `normal`; `24px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `40px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use softly rounded entry surfaces, clear compact actions, understated dividers, and well-spaced supporting cards.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 20px / 20px, and gap 10px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use abstract information diagrams and original editorial images with restrained supporting icons.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `background-color, border-color, color, opacity 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Curious and concise; make prompts and actions useful rather than theatrical.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

