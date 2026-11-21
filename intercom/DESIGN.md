---
version: alpha
name: "Intercom"
description: "Intercom's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Intercom."
colors:
  primary: "rgb(17, 17, 17)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(250, 249, 246)"
  foreground: "rgb(17, 17, 17)"
  muted: "oklab(0 0 0 / 0.6)"
  border: "rgb(222, 219, 214)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.037em
  display-mobile:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  heading:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.033em
  body:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: 'SaansMono, "SaansMono Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-monospace, monospace'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.1em
  display-emphasis:
    fontFamily: 'Serrif, "Serrif Fallback", "Hiragino Mincho ProN", "Yu Mincho", "Noto Serif JP", ui-serif, Georgia, serif'
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.4
    letterSpacing: -0.01em
rounded:
  control: 4px
  card: 0px
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

# Intercom DESIGN.md

## Overview

A refined editorial customer-service system pairs light Saans statements, Serrif supporting prose and small SaansMono labels with white space and warm neutral surfaces.

Built from [/](https://intercom.com/) and [/pricing](https://intercom.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(17, 17, 17)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(250, 249, 246)` | Panels and cards |
| foreground | `rgb(17, 17, 17)` | Primary text |
| muted | `oklab(0 0 0 / 0.6)` | Supporting text |
| border | `rgb(222, 219, 214)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Saans | 64px | 400 | 1 | -0.037em |
| display-mobile | Saans | 40px | 400 | 0.95 | -0.03em |
| heading | Saans | 48px | 400 | 1 | -0.033em |
| body | Saans | 14px | 400 | 1.4 | 0em |
| action | SaansMono | 12px | 400 | 1.3 | 0.1em |
| display-emphasis | Serrif | 16px | 300 | 1.4 | -0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Saans; src: url("https://www.intercom.com/_next/static/immutable/media/Saans_Regular-s.0y32wrc-1quhd.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: Saans; src: url("https://www.intercom.com/_next/static/immutable/media/Saans_Medium-s.30fecupmfg4ht.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: SaansMono; src: url("https://www.intercom.com/_next/static/immutable/media/SaansMono_Light-s.0ume0g23n3dzv.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: SaansMono; src: url("https://www.intercom.com/_next/static/immutable/media/SaansMono_Regular-s.2_pi34rl7_j33.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: Serrif; src: url("https://www.intercom.com/_next/static/immutable/media/Serrif_Light_subset-s.0xcw-beyjla6z.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: Serrif; src: url("https://www.intercom.com/_next/static/immutable/media/Serrif_Regular_subset-s.01dfn90lujsv9.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage statement amid small photographic crops, then use a wide two-product demonstration section. Pricing uses a fine-ruled multi-plan table with a separate AI-agent column; the mobile version stacks complete plans and their feature lists.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 108px high, with 0px left and 0px right padding. The sampled nav is static, 40px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px 102.656px` with gap `normal 16px`; `subgrid [] [] [] [] [] [] [] [] [] [] [] [] []` with gap `normal`; `subgrid [] [] [] [] [] [] [] [] [] [] [] [] []` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `640.32px`, `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Near-black filled actions, thin outlines, square-edged comparison rules and quiet beige panels keep the interface economical. Small mono labels and blue promotional figures provide precise secondary hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 12px / 12px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Human photographic details, soft abstract textures and realistic inbox or agent demonstrations balance the technical product material.

**Motion.** Observed CSS transition declarations include `top 0.25s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Composed and human, with concise headings and editorial explanatory prose.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
