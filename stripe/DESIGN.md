---
version: alpha
name: "Stripe"
description: "Stripe's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Stripe."
colors:
  primary: "rgb(83, 58, 253)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(248, 250, 253)"
  foreground: "rgb(6, 27, 49)"
  muted: "rgb(90, 102, 119)"
  border: "rgba(212, 222, 233, 0.75)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(0, 212, 255)"
typography:
  display:
    fontFamily: 'sohne-var, "SF Pro Display", sans-serif'
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'sohne-var, "SF Pro Display", sans-serif'
    fontSize: 34px
    fontWeight: 300
    lineHeight: 1.03
    letterSpacing: -0.01em
  heading:
    fontFamily: 'sohne-var, "SF Pro Display", sans-serif'
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  body:
    fontFamily: 'sohne-var, "SF Pro Display", sans-serif'
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: 'sohne-var, "SF Pro Display", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
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

# Stripe DESIGN.md

## Overview

A financial platform site pairs dark navy typography with vivid violet actions, fine structural rules and expansive multicolor gradient fields. The homepage is editorial and product-led, while pricing uses denser, softly elevated comparison panels.

Built from [/](https://stripe.com/) and [/pricing](https://stripe.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(83, 58, 253)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(248, 250, 253)` | Panels and cards |
| foreground | `rgb(6, 27, 49)` | Primary text |
| muted | `rgb(90, 102, 119)` | Supporting text |
| border | `rgba(212, 222, 233, 0.75)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(0, 212, 255)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | sohne-var | 48px | 300 | 1.15 | -0.02em |
| display-mobile | sohne-var | 34px | 300 | 1.03 | -0.01em |
| heading | sohne-var | 32px | 300 | 1.1 | -0.02em |
| body | sohne-var | 16px | 300 | 1.4 | 0em |
| action | sohne-var | 14px | 400 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:sohne-var;src:url("https://b.stripecdn.com/mkt-ssr-statics/assets/_next/static/media/Sohne.cb178166.woff2") format("woff2-variations");font-weight:1 1000;font-display:block}
@font-face{font-family:sohne-var;src:url("https://b.stripecdn.com/mkt-ssr-statics/assets/_next/static/media/Sohne.cb178166.woff2") format("woff2-variations");font-weight:1 1000;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a wide desktop headline and product story within a disciplined column grid. Let diagonal color fields cross section boundaries without disrupting reading edges. Pricing presents contrasting standard and custom panels; mobile stacks the panels and actions while preserving generous margins.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 76px high, with 0px left and 0px right padding. The sampled header is static, 130.219px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px` with gap `8px 16px`; `88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px` with gap `8px 16px`; `88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px 88px` with gap `8px 16px`. Build them as a fluid grid. Sampled container maximum widths: `1349px`, `1018.56px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small filled violet actions, understated outlined companions, crisp product tiles, fine grid lines and lightly shadowed pricing panels. Dark navy comparison surfaces provide contrast to the pale page ground.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 24px / 24px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 46px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(6, 27, 49). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source combines colorful gradient ribbons and detailed product imagery. Use original gradient compositions and generic financial interface diagrams; exclude logos, customer marks, source screenshots and marketing wording.

**Motion.** Observed CSS transition declarations include `color 1.2s`, `color 0.3s`, `background-color, color, outline-color, border 0.3s, 0.3s, 0.3s, 0.3s`, `color, background-color, border-color 0.24s, 0.24s, 0.24s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Assured, explanatory and precise, with clear benefit statements and practical next steps.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
