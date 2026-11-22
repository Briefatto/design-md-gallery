---
version: alpha
name: "Clay"
description: "Clay's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Clay."
colors:
  primary: "rgb(203, 216, 16)"
  background: "rgb(254, 253, 251)"
  surface: "rgb(244, 243, 240)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(123, 121, 116)"
  border: "rgba(123, 121, 116, 0.15)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(3, 93, 68)"
typography:
  display:
    fontFamily: 'Roobertvf, Arial, sans-serif'
    fontSize: 88px
    fontWeight: 575
    lineHeight: 1
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'Roobertvf, Arial, sans-serif'
    fontSize: 41.6px
    fontWeight: 575
    lineHeight: 1
    letterSpacing: -0.04em
  heading:
    fontFamily: 'Roobertvf, Arial, sans-serif'
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.02em
  body:
    fontFamily: 'Roobertvf, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'Roobertvf, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 12px
  card: 18px
spacing:
  xs: 4.5px
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

# Clay DESIGN.md

## Overview

A revenue-workflow platform combines a deep green, illustration-led introduction with bright lime actions, warm neutral surfaces and clear Roobert typography. Pricing adds a distinctive set of brightly colored plan headers above restrained comparison content.

Built from [/](https://clay.com/) and [/pricing](https://clay.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(203, 216, 16)` | Priority actions and selected emphasis |
| background | `rgb(254, 253, 251)` | Page canvas |
| surface | `rgb(244, 243, 240)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(123, 121, 116)` | Supporting text |
| border | `rgba(123, 121, 116, 0.15)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(3, 93, 68)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

The portable neutral card uses an observed near-white canvas and dark text. Deep green remains a section and accent role; light text is reserved for the source hero rather than paired with light cards.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Roobertvf | 88px | 575 | 1 | -0.04em |
| display-mobile | Roobertvf | 41.6px | 575 | 1 | -0.04em |
| heading | Roobertvf | 44px | 500 | 1.1 | -0.02em |
| body | Roobertvf | 14px | 500 | 1.5 | 0em |
| action | Roobertvf | 16px | 500 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Roobertvf; src: url("https://cdn.prod.website-files.com/61477f2c24a826836f969afe/6a1e067cbcc79b9f76bb28f5_RoobertVF.woff2") format("woff2"); font-weight: 300 900; font-style: normal; font-display: swap; }
@font-face { font-family: Roobertvf; src: url("https://cdn.prod.website-files.com/61477f2c24a826836f969afe/69725ade5962e8042ad57236_035407a8acc8ca39ff50fd6c4f9765f6_RoobertItalicsVF.woff2") format("woff2"); font-weight: 300 900; font-style: italic; font-display: swap; }
@font-face{font-family:Roobertvf;src:url("https://cdn.prod.website-files.com/61477f2c24a826836f969afe/6a1e067cbcc79b9f76bb28f5_RoobertVF.woff2")format("woff2");font-weight:300 900;font-style:normal;font-display:swap}
@font-face{font-family:Roobertvf;src:url("https://cdn.prod.website-files.com/61477f2c24a826836f969afe/69725ade5962e8042ad57236_035407a8acc8ca39ff50fd6c4f9765f6_RoobertItalicsVF.woff2")format("woff2");font-weight:300 900;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Let a large dimensional landscape lead the homepage, then place a broad headline and actions above rounded proof and feature sections. Pricing uses aligned plan columns with colored summaries, usage selectors and long feature lists. Mobile stacks the plan columns and keeps the illustration above the main copy.

Spacing scale: xs 4.5px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is static, 57.7656px high, with 0px left and 0px right padding. The sampled nav is static, 57.7656px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `128px 128px 128px 128px 128px 128px 128px 128px 128px` with gap `16px`; `204.797px 204.797px 204.797px 204.797px 204.812px` with gap `24px 40px`; `204.797px 204.797px 204.797px 204.797px 204.812px` with gap `24px 40px`. Build them as a fluid grid. Sampled container maximum widths: `640px`, `2000px`, `1280px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `18px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use modestly rounded priority actions, warm neutral cards, pill-like labels, thin comparison rules and repeated usage selectors. Color-coded plan headers distinguish categories; avoid applying every plan color to unrelated controls.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 47px, horizontal padding 18px / 18px, and gap 9px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 56px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses playful dimensional landscapes, workflow objects and product demonstrations. Create original sculptural scenes and generic workflow diagrams without copying the illustrated objects, screenshots or customer marks.

**Motion.** Observed CSS transition declarations include `background-color 0.3s`, `background-color 0.25s`, `background-color 0.26s`, `opacity 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, playful and practical, with concise workflow and growth terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
