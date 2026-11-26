---
version: alpha
name: "Fin"
description: "Fin's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Fin."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(250, 249, 246)"
  surface: "rgb(241, 238, 233)"
  foreground: "rgb(0, 0, 0)"
  muted: "oklab(0 0 0 / 0.6)"
  border: "oklab(0 0 0 / 0.12)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(255, 86, 0)"
typography:
  display:
    fontFamily: 'Serrif, "Serrif Fallback", "Hiragino Mincho ProN", "Yu Mincho", "Noto Serif JP", ui-serif, Georgia, serif'
    fontSize: 100px
    fontWeight: 300
    lineHeight: 0.95
    letterSpacing: -0.046em
  display-mobile:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: -0.04em
  heading:
    fontFamily: 'Serrif, "Serrif Fallback", "Hiragino Mincho ProN", "Yu Mincho", "Noto Serif JP", ui-serif, Georgia, serif'
    fontSize: 24px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.034em
  body:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.01em
  action:
    fontFamily: 'Saans, "Saans Fallback", "Hiragino Kaku Gothic ProN", "Hiragino Sans", "Yu Gothic UI", "Yu Gothic", Meiryo, "Noto Sans JP", ui-sans-serif, system-ui, sans-serif'
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
rounded:
  control: 0px
  card: 16px
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

# Fin DESIGN.md

## Overview

A customer-agent site pairs oversized editorial serif headlines with compact sans-serif controls, warm white surfaces and sculptural orange imagery. Pricing introduces precise comparison rules and occasional dark navy surfaces.

Built from [/](https://fin.ai/) and [/pricing](https://fin.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(250, 249, 246)` | Page canvas |
| surface | `rgb(241, 238, 233)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `oklab(0 0 0 / 0.6)` | Supporting text |
| border | `oklab(0 0 0 / 0.12)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(255, 86, 0)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Serrif | 100px | 300 | 0.95 | -0.046em |
| display-mobile | Saans | 36px | 400 | 0.9 | -0.04em |
| heading | Serrif | 24px | 300 | 1.2 | -0.034em |
| body | Saans | 18px | 400 | 1.4 | -0.01em |
| action | Saans | 20px | 400 | 1 | -0.02em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Saans; src: url("https://fin.ai/_next/static/immutable/media/Saans_Regular-s.0y32wrc-1quhd.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: Saans; src: url("https://fin.ai/_next/static/immutable/media/Saans_Medium-s.30fecupmfg4ht.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: Serrif; src: url("https://fin.ai/_next/static/immutable/media/Serrif_Light_subset-s.0xcw-beyjla6z.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: Serrif; src: url("https://fin.ai/_next/static/immutable/media/Serrif_Regular_subset-s.01dfn90lujsv9.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
```

The full fallback stacks are in the front matter.

## Layout

Use a broad left-aligned desktop introduction with a large dimensional visual and short paired actions. The mobile homepage centers the introduction and places a product demonstration within the visual. Pricing groups helpdesk options into clearly divided panels, with a distinct dark treatment in the captured mobile state.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 108px high, with 0px left and 0px right padding. The sampled nav is static, 60px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `164.438px 164.453px 164.453px 164.438px 164.453px 164.453px` with gap `56px 32px`; `915.969px 206.703px` with gap `24px`; `915.969px 206.703px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular dark actions, lightly outlined companions, fine orange emphasis rules, warm neutral panels and restrained pricing feature lists. Preserve the contrast between expressive serif display roles and practical sans-serif interface text.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 8px / 8px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses dimensional orange ribbons, abstract textures and chat demonstrations. Create original sculptural forms and generic service-workflow diagrams without copying artwork, conversations, screenshots or customer marks.

**Motion.** Observed CSS transition declarations include `top 0.25s`, `color 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, clear and service-oriented, with practical capability and workflow labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
