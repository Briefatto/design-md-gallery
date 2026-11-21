---
version: alpha
name: "Vercel"
description: "Vercel's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Vercel."
colors:
  primary: "rgb(23, 23, 23)"
  background: "rgb(250, 250, 250)"
  surface: "rgb(250, 250, 250)"
  foreground: "rgb(23, 23, 23)"
  muted: "rgb(77, 77, 77)"
  border: "oklab(0.999998 -0.00000980496 0.0000234246 / 0.4)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'GeistSans, "GeistSans Fallback"'
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.06em
  display-mobile:
    fontFamily: 'GeistSans, "GeistSans Fallback"'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.17
    letterSpacing: -0.06em
  heading:
    fontFamily: 'GeistSans, "GeistSans Fallback"'
    fontSize: 32px
    fontWeight: 450
    lineHeight: 1.25
    letterSpacing: -0.05em
  body:
    fontFamily: 'GeistSans, "GeistSans Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'GeistSans, "GeistSans Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 6px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 72px
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

# Vercel DESIGN.md

## Overview

A nearly monochrome infrastructure site combines large, light Geist headlines with compact product information, pale neutral grounds and very fine dividing rules.

Built from [/](https://vercel.com/) and [/pricing](https://vercel.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(23, 23, 23)` | Priority actions and selected emphasis |
| background | `rgb(250, 250, 250)` | Page canvas |
| surface | `rgb(250, 250, 250)` | Panels and cards |
| foreground | `rgb(23, 23, 23)` | Primary text |
| muted | `rgb(77, 77, 77)` | Supporting text |
| border | `oklab(0.999998 -0.00000980496 0.0000234246 / 0.4)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | GeistSans | 64px | 400 | 1 | -0.06em |
| display-mobile | GeistSans | 48px | 400 | 1.17 | -0.06em |
| heading | GeistSans | 32px | 450 | 1.25 | -0.05em |
| body | GeistSans | 14px | 400 | 1.43 | 0em |
| action | GeistSans | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: GeistSans; src: url("https://vercel.com/vc-ap-vercel-marketing/_next/static/immutable/media/Geist_Variable-s.p.2wz-lhd5-5z0-.woff2") format("woff2"); font-display: swap; font-weight: 100 900; }
@font-face{font-family:GeistSans;src:url("https://vercel.com/vc-ap-vercel-marketing/_next/static/immutable/media/Geist_Variable-s.p.2wz-lhd5-5z0-.woff2")format("woff2");font-display:swap;font-weight:100 900}
```

The full fallback stacks are in the front matter.

## Layout

Use an expansive two-column desktop hero with a large geometric centerpiece and actions near the title. The mobile hero centers the visual above the copy and stacks full-width actions. Pricing uses three quiet columns that become a vertical sequence on narrow screens.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 72px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 0px left and 0px right padding. The sampled header is relative, 200px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px` with gap `4px 20px`; `97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px` with gap `4px 20px`; `97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px 97.6562px` with gap `4px 20px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`, `444px`, `673.343px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 2px 2px 0px, rgb(250, 250, 250) 0px 0px 0px 1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact pill-shaped black and white actions, subdued badges, small technical icons and thin separators. Keep plan descriptions and feature lists aligned to a consistent edge rather than enclosing every block in a heavy card.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 6px / 6px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 36px, radius 0px, background rgb(255, 255, 255), and border 0px rgb(235, 235, 235). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The homepage centers a large black geometric brand symbol and restrained product imagery. Use original abstract infrastructure diagrams without reproducing the mark or customer logos.

**Motion.** Observed CSS transition declarations include `opacity 0.3s`, `all 0.15s`, `opacity 1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Concise, technical and confident, with short actions and specific capability names.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
