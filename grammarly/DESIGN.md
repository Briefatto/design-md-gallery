---
version: alpha
name: "Grammarly"
description: "Grammarly's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Grammarly."
colors:
  primary: "rgb(2, 126, 111)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(245, 245, 245)"
  foreground: "rgb(14, 16, 26)"
  muted: "rgb(112, 112, 112)"
  border: "rgb(217, 217, 217)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(0, 35, 31)"
typography:
  display:
    fontFamily: 'matter, sans-serif'
    fontSize: 46px
    fontWeight: 670
    lineHeight: 1.09
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'matter, sans-serif'
    fontSize: 30px
    fontWeight: 670
    lineHeight: 1.13
    letterSpacing: -0.01em
  heading:
    fontFamily: 'matter, sans-serif'
    fontSize: 36px
    fontWeight: 670
    lineHeight: 1.11
    letterSpacing: -0.01em
  body:
    fontFamily: 'Glyph, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  action:
    fontFamily: 'Glyph, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 6px
  card: 8px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 60px
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

# Grammarly DESIGN.md

## Overview

A writing-assistance site uses strong rounded sans-serif headings, deep teal actions, white surfaces and pale mint plan emphasis. Colorful product demonstrations sit inside a restrained, practical interface.

Built from [/](https://grammarly.com/) and [/pricing](https://grammarly.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(2, 126, 111)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(245, 245, 245)` | Panels and cards |
| foreground | `rgb(14, 16, 26)` | Primary text |
| muted | `rgb(112, 112, 112)` | Supporting text |
| border | `rgb(217, 217, 217)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(0, 35, 31)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | matter | 46px | 670 | 1.09 | -0.01em |
| display-mobile | matter | 30px | 670 | 1.13 | -0.01em |
| heading | matter | 36px | 670 | 1.11 | -0.01em |
| body | Glyph | 14px | 400 | 1.25 | 0em |
| action | Glyph | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Matter; font-style: normal; font-weight: 670; font-display: swap; src: url("https://static-web.grammarly.com/shared/fonts/matter-semi-bold.woff2") format("woff2"); }
@font-face { font-family: Matter; font-style: normal; font-weight: 570; font-display: swap; src: url("https://static-web.grammarly.com/shared/fonts/matter-medium.woff2") format("woff2"); }
@font-face { font-family: Glyph; font-style: normal; font-weight: 400; font-display: swap; src: url("https://static-web.grammarly.com/shared/fonts/glyph-regular.woff2") format("woff2"); }
@font-face { font-family: Glyph; font-weight: 700; font-display: swap; src: url("https://static-web.grammarly.com/shared/fonts/glyph-bold.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: Glyph; font-style: normal; font-weight: 400; src: url("https://static-web.grammarly.com/shared/fonts/glyph-regular.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: Glyph; font-style: normal; font-weight: 500; src: url("https://static-web.grammarly.com/shared/fonts/glyph-medium.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: Glyph; font-style: normal; font-weight: 700; src: url("https://static-web.grammarly.com/shared/fonts/glyph-bold.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: Matter; font-style: normal; font-weight: 670; src: url("https://static-web.grammarly.com/shared/fonts/matter-semi-bold.woff2") format("woff2"); }
@font-face { font-display: swap; font-family: Matter; font-style: normal; font-weight: 570; src: url("https://static-web.grammarly.com/shared/fonts/matter-medium.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction above a wide action group and a three-column feature gallery. Pricing centers its heading above three aligned plan columns, with a mint-filled featured plan and repeated comparison lists. Mobile stacks the feature cards and plan columns.

Spacing scale: xs 8px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 65px high, with 48px left and 48px right padding. The sampled header is static, 116px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px` with gap `16px 32px`; `77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px` with gap `16px 32px`; `77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px 77.3281px` with gap `16px 32px`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact teal filled actions, quiet outlined companions, modestly rounded cards, a clear featured-plan ribbon and small feature checks. Keep body copy and comparison details economical and readable rather than enlarging every label.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 34px, horizontal padding 8px / 8px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 50%, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses writing-interface demonstrations and colorful abstract feature backgrounds. Create original generic writing specimens and simple diagrams without copying source text, screenshots, illustrations or organization marks.

**Motion.** Observed CSS transition declarations include `transform, box-shadow 0.2s, 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, reassuring and practical, with concise descriptions and clear actions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
