---
version: alpha
name: "Linear"
description: "Linear's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Linear."
colors:
  primary: "rgb(229, 229, 230)"
  background: "rgb(8, 9, 10)"
  surface: "rgb(18, 20, 20)"
  foreground: "rgb(247, 248, 248)"
  muted: "rgb(138, 143, 152)"
  border: "rgb(46, 46, 50)"
  on-primary: "rgb(8, 9, 10)"
  accent: "rgb(94, 106, 210)"
typography:
  display:
    fontFamily: '"Inter Variable", "SF Pro Display", -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif'
    fontSize: 64px
    fontWeight: 510
    lineHeight: 1
    letterSpacing: -0.022em
  display-mobile:
    fontFamily: '"Inter Variable", "SF Pro Display", -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif'
    fontSize: 38px
    fontWeight: 510
    lineHeight: 1.1
    letterSpacing: -0.022em
  heading:
    fontFamily: '"Inter Variable", "SF Pro Display", -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif'
    fontSize: 48px
    fontWeight: 510
    lineHeight: 1
    letterSpacing: -0.022em
  body:
    fontFamily: '"Inter Variable", "SF Pro Display", -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.011em
  action:
    fontFamily: '"Inter Variable", "SF Pro Display", -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif'
    fontSize: 13px
    fontWeight: 510
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 9999px
  card: 0px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 63.8px
components:
  accent-text:
    textColor: "{colors.accent}"
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

# Linear DESIGN.md

## Overview

A near-black product site uses pale, tightly tracked sans-serif headlines, quiet gray supporting copy and precise interface imagery. Most visual energy comes from product panels and a few selective luminous accents.

Built from [/](https://linear.app/) and [/pricing](https://linear.app/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(229, 229, 230)` | Priority actions and selected emphasis |
| background | `rgb(8, 9, 10)` | Page canvas |
| surface | `rgb(18, 20, 20)` | Panels and cards |
| foreground | `rgb(247, 248, 248)` | Primary text |
| muted | `rgb(138, 143, 152)` | Supporting text |
| border | `rgb(46, 46, 50)` | Quiet separators and outlines |
| on-primary | `rgb(8, 9, 10)` | Text on the primary action |
| accent | `rgb(94, 106, 210)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Inter Variable" | 64px | 510 | 1 | -0.022em |
| display-mobile | "Inter Variable" | 38px | 510 | 1.1 | -0.022em |
| heading | "Inter Variable" | 48px | 510 | 1 | -0.022em |
| body | "Inter Variable" | 15px | 400 | 1.6 | -0.011em |
| action | "Inter Variable" | 13px | 510 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Inter Variable;font-weight:100 900;font-display:swap;font-style:normal;src:url("https://static.linear.app/fonts/InterVariable.woff2?v=4.1")format("woff2")}
@font-face{font-family:Inter Variable;font-weight:100 900;font-display:swap;font-style:italic;src:url("https://static.linear.app/fonts/InterVariable-Italic.woff2?v=4.1")format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Use a wide, left-aligned introduction followed by a large product demonstration with deep surrounding whitespace. Pricing becomes an economical row of plan columns separated by faint rules; the mobile view stacks plans and crops or scales supporting demonstrations.

Spacing scale: xs 3px, sm 8px, md 16px, lg 24px, xl 32px, section 63.8px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 73px high, with 0px left and 0px right padding. The sampled header is static, 44px high, with 12px left and 12px right padding.

 Sampled container maximum widths: `1250px`, `541.566px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact light pill actions, subdued dark secondary actions, thin separators, small feature checks and restrained dark panels. Price plans remain mostly unboxed, with the main action aligned near the lower edge.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 12px / 12px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgb(59, 59, 59), and border 0px rgb(255, 255, 255). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Original dark interface diagrams can convey layered workflows and activity. Avoid copying screenshots, customer marks or source product content.

**Motion.** Observed CSS transition declarations include `border-color, background 0.1s`, `color, background 0.1s`, `border, background-color, color, box-shadow, opacity, filter, transform 0.16s`, `background-color 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Assured, economical and product-focused; concise labels support more detailed workflow explanations.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
