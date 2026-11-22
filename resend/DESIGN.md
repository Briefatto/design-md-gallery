---
version: alpha
name: "Resend"
description: "Resend's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Resend."
colors:
  primary: "rgb(240, 240, 240)"
  background: "rgb(0, 0, 0)"
  surface: "rgb(11, 14, 20)"
  foreground: "rgb(240, 240, 240)"
  muted: "rgb(171, 171, 171)"
  border: "rgba(214, 235, 253, 0.19)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgba(70, 254, 165, 0.83)"
typography:
  display:
    fontFamily: 'domaine, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'domaine, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  heading:
    fontFamily: 'aBCFavorit, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  body:
    fontFamily: '"Inter Website", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Inter Website", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 0px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 48px
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

# Resend DESIGN.md

## Overview

A near-black email platform site contrasts elegant high-contrast serif display type with quiet sans-serif interface copy and dense monospace code examples. Subtle metallic light, texture and small green status marks provide depth.

Built from [/](https://resend.com/) and [/pricing](https://resend.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(240, 240, 240)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 0)` | Page canvas |
| surface | `rgb(11, 14, 20)` | Panels and cards |
| foreground | `rgb(240, 240, 240)` | Primary text |
| muted | `rgb(171, 171, 171)` | Supporting text |
| border | `rgba(214, 235, 253, 0.19)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgba(70, 254, 165, 0.83)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | domaine | 96px | 400 | 1 | -0.01em |
| display-mobile | domaine | 64px | 400 | 1 | -0.01em |
| heading | aBCFavorit | 20px | 400 | 1.3 | 0em |
| body | "Inter Website" | 18px | 400 | 1.5 | 0em |
| action | "Inter Website" | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: aBCFavorit; src: url("https://resend.com/_next/static/immutable/media/abc_favorit_book.p.2svqvtuar83ra.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: aBCFavorit; src: url("https://resend.com/_next/static/immutable/media/abc_favorit_medium.p.25jbl6miwtyjw.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: domaine; src: url("https://resend.com/_next/static/immutable/media/domaine_regular.p.2joc-huu8rdu_.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: domaine; src: url("https://resend.com/_next/static/immutable/media/domaine_medium.p.180pom31p-fh2.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: domaine; src: url("https://resend.com/_next/static/immutable/media/domaine_bold.p.3n2td7ookua-p.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: normal; }
@font-face { font-family: "Inter Website"; src: url("https://resend.com/fonts/website/inter.eb71fd6b.woff2") format("woff2"); font-weight: 100 900; font-display: swap; }
@font-face{font-family:aBCFavorit;src:url("https://resend.com/_next/static/immutable/media/abc_favorit_book.p.2svqvtuar83ra.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:aBCFavorit;src:url("https://resend.com/_next/static/immutable/media/abc_favorit_medium.p.25jbl6miwtyjw.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:domaine;src:url("https://resend.com/_next/static/immutable/media/domaine_regular.p.2joc-huu8rdu_.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:domaine;src:url("https://resend.com/_next/static/immutable/media/domaine_medium.p.180pom31p-fh2.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:domaine;src:url("https://resend.com/_next/static/immutable/media/domaine_bold.p.3n2td7ookua-p.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Use a spacious desktop hero with left-aligned copy and a restrained abstract visual; center and stack the same roles on mobile. Pricing centers the title, category switch and volume slider above a repeated row of dark plan panels that stack at narrow widths.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 58px high, with 0px left and 0px right padding. The sampled header is static, 64px high, with 16px left and 16px right padding.

Measured desktop grid tracks: `157.766px 157.781px 157.781px 157.766px 157.781px 157.781px` with gap `normal 16px`; `157.766px 157.781px 157.781px 157.766px 157.781px 157.781px` with gap `normal 16px`; `600px 600px` with gap `32px`. Build them as a fluid grid. Sampled container maximum widths: `480px`, `512px`, `1024px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use low-contrast dark actions with subtle outlines, compact segmented controls, understated sliders, small green feature checks and code panels. Keep surfaces close to black so hierarchy depends on type, spacing and carefully lit borders.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 58px, horizontal padding 12px / 12px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(240, 240, 240). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses abstract black sculptural objects, soft light streaks and code demonstrations. Recreate the atmosphere with original geometry and generic code snippets, excluding product artwork, source copy and customer marks.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.2s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.15s`, `transform, translate, scale, rotate 0.15s`, `all 0.5s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Measured, developer-oriented and concise, with clear delivery, usage and integration terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
