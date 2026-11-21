---
version: alpha
name: "Shopify"
description: "Shopify's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Shopify."
colors:
  primary: "rgb(255, 255, 255)"
  background: "rgb(2, 9, 10)"
  surface: "rgb(16, 38, 32)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(161, 161, 170)"
  border: "rgb(30, 44, 49)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(149, 191, 71)"
typography:
  display:
    fontFamily: 'Shopify-Inter, Helvetica, Arial, sans-serif'
    fontSize: 96px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'Shopify-Inter, Helvetica, Arial, sans-serif'
    fontSize: 36px
    fontWeight: 330
    lineHeight: 1.12
    letterSpacing: -0.02em
  heading:
    fontFamily: 'Shopify-Inter, Helvetica, Arial, sans-serif'
    fontSize: 36px
    fontWeight: 330
    lineHeight: 1.12
    letterSpacing: -0.02em
  body:
    fontFamily: 'Shopify-Inter, Helvetica, Arial, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: 'Shopify-Inter, Helvetica, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 9999px
  card: 0px
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

# Shopify DESIGN.md

## Overview

A commerce platform uses dark near-black and forest-toned surfaces, large light sans-serif headlines, white pill actions and expansive business photography. Lime signals and selective colorful product sections add emphasis without replacing the dark foundation.

Built from [/](https://shopify.com/) and [/pricing](https://shopify.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 255, 255)` | Priority actions and selected emphasis |
| background | `rgb(2, 9, 10)` | Page canvas |
| surface | `rgb(16, 38, 32)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(161, 161, 170)` | Supporting text |
| border | `rgb(30, 44, 49)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(149, 191, 71)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Shopify-Inter | 96px | 300 | 1.08 | -0.02em |
| display-mobile | Shopify-Inter | 36px | 330 | 1.12 | -0.02em |
| heading | Shopify-Inter | 36px | 330 | 1.12 | -0.02em |
| body | Shopify-Inter | 18px | 400 | 1.4 | 0em |
| action | Shopify-Inter | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Shopify-Inter; src: url("https://shopify-assets.shopifycdn.com/b/shopify-brochure2-assets/b2ba26f35a9189c443bbbd74242e6b0e.woff2") format("woff2"); font-style: normal; font-display: optional; font-weight: 100 900; unicode-range: U+0-19F, U+1B1-24F, U+250-2FF, U+300-36F, U+2000-218F, U+2190-22FF, U+2400-27BF, U+FB00-FB4F, U+FEFF, U+FFFD; }
@font-face { font-family: Shopify-Inter; src: url("https://shopify-assets.shopifycdn.com/b/shopify-brochure2-assets/5678e3c531039ef886c19698d9ca403a.woff2") format("woff2"); font-style: normal; font-display: swap; font-weight: 100 900; unicode-range: U+1A0-1A1, U+1AF-1B0, U+1E00-1EFF; }
@font-face { font-family: Shopify-Inter; src: url("https://shopify-assets.shopifycdn.com/b/shopify-brochure2-assets/b8de81e471b1644e9ab09f75751443bf.woff2") format("woff2"); font-style: normal; font-display: swap; font-weight: 100 900; unicode-range: U+400-52F; }
@font-face { font-family: Shopify-Inter; src: url("https://shopify-assets.shopifycdn.com/b/shopify-brochure2-assets/4a4ddbf76d541b9bfb47d7ae74bbe766.woff2") format("woff2"); font-style: normal; font-display: swap; font-weight: 100 900; unicode-range: U+370-3FF; }
@font-face { font-family: Shopify-Inter; src: url("https://shopify-assets.shopifycdn.com/b/shopify-brochure2-assets/b2ba26f35a9189c443bbbd74242e6b0e.woff2") format("woff2"); font-style: normal; font-display: swap; font-weight: 100 900; unicode-range: U+0-19F, U+1B1-24F, U+250-2FF, U+300-36F, U+2000-218F, U+2190-22FF, U+2400-27BF, U+FB00-FB4F, U+FEFF, U+FFFD; }
```

The full fallback stacks are in the front matter.

## Layout

Place the homepage introduction over full-width cinematic media, followed by large rounded feature bands and product demonstrations. Pricing combines a media-led introduction with detailed plan comparisons; mobile gives priority to narrow browsable plan cards and stacked feature sections.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 72px high, with 90px left and 90px right padding. The sampled nav is static, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `1440px` with gap `0px normal`; `1440px` with gap `64px normal`; `1440px` with gap `64px normal`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use white pill actions on dark surfaces, fine outlined companions, small billing toggles, broad rounded section corners and restrained dark plan panels. Keep dense comparison text clearly separated from the larger editorial media sections.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 56px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(229, 231, 235). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source relies on business photography, merchant stories and commerce demonstrations. Use original licensed photography and generic commerce diagrams without copying people, storefronts, screenshots or organization marks.

**Motion.** Observed CSS transition declarations include `opacity, translate 0.3s`, `all 0.15s`, `transform, translate, scale, rotate 0.3s`, `opacity 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, encouraging and practical, with concise actions and clear commerce capability descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
