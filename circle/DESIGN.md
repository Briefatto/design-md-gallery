---
version: alpha
name: "Circle"
description: "Circle's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Circle."
colors:
  primary: "rgb(54, 85, 229)"
  background: "rgb(15, 15, 53)"
  surface: "rgb(15, 15, 53)"
  foreground: "rgb(250, 250, 250)"
  muted: "rgba(255, 255, 255, 0.6)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(62, 27, 201)"
typography:
  display:
    fontFamily: 'Inter'
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.023em
  display-mobile:
    fontFamily: 'Inter'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.037em
  heading:
    fontFamily: 'Inter, sans-serif'
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.025em
  body:
    fontFamily: 'Inter, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, sans-serif'
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.014em
  action:
    fontFamily: 'Inter, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, sans-serif'
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.56
    letterSpacing: -0.028em
rounded:
  control: 9999px
  card: 20px
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

# Circle DESIGN.md

## Overview

A community platform pairs a deep indigo, aurora-like homepage introduction with bold Inter headlines, rounded conversion controls and colorful product demonstrations. The pricing route switches to a bright, card-based presentation.

Built from [/](https://circle.so/) and [/pricing](https://circle.so/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(54, 85, 229)` | Priority actions and selected emphasis |
| background | `rgb(15, 15, 53)` | Page canvas |
| surface | `rgb(15, 15, 53)` | Panels and cards |
| foreground | `rgb(250, 250, 250)` | Primary text |
| muted | `rgba(255, 255, 255, 0.6)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(62, 27, 201)` | Selective emphasis in headings, graphics, and small signals |



The captured priority actions use a blue-to-violet gradient. The primary token selects a measured blue for portable flat controls; recreate gradient composition separately when it is appropriate to the new interface. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Inter | 64px | 700 | 1.1 | -0.023em |
| display-mobile | Inter | 40px | 700 | 1.2 | -0.037em |
| heading | Inter | 20px | 500 | 1.4 | -0.025em |
| body | Inter | 18px | 500 | 1.33 | -0.014em |
| action | Inter | 18px | 500 | 1.56 | -0.028em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; src: url("https://circle.so/_next/static/immutable/media/Inter_latin.p.45535valc9rzk.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; src: url("https://circle.so/_next/static/immutable/media/Inter_latin_ext.0szrwpqb9mkwe.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; src: url("https://circle.so/_next/static/immutable/media/Inter_cyrillic_ext.03ez25a9g3i0n.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; src: url("https://circle.so/_next/static/immutable/media/Inter_cyrillic.3i9rha7jpxn0q.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+1F00-1FFF; src: url("https://circle.so/_next/static/immutable/media/Inter_greek_ext.2o7ko1d-5m1xu.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; src: url("https://circle.so/_next/static/immutable/media/Inter_greek.1ee5w62fj497l.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face { font-family: Inter; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; src: url("https://circle.so/_next/static/immutable/media/Inter_vietnamese.1way2z9fj6cig.woff2") format("woff2"); font-display: swap; font-weight: 200 900; font-style: normal; }
@font-face{font-family:Inter;unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;src:url("https://circle.so/_next/static/immutable/media/Inter_latin.p.45535valc9rzk.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF;src:url("https://circle.so/_next/static/immutable/media/Inter_latin_ext.0szrwpqb9mkwe.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F;src:url("https://circle.so/_next/static/immutable/media/Inter_cyrillic_ext.03ez25a9g3i0n.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116;src:url("https://circle.so/_next/static/immutable/media/Inter_cyrillic.3i9rha7jpxn0q.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+1F??;src:url("https://circle.so/_next/static/immutable/media/Inter_greek_ext.2o7ko1d-5m1xu.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF;src:url("https://circle.so/_next/static/immutable/media/Inter_greek.1ee5w62fj497l.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
@font-face{font-family:Inter;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB;src:url("https://circle.so/_next/static/immutable/media/Inter_vietnamese.1way2z9fj6cig.woff2")format("woff2");font-display:swap;font-weight:200 900;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage title and email conversion form within a broad gradient field, followed by product demonstrations and alternating pale feature bands. Desktop pricing uses four tall plan cards; mobile introduces a tabbed plan selector that shows one detailed plan at a time.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 68px high, with 0px left and 0px right padding. The sampled nav is relative, 68px high, with 32px left and 32px right padding.

Measured desktop grid tracks: `156px 156px 156px 156px 156px` with gap `99px`; `156px 156px 156px 156px 156px` with gap `99px`. Build them as a fluid grid. Sampled container maximum widths: `1260px`, `1200px`, `1280px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `20px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use pill-shaped actions, a large rounded email field, compact review badges, softly elevated plan cards, small feature checks and a clear featured-plan ribbon. Keep the dark hero and bright pricing surfaces distinct while retaining the same typography and control geometry.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 13px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses luminous gradient atmosphere, community interface demonstrations and editorial imagery. Create original gradient fields and generic community diagrams without copying screenshots, photos or customer marks.

**Motion.** Observed CSS transition declarations include `all 0.5s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `all 0.2s`, `opacity 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Welcoming, confident and practical, with clear actions and concise descriptions of community, courses and events.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
