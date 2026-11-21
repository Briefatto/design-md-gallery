---
version: alpha
name: "Animejs"
description: "Animejs's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Animejs."
colors:
  primary: "rgb(255, 75, 75)"
  background: "rgb(37, 36, 35)"
  surface: "rgb(37, 36, 35)"
  foreground: "rgb(246, 244, 242)"
  muted: "rgb(180, 177, 175)"
  border: "rgb(53, 52, 50)"
  on-primary: "rgb(37, 36, 35)"
  accent: "rgb(183, 255, 84)"
typography:
  display:
    fontFamily: 'DIN, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 64px
    fontWeight: 700
    lineHeight: 0.87
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'DIN, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.87
    letterSpacing: 0em
  heading:
    fontFamily: 'DIN, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.87
    letterSpacing: 0em
  body:
    fontFamily: 'DIN, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: 0em
  action:
    fontFamily: 'Mono, monospace'
    fontSize: 12px
    fontWeight: 600
    lineHeight: 4
    letterSpacing: 0.01em
rounded:
  control: 4px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
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

# Animejs DESIGN.md

## Overview

An animation-engine site uses warm charcoal surfaces, compact technical labels and heavy, tightly packed DIN headlines. Bright red and multicolor animated geometry bring energy to an otherwise restrained interface.

Built from [/](https://animejs.com/) and [/documentation/](https://animejs.com/documentation/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 75, 75)` | Priority actions and selected emphasis |
| background | `rgb(37, 36, 35)` | Page canvas |
| surface | `rgb(37, 36, 35)` | Panels and cards |
| foreground | `rgb(246, 244, 242)` | Primary text |
| muted | `rgb(180, 177, 175)` | Supporting text |
| border | `rgb(53, 52, 50)` | Quiet separators and outlines |
| on-primary | `rgb(37, 36, 35)` | Text on the primary action |
| accent | `rgb(183, 255, 84)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | DIN | 64px | 700 | 0.87 | 0em |
| display-mobile | DIN | 40px | 700 | 0.87 | 0em |
| heading | DIN | 40px | 700 | 0.87 | 0em |
| body | DIN | 20px | 600 | 1.25 | 0em |
| action | Mono | 12px | 600 | 4 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Mono; src: url("https://animejs.com/assets/fonts/BerkeleyMono-Regular.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Mono; src: url("https://animejs.com/assets/fonts/BerkeleyMono-Italic.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: DIN; src: url("https://animejs.com/assets/fonts/DINish[slnt,wdth,wght].woff2") format("woff2"); font-variation-settings: "wdth" 125; font-weight: 100 900; font-stretch: 50% 125%; font-style: oblique 0deg 12deg; font-display: swap; }
@font-face{font-family:Mono;src:url("https://animejs.com/assets/fonts/BerkeleyMono-Regular.woff2") format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Mono;src:url("https://animejs.com/assets/fonts/BerkeleyMono-Italic.woff2") format("woff2");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:DIN;src:url("https://animejs.com/assets/fonts/DINish[slnt,wdth,wght].woff2") format("woff2");font-variation-settings:"wdth" 125;font-weight:100 900;font-stretch:50% 125%;font-style:oblique 0deg 12deg;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Balance a large left-aligned introductory title with a dominant circular motion demonstration. Documentation adds a narrow category rail, a compact contents column and a main reading area; mobile collapses the rails and stacks the article.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 36px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 72px high, with 24px left and 24px right padding. The sampled nav is relative, 71px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `1500px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small squared technical controls, uppercase monospace labels, subtle panel changes and thin separators. Documentation categories and example panels should feel functional, with selective red emphasis marking the current topic.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 44px, radius 4px 0px 0px 4px, background rgb(53, 52, 50), and border 0px rgb(246, 244, 242). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses animated rings, dots and line geometry. Build original geometric demonstrations rather than copying its exact animation, logos or sponsor artwork.

**Motion.** Observed CSS transition declarations include `transform 0.125s`, `opacity, color 0.125s, 0.125s`, `color 0.1s`. These prove declared timing, not that a particular animation was watched end to end. The captured hero shows different animation stages across viewports. Provide reduced-motion behaviour.

**Voice.** Concise, technical and exploratory, with clear capability names and documentation labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
