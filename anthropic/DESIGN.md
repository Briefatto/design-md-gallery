---
version: alpha
name: "Anthropic"
description: "Anthropic's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Anthropic."
colors:
  primary: "rgb(20, 20, 19)"
  background: "rgb(250, 249, 245)"
  surface: "rgb(250, 249, 245)"
  foreground: "rgb(20, 20, 19)"
  muted: "rgb(94, 93, 89)"
  border: "rgb(222, 220, 209)"
  on-primary: "rgb(250, 249, 245)"
  accent: "rgb(217, 119, 87)"
typography:
  display:
    fontFamily: 'anthropicSans, "anthropicSans Fallback", sans-serif'
    fontSize: 40.7843px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'anthropicSans, "anthropicSans Fallback", sans-serif'
    fontSize: 25px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: -0.01em
  heading:
    fontFamily: 'anthropicSans, "anthropicSans Fallback", sans-serif'
    fontSize: 40.7843px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.01em
  body:
    fontFamily: 'anthropicSans, "anthropicSans Fallback", sans-serif'
    fontSize: 14.6863px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'anthropicSans, "anthropicSans Fallback", sans-serif'
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
    letterSpacing: 0.01em
  display-emphasis:
    fontFamily: 'anthropicSerif, "anthropicSerif Fallback", serif'
    fontSize: 40.7843px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.01em
rounded:
  control: 12px
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

# Anthropic DESIGN.md

## Overview

A research-led AI site uses warm off-white surfaces, near-black ink and a deliberate pairing of plain sans-serif and expressive serif text. The corporate homepage reads like an editorial statement, while the Claude product route gives the serif display role more prominence.

Built from [/](https://anthropic.com/) and [/claude](https://anthropic.com/claude), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(20, 20, 19)` | Priority actions and selected emphasis |
| background | `rgb(250, 249, 245)` | Page canvas |
| surface | `rgb(250, 249, 245)` | Panels and cards |
| foreground | `rgb(20, 20, 19)` | Primary text |
| muted | `rgb(94, 93, 89)` | Supporting text |
| border | `rgb(222, 220, 209)` | Quiet separators and outlines |
| on-primary | `rgb(250, 249, 245)` | Text on the primary action |
| accent | `rgb(217, 119, 87)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | anthropicSans | 40.7843px | 600 | 1.25 | -0.01em |
| display-mobile | anthropicSans | 25px | 600 | 1.3 | -0.01em |
| heading | anthropicSans | 40.7843px | 600 | 1.25 | -0.01em |
| body | anthropicSans | 14.6863px | 400 | 1.5 | 0em |
| action | anthropicSans | 13px | 400 | 1.54 | 0.01em |
| display-emphasis | anthropicSerif | 40.7843px | 400 | 1.25 | -0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: anthropicSans; src: url("https://www.anthropic.com/_next/static/media/AnthropicSans_Roman_Web-s.p.1e3n6bt4oqimz.woff2") format("woff2"); font-display: swap; font-style: normal; }
@font-face { font-family: anthropicSans; src: url("https://www.anthropic.com/_next/static/media/AnthropicSans_Italic_Web-s.p.212cqpul8-axk.woff2") format("woff2"); font-display: swap; font-style: italic; }
@font-face { font-family: anthropicSerif; src: url("https://www.anthropic.com/_next/static/media/AnthropicSerif_Roman_Web-s.p.0twp0vwi-lncj.woff2") format("woff2"); font-display: swap; font-style: normal; }
@font-face { font-family: anthropicSerif; src: url("https://www.anthropic.com/_next/static/media/AnthropicSerif_Italic_Web-s.p.1fjksu1uimpf3.woff2") format("woff2"); font-display: swap; font-style: italic; }
@font-face{font-family:anthropicSans;src:url("https://www.anthropic.com/_next/static/media/AnthropicSans_Roman_Web-s.p.1e3n6bt4oqimz.woff2")format("woff2");font-display:swap;font-style:normal}
@font-face{font-family:anthropicSans;src:url("https://www.anthropic.com/_next/static/media/AnthropicSans_Italic_Web-s.p.212cqpul8-axk.woff2")format("woff2");font-display:swap;font-style:italic}
@font-face{font-family:anthropicSerif;src:url("https://www.anthropic.com/_next/static/media/AnthropicSerif_Roman_Web-s.p.0twp0vwi-lncj.woff2")format("woff2");font-display:swap;font-style:normal}
@font-face{font-family:anthropicSerif;src:url("https://www.anthropic.com/_next/static/media/AnthropicSerif_Italic_Web-s.p.1fjksu1uimpf3.woff2")format("woff2");font-display:swap;font-style:italic}
@font-face { font-family: anthropicSans; src: url("https://claude.com/_next/static/media/AnthropicSans_Roman_Web-s.p.050e7498.woff2") format("woff2"); font-display: swap; font-style: normal; }
@font-face { font-family: anthropicSans; src: url("https://claude.com/_next/static/media/AnthropicSans_Italic_Web-s.p.6550bf15.woff2") format("woff2"); font-display: swap; font-style: italic; }
@font-face { font-family: anthropicSerif; src: url("https://claude.com/_next/static/media/AnthropicSerif_Roman_Web-s.p.c28786b4.woff2") format("woff2"); font-display: swap; font-style: normal; }
@font-face { font-family: anthropicSerif; src: url("https://claude.com/_next/static/media/AnthropicSerif_Italic_Web-s.p.43888cc6.woff2") format("woff2"); font-display: swap; font-style: italic; }
@font-face{font-family:anthropicSans;src:url("https://claude.com/_next/static/media/AnthropicSans_Roman_Web-s.p.050e7498.woff2")format("woff2");font-display:swap;font-style:normal}
@font-face{font-family:anthropicSans;src:url("https://claude.com/_next/static/media/AnthropicSans_Italic_Web-s.p.6550bf15.woff2")format("woff2");font-display:swap;font-style:italic}
@font-face{font-family:anthropicSerif;src:url("https://claude.com/_next/static/media/AnthropicSerif_Roman_Web-s.p.c28786b4.woff2")format("woff2");font-display:swap;font-style:normal}
@font-face{font-family:anthropicSerif;src:url("https://claude.com/_next/static/media/AnthropicSerif_Italic_Web-s.p.43888cc6.woff2")format("woff2");font-display:swap;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Keep the corporate introduction broad and text-led, followed by a large media panel and quiet content cards. The product route centers its hero among a loose image collage and repeated feature sections. Mobile narrows the reading measure, stacks media and retains the mixed type hierarchy.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 84px high, with 0px left and 0px right padding. The sampled header is static, 20.0156px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `539px 170px 539px` with gap `normal 16px`; `1440px` with gap `normal`; `416px 416px 416px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `1920px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small quiet navigation pills, restrained dark actions, pale secondary controls, fine separators and softly rounded media or feature panels. Preserve the distinction between corporate editorial blocks and the more product-oriented Claude demonstrations.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 46px, horizontal padding 16px / 16px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 30px, radius 8px, background rgb(245, 244, 237), and border 1px rgb(232, 230, 220). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source combines atmospheric sky imagery, editorial photography and abstract product-adjacent image tiles. Use original licensed imagery and simple diagrams without copying photos, illustrations, marks or source product content.

**Motion.** Observed CSS transition declarations include `transform 0.3s`, `color 0.3s`, `color 0.2s`, `border-color, box-shadow, background-color, color 0.15s, 0.15s, 0.15s, 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Measured, explanatory and thoughtful, with clear actions and carefully structured information.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
