---
version: alpha
name: "Calendly"
description: "Calendly's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Calendly."
colors:
  primary: "rgb(7, 26, 49)"
  background: "rgb(252, 251, 248)"
  surface: "rgb(245, 243, 238)"
  foreground: "rgb(7, 26, 49)"
  muted: "rgb(95, 109, 119)"
  border: "rgb(216, 220, 224)"
  on-primary: "rgb(252, 251, 248)"
typography:
  display:
    fontFamily: '"Calendly Sans", system-ui, -apple-system, "Segoe UI", Roboto, sans-serif'
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.028em
  display-mobile:
    fontFamily: '"Calendly Sans", system-ui, -apple-system, "Segoe UI", Roboto, sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0em
  heading:
    fontFamily: 'Geist, system-ui, -apple-system, "Segoe UI", Roboto, sans-serif'
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.028em
  body:
    fontFamily: 'Geist, system-ui, -apple-system, "Segoe UI", Roboto, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: 'Geist, system-ui, -apple-system, "Segoe UI", Roboto, sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0em
rounded:
  control: 16px
  card: 48px
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

# Calendly DESIGN.md

## Overview

A warm scheduling system combines distinctive Calendly Sans headings, Geist interface text and navy actions with soft blue, lilac and peach visual fields.

Built from [/](https://calendly.com/) and [/pricing](https://calendly.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(7, 26, 49)` | Priority actions and selected emphasis |
| background | `rgb(252, 251, 248)` | Page canvas |
| surface | `rgb(245, 243, 238)` | Panels and cards |
| foreground | `rgb(7, 26, 49)` | Primary text |
| muted | `rgb(95, 109, 119)` | Supporting text |
| border | `rgb(216, 220, 224)` | Quiet separators and outlines |
| on-primary | `rgb(252, 251, 248)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Calendly Sans" | 72px | 500 | 1.1 | -0.028em |
| display-mobile | "Calendly Sans" | 40px | 500 | 1.1 | 0em |
| heading | Geist | 36px | 500 | 1.1 | -0.028em |
| body | Geist | 14px | 400 | 1.4 | 0em |
| action | Geist | 14px | 500 | 1.4 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Geist; src: url("https://calendly.com/_astro/geist-latin.BfrrXRGr.woff2") format("woff2"); font-weight: 100 900; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Geist; src: url("https://calendly.com/_astro/geist-latin-ext.DavUKqbp.woff2") format("woff2"); font-weight: 100 900; font-style: normal; font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Calendly Sans"; src: url("https://calendly.com/_astro/calendly-sans-variable.D6oRyvrG.woff2") format("woff2"); font-weight: 100 900; font-style: oblique 0deg 10deg; font-display: swap; }
@font-face{font-family:Geist;src:url("https://calendly.com/_astro/geist-latin.BfrrXRGr.woff2")format("woff2");font-weight:100 900;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Geist;src:url("https://calendly.com/_astro/geist-latin-ext.DavUKqbp.woff2")format("woff2");font-weight:100 900;font-style:normal;font-display:swap;unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Calendly Sans;src:url("https://calendly.com/_astro/calendly-sans-variable.D6oRyvrG.woff2")format("woff2");font-weight:100 900;font-style:oblique 0deg 10deg;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Inset major sections into large rounded panels on an off-white canvas. Center the hero above paired sign-up controls, then use broad feature cards. Pricing places four tall plans in a regular row with a raised blue featured header and stacked mobile cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 68px high, with 0px left and 0px right padding. The sampled nav is static, 35.5938px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `56px` with gap `normal`; `56px` with gap `normal`; `56px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `640px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `16px`; the reusable card treatment uses `48px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Navy filled and outlined controls, modestly rounded fields, quiet separators and lightly elevated white cards establish the interface. Serif price numerals add editorial emphasis without replacing the sans-serif navigation.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 50%, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use scheduling and meeting-summary interface illustrations, small participant portraits, soft geometric backgrounds and compact colored category icons.

**Motion.** Observed CSS transition declarations include `box-shadow 0.2s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `all 0.15s`, `background-color, color, border-color 0.15s, 0.15s, 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Reassuring and efficient, focused on reducing meeting work and giving clear next steps.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
