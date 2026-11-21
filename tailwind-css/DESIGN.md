---
version: alpha
name: "Tailwind CSS"
description: "Tailwind CSS's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Tailwind CSS."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(255, 255, 255)"
  surface: "lab(98.3189 -4.74921 -0.111711)"
  foreground: "lab(1.90334 0.278696 -5.48866)"
  muted: "lab(47.7841 -0.393182 -10.0268)"
  border: "oklab(0.129999 -0.00404751 -0.027702 / 0.2)"
  on-primary: "rgb(255, 255, 255)"
  accent: "lab(70.687 -23.6078 -45.9483)"
typography:
  display:
    fontFamily: 'inter, "inter Fallback", system-ui'
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.05em
  display-mobile:
    fontFamily: 'inter, "inter Fallback", system-ui'
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.05em
  heading:
    fontFamily: 'inter, "inter Fallback", system-ui'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  body:
    fontFamily: 'inter, "inter Fallback", system-ui'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
    letterSpacing: 0em
  action:
    fontFamily: 'inter, "inter Fallback", system-ui'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: 0em
rounded:
  control: 32px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 64px
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

# Tailwind CSS DESIGN.md

## Overview

A utility-CSS site combines oversized, tightly tracked sans-serif headlines with a white technical grid, dark code panels and selective cyan emphasis. Documentation reduces the display scale while retaining the same precise reading and code roles.

Built from [/](https://tailwindcss.com/) and [/docs/installation/using-vite](https://tailwindcss.com/docs/installation/using-vite), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `lab(98.3189 -4.74921 -0.111711)` | Panels and cards |
| foreground | `lab(1.90334 0.278696 -5.48866)` | Primary text |
| muted | `lab(47.7841 -0.393182 -10.0268)` | Supporting text |
| border | `oklab(0.129999 -0.00404751 -0.027702 / 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `lab(70.687 -23.6078 -45.9483)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | inter | 96px | 400 | 1 | -0.05em |
| display-mobile | inter | 36px | 500 | 1.11 | -0.05em |
| heading | inter | 40px | 500 | 1 | -0.05em |
| body | inter | 14px | 400 | 2 | 0em |
| action | inter | 12px | 400 | 1.67 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: inter; src: url("https://tailwindcss.com/_next/static/media/InterVariable-s.p.0r27kd5h06n72.woff2") format("woff2"); font-display: swap; font-weight: 100 900; font-style: normal; }
@font-face { font-family: inter; src: url("https://tailwindcss.com/_next/static/media/InterVariable_Italic-s.p.0lyls.rsx6v21.woff2") format("woff2"); font-display: swap; font-weight: 100 900; font-style: italic; }
@font-face{font-family:inter;src:url("https://tailwindcss.com/_next/static/media/InterVariable-s.p.0r27kd5h06n72.woff2")format("woff2");font-display:swap;font-weight:100 900;font-style:normal}
@font-face{font-family:inter;src:url("https://tailwindcss.com/_next/static/media/InterVariable_Italic-s.p.0lyls.rsx6v21.woff2")format("woff2");font-display:swap;font-weight:100 900;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use a wide left-aligned homepage introduction above a large code-and-result demonstration. Documentation adds a persistent desktop sidebar, a clear article column and step-by-step command panels. On mobile, collapse the rail, stack code examples and preserve a readable text measure.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is static, 7384px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `14px 245.922px 20.0781px` with gap `4px`; `40px 1360px 40px` with gap `normal`; `1360px` with gap `160px`. Build them as a fluid grid. Sampled container maximum widths: `512px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `32px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact black pill actions, outlined search fields, small version badges, numbered setup steps and dark rounded code panels. Fine hatched gutters and subtle separators establish structure without heavy cards.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source demonstrates interface construction with code and rendered examples. Use original generic examples and simple technical geometry rather than copying the displayed artwork, portraits or screenshots.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Practical, concise and instructional, with clear setup steps and accurate developer terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
