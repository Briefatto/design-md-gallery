---
version: alpha
name: "Granola"
description: "Granola's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Granola."
colors:
  primary: "rgb(178, 194, 72)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 247, 242)"
  foreground: "rgb(41, 41, 41)"
  muted: "rgb(114, 114, 110)"
  border: "rgb(222, 222, 222)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'quadrant, "quadrant Fallback"'
    fontSize: 86.4px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'quadrant, "quadrant Fallback"'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.02em
  heading:
    fontFamily: 'quadrant, "quadrant Fallback"'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.015em
  body:
    fontFamily: 'melange, "melange Fallback"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: 0em
  action:
    fontFamily: 'melange, "melange Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
    letterSpacing: 0.01em
rounded:
  control: 33554400px
  card: 8px
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

# Granola DESIGN.md

## Overview

A meeting-notes product combines large editorial serif headlines, friendly sans-serif interface text, moss-lime actions and warm neutral surfaces. Layered notepad and call demonstrations give the otherwise quiet pages a tactile quality.

Built from [/](https://granola.ai/) and [/pricing](https://granola.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(178, 194, 72)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 247, 242)` | Panels and cards |
| foreground | `rgb(41, 41, 41)` | Primary text |
| muted | `rgb(114, 114, 110)` | Supporting text |
| border | `rgb(222, 222, 222)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | quadrant | 86.4px | 400 | 0.93 | -0.02em |
| display-mobile | quadrant | 48px | 400 | 0.93 | -0.02em |
| heading | quadrant | 36px | 400 | 1.11 | -0.015em |
| body | melange | 16px | 400 | 1.35 | 0em |
| action | melange | 14px | 400 | 1.29 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: melange; src: url("https://www.granola.ai/_next/static/media/468f6ca7592b58d2-s.p.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: melange; src: url("https://www.granola.ai/_next/static/media/20e854a24a032470-s.p.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: melange; src: url("https://www.granola.ai/_next/static/media/5b7dea13d8cb4b8a-s.p.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: melange; src: url("https://www.granola.ai/_next/static/media/24ab849dc6206ce6-s.p.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: normal; }
@font-face { font-family: melange; src: url("https://www.granola.ai/_next/static/media/cf3c2d32f7e0e5c5-s.p.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: quadrant; src: url("https://www.granola.ai/_next/static/media/c7f97008bd38275e-s.p.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face{font-family:melange;src:url("https://www.granola.ai/_next/static/media/468f6ca7592b58d2-s.p.woff2") format("woff2");font-display:swap;font-weight:300;font-style:normal}
@font-face{font-family:melange;src:url("https://www.granola.ai/_next/static/media/20e854a24a032470-s.p.woff2") format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:melange;src:url("https://www.granola.ai/_next/static/media/5b7dea13d8cb4b8a-s.p.woff2") format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:melange;src:url("https://www.granola.ai/_next/static/media/24ab849dc6206ce6-s.p.woff2") format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:melange;src:url("https://www.granola.ai/_next/static/media/cf3c2d32f7e0e5c5-s.p.woff2") format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:quadrant;src:url("https://www.granola.ai/_next/static/media/c7f97008bd38275e-s.p.woff2") format("woff2");font-display:swap;font-weight:400;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column homepage with a large left-aligned title and download action beside layered product panels. Pricing centers its introduction over three finely divided plan cards, with a vertical plan presentation on mobile. Keep broad whitespace around the expressive display type.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 56px high, with 0px left and 0px right padding. The sampled nav is relative, 56px high, with 8px left and 8px right padding.

Measured desktop grid tracks: `600px 600px` with gap `normal`; `237px` with gap `normal`; `96px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `561.6px`, `748.8px`, `936px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.08) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.25) 0px 12px 32px -8px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use pill-shaped moss-lime actions, quiet neutral companions, small release badges, fine card outlines and soft product-panel depth. Keep functional text concise and let serif typography carry the larger editorial messages.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 56px, horizontal padding 24px / 24px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses notepad demonstrations, call tiles, paper-like textures and small illustrations. Create original generic note and meeting diagrams without copying people, recordings, screenshots or brand artwork.

**Motion.** Observed CSS transition declarations include `background-color, border-color, box-shadow 0.3s, 0.3s, 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.15s`, `all 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.5s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Friendly, conversational and practical, with concise labels and clear next steps.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
