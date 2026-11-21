---
version: alpha
name: "Runway"
description: "Runway's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Runway."
colors:
  primary: "rgb(12, 12, 12)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 247, 247)"
  foreground: "rgb(12, 12, 12)"
  muted: "rgb(102, 110, 122)"
  border: "rgba(0, 0, 0, 0.1)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(43, 34, 250)"
typography:
  display:
    fontFamily: 'abcNormal, "abcNormal Fallback"'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
  display-mobile:
    fontFamily: 'abcNormal, "abcNormal Fallback"'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
  heading:
    fontFamily: 'abcNormal, "abcNormal Fallback"'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
  body:
    fontFamily: 'abcNormal, "abcNormal Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0em
  action:
    fontFamily: 'abcNormal, "abcNormal Fallback"'
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.007em
rounded:
  control: 9999px
  card: 12px
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

# Runway DESIGN.md

## Overview

A creative AI platform uses an economical sans-serif interface around large cinematic media panels. White editorial surfaces, near-black controls and selective electric-blue signals keep the surrounding chrome quiet.

Built from [/](https://runwayml.com/) and [/pricing](https://runwayml.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(12, 12, 12)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 247, 247)` | Panels and cards |
| foreground | `rgb(12, 12, 12)` | Primary text |
| muted | `rgb(102, 110, 122)` | Supporting text |
| border | `rgba(0, 0, 0, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(43, 34, 250)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | abcNormal | 56px | 400 | 1.1 | -0.015em |
| display-mobile | abcNormal | 36px | 400 | 1.1 | -0.015em |
| heading | abcNormal | 36px | 400 | 1.1 | -0.015em |
| body | abcNormal | 14px | 400 | 1.55 | 0em |
| action | abcNormal | 24px | 400 | 1.25 | -0.007em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: abcNormal; src: url("https://runway.com/_next/static/immutable/media/ABCNormal_Book-s.p.21kfti5c116f2.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: abcNormal; src: url("https://runway.com/_next/static/immutable/media/ABCNormal_Regular-s.p.1b_g1ycxls7-a.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: abcNormal; src: url("https://runway.com/_next/static/immutable/media/ABCNormal_Neutral-s.p.2n7_-unbs3n48.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: abcNormal; src: url("https://runway.com/_next/static/immutable/media/ABCNormal_Neutral-s.p.2n7_-unbs3n48.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: normal; }
```

The full fallback stacks are in the front matter.

## Layout

Frame the homepage introduction inside a large rounded media panel, then move into spacious product and editorial sections. Pricing centers its title above audience and billing selectors and a repeated row of plan cards; mobile stacks the plans and keeps controls compact.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 68px high, with 0px left and 0px right padding. The sampled nav is static, 68px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `1400px` with gap `normal`; `456px 456px 456px` with gap `16px`; `456px` with gap `0px normal`. Build them as a fluid grid. Sampled container maximum widths: `896px`, `1024px`, `672px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small dark or light actions according to the surrounding surface, thin outlined companions, segmented selectors, fine plan borders and restrained badges. Media panels may be broadly rounded while dense comparison controls remain compact.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source relies on cinematic moving imagery, stills and creative project examples. Use original licensed media or abstract placeholders rather than copying films, generated scenes, screenshots or partner marks.

**Motion.** Observed CSS transition declarations include `all 0.2s`, `all 0.15s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, confident and creative, with practical product and workflow labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
