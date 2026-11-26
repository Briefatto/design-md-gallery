---
version: alpha
name: "Discord"
description: "Discord's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Discord."
colors:
  primary: "rgb(88, 101, 242)"
  background: "rgb(26, 32, 129)"
  surface: "rgb(0, 0, 0)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.7)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Abcgintodiscordnord, Arial, sans-serif'
    fontSize: 56px
    fontWeight: 700
    lineHeight: 0.86
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'Abcgintodiscordnord, Arial, sans-serif'
    fontSize: 27px
    fontWeight: 700
    lineHeight: 0.89
    letterSpacing: -0.01em
  heading:
    fontFamily: 'Abcgintodiscordnord, Arial, sans-serif'
    fontSize: 36px
    fontWeight: 800
    lineHeight: 0.93
    letterSpacing: -0.01em
  body:
    fontFamily: 'Abcgintodiscord, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.02em
  action:
    fontFamily: 'Abcgintodiscord, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 12px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 56px
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

# Discord DESIGN.md

## Overview

A highly expressive community site combines a deep blue atmospheric canvas, enormous blocky uppercase display type, vivid purple actions, and playful dimensional visual storytelling.

Built from [/](https://discord.com/) and [/nitro](https://discord.com/nitro), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(88, 101, 242)` | Priority actions and selected emphasis |
| background | `rgb(26, 32, 129)` | Page canvas |
| surface | `rgb(0, 0, 0)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.7)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Use the deep blue canvas and white reading text as a stable pair. Reserve blurple for the browser action and use white for a contrasting download-style action. Nitro introduces a separate purple gradient environment. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Abcgintodiscordnord | 56px | 700 | 0.86 | -0.01em |
| display-mobile | Abcgintodiscordnord | 27px | 700 | 0.89 | -0.01em |
| heading | Abcgintodiscordnord | 36px | 800 | 0.93 | -0.01em |
| body | Abcgintodiscord | 16px | 400 | 1.3 | 0.02em |
| action | Abcgintodiscord | 16px | 500 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-family: Abcgintodiscord; src: url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110a451d677abf8340c6da_ABCGintoDiscord-Regular.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Abcgintodiscordnord; src: url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110b10efb84547ce5e8ef7_ABCGintoDiscordNord-Bold.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: Abcgintodiscord; src: url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110a452ee74d65f90c1dc0_ABCGintoDiscord-Medium.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: Abcgintodiscordnord; src: url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/6889f627207aaaa4b432ae38_ABCGintoDiscordNord-BoldItalic.woff2") format("woff2"); font-weight: 700; font-style: italic; font-display: swap; }
@font-face{font-family:Abcgintodiscord;src:url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110a451d677abf8340c6da_ABCGintoDiscord-Regular.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Abcgintodiscordnord;src:url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110b10efb84547ce5e8ef7_ABCGintoDiscordNord-Bold.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:Abcgintodiscord;src:url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/67110a452ee74d65f90c1dc0_ABCGintoDiscord-Medium.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:Abcgintodiscordnord;src:url("https://cdn.prod.website-files.com/6257adef93867e50d84d30e2/6889f627207aaaa4b432ae38_ABCGintoDiscordNord-BoldItalic.woff2")format("woff2");font-weight:700;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a broad split hero with text beside a large visual composition, followed by generously rounded feature panels. Mobile puts the visual first and centers the main message and actions. Nitro has a separate purple/pink gradient context with italic display type and plan cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 56px. Use smaller steps within a control and larger steps between content groups.

The sampled header is absolute, 80px high, with 0px left and 0px right padding. The sampled nav is static, 168px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `105px 105px 105px 105px 90px 90px 90px 90px 90px 90px 90px 90px` with gap `20px`; `105px 105px 105px 105px 90px 90px 90px 90px 90px 90px 90px 90px` with gap `20px`. Build them as a fluid grid. Sampled container maximum widths: `1240px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `16px`. The captured homepage includes 104px and 120px radii on very large media panels. The small sample uses the observed 16px geometry for its compact card; do not treat that as the radius for a full-width feature chapter.

## Components

Use substantial rounded actions, generous feature containers, and clear navigation contrast.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 65px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original playful illustrations and abstract shapes; do not reproduce mascots, UI screenshots, or the wordmark.

**Motion.** Observed CSS transition declarations include `none 0.2s`, `transform, opacity 0.25s, 0.25s`, `background-color 0.25s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Energetic, casual, and welcoming, while keeping controls direct.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
