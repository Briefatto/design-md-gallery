---
version: alpha
name: "Lovart"
description: "Lovart's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Lovart."
colors:
  primary: "rgb(44, 44, 44)"
  background: "rgb(249, 248, 246)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgba(0, 0, 0, 0.9)"
  muted: "rgba(0, 0, 0, 0.55)"
  border: "rgba(0, 0, 0, 0.1)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(225, 255, 103)"
typography:
  display:
    fontFamily: 'featureDisplay, "featureDisplay Fallback", "Noto Serif SC Variable", "Noto Serif TC Variable", "Noto Serif JP Variable", "Noto Serif KR Variable", ui-serif, Georgia, "Times New Roman", serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'featureDisplay, "featureDisplay Fallback", "Noto Serif SC Variable", "Noto Serif TC Variable", "Noto Serif JP Variable", "Noto Serif KR Variable", ui-serif, Georgia, "Times New Roman", serif'
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  heading:
    fontFamily: 'featureDisplay, "featureDisplay Fallback", "Noto Serif SC Variable", "Noto Serif TC Variable", "Noto Serif JP Variable", "Noto Serif KR Variable", ui-serif, Georgia, "Times New Roman", serif'
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  body:
    fontFamily: 'inter, "inter Fallback", system-ui, ui-sans-serif, -apple-system, system-ui, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
    letterSpacing: 0em
  action:
    fontFamily: 'inter, "inter Fallback", system-ui, ui-sans-serif, -apple-system, system-ui, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
    letterSpacing: 0em
rounded:
  control: 9999px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 27.2px
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

# Lovart DESIGN.md

## Overview

A creative tool combines a quiet public creation workspace with a warmer editorial pricing site. Inter handles the compact utility layer; featureDisplay serif headings give the marketing page its character. Charcoal actions and an acid-lime signal sit over white and warm off-white surfaces.

Built from [/](https://www.lovart.ai/) and [/pricing](https://www.lovart.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(44, 44, 44)` | Priority actions and selected emphasis |
| background | `rgb(249, 248, 246)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgba(0, 0, 0, 0.9)` | Primary text |
| muted | `rgba(0, 0, 0, 0.55)` | Supporting text |
| border | `rgba(0, 0, 0, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(225, 255, 103)` | Selective emphasis in headings, graphics, and small signals |



Use charcoal as the stable action color and acid lime as a selective announcement, badge, or recommended-plan signal. The warm canvas and white surfaces should keep artwork and controls distinct. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | featureDisplay | 56px | 400 | 1.25 | 0em |
| display-mobile | featureDisplay | 30px | 400 | 1.25 | 0em |
| heading | featureDisplay | 30px | 400 | 1.25 | 0em |
| body | inter | 14px | 400 | 1.57 | 0em |
| action | inter | 13px | 400 | 1.54 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: inter; src: url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/Inter_Variable-s.37ot7fjk1n7ak.woff2") format("woff2"); font-display: swap; font-weight: 100 900; font-style: normal; }
@font-face { font-family: inter; src: url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/Inter_Italic_Variable-s.05ci792g-jfby.woff2") format("woff2"); font-display: swap; font-weight: 100 900; font-style: italic; }
@font-face { font-family: featureDisplay; src: url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_Regular_Web-s.p.15okwp9-8254o.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: featureDisplay; src: url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_RegularItalic_Web-s.p.0s_s3gu3ebr02.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: featureDisplay; src: url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_Medium_Web-s.p.1r1l7yt36wzfm.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face{font-family:inter;src:url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/Inter_Variable-s.37ot7fjk1n7ak.woff2")format("woff2");font-display:swap;font-weight:100 900;font-style:normal}
@font-face{font-family:inter;src:url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/Inter_Italic_Variable-s.05ci792g-jfby.woff2")format("woff2");font-display:swap;font-weight:100 900;font-style:italic}
@font-face{font-family:featureDisplay;src:url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_Regular_Web-s.p.15okwp9-8254o.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:featureDisplay;src:url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_RegularItalic_Web-s.p.0s_s3gu3ebr02.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:featureDisplay;src:url("https://web-static3.lovart.ai/lovart_prd/static/_next/static/media/FeatureDisplay_Medium_Web-s.p.1r1l7yt36wzfm.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

The public homepage uses a left utility rail, centered prompt composer, small category chips, tool thumbnails, and an exploration feed. The pricing page switches to a slim horizontal navigation, centered serif introduction, billing controls, and aligned plan panels. Mobile collapses the rail and stacks both workflows.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 27.2px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 56px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `733px` with gap `normal`; `168px 168px 168px 168px 168px 168px` with gap `16px`; `315px 315px 315px 315px` with gap `20px`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 1px 2px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact charcoal pill actions, a generously rounded white composer, small outlined category chips, tabbed exploration controls, and low-contrast plan panels. Acid lime highlights an announcement or recommended tier; it is not the default long-form text color.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 9px / 9px, and gap 2px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use only original artwork and generic creative-tool thumbnails, with restrained rounded corners and neutral framing.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `all 0.5s`, `all 0.2s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Inviting and creative, with concise instructions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

