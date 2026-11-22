---
version: alpha
name: "ElevenLabs"
description: "ElevenLabs's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with ElevenLabs."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(253, 252, 252)"
  surface: "rgb(253, 252, 252)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(119, 113, 105)"
  border: "rgb(229, 229, 229)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Waldenburg, "Waldenburg Fallback"'
    fontSize: 44px
    fontWeight: 300
    lineHeight: 1.09
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'Waldenburg, "Waldenburg Fallback"'
    fontSize: 36px
    fontWeight: 300
    lineHeight: 1.17
    letterSpacing: -0.02em
  heading:
    fontFamily: 'Waldenburg, "Waldenburg Fallback"'
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.13
    letterSpacing: 0em
  body:
    fontFamily: 'Inter, "Inter Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  action:
    fontFamily: 'Inter, "Inter Fallback"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
rounded:
  control: 9999px
  card: 16px
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

# ElevenLabs DESIGN.md

## Overview

An audio and voice platform uses near-white surfaces, spare Waldenburg display lettering, compact Inter interface text and black pill actions. Color is concentrated in rich, textured media demonstrations rather than the surrounding controls.

Built from [/](https://elevenlabs.io/) and [/pricing](https://elevenlabs.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(253, 252, 252)` | Page canvas |
| surface | `rgb(253, 252, 252)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(119, 113, 105)` | Supporting text |
| border | `rgb(229, 229, 229)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Waldenburg | 44px | 300 | 1.09 | -0.02em |
| display-mobile | Waldenburg | 36px | 300 | 1.17 | -0.02em |
| heading | Waldenburg | 32px | 300 | 1.13 | 0em |
| body | Inter | 14px | 400 | 1.5 | 0.01em |
| action | Inter | 14px | 500 | 1.5 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Waldenburg; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Buch-latin.1f7863d3c4317f3d.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); font-weight: 300; font-style: normal; font-display: swap; }
@font-face { font-family: Waldenburg; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Normal-latin.47fcefe5bf77b4e5.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Waldenburg; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Fett-latin.e6b0db8ee0a63897.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/ba9851c3c22cd980-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/21350d82a1f187e9-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/c5fe6dc8356a8c31-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/19cfc7226ec3afaa-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/df0a9ae256c0569c-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/8e9860b6e62d6359-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/e4af272ccee01ff0-s.p.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face{font-family:Waldenburg;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Buch-latin.1f7863d3c4317f3d.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");font-weight:300;font-style:normal;font-display:swap}
@font-face{font-family:Waldenburg;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Normal-latin.47fcefe5bf77b4e5.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Waldenburg;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/chunks/src/app/_ui/fonts/waldenburg/KMR-Waldenburg-Fett-latin.e6b0db8ee0a63897.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/ba9851c3c22cd980-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/21350d82a1f187e9-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/c5fe6dc8356a8c31-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+1f??}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/19cfc7226ec3afaa-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+0370-0377,u+037a-037f,u+0384-038a,u+038c,u+038e-03a1,u+03a3-03ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/df0a9ae256c0569c-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/8e9860b6e62d6359-s.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c4,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://eleven-public-cdn.elevenlabs.io/marketing_website/_next/static/media/e4af272ccee01ff0-s.p.woff2?dpl=5ad643d8b5061275004af948f89d258e45d57ead") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column desktop introduction above a large tabbed product demonstration. Mobile stacks the introduction and keeps a focused media specimen within the panel. Pricing uses a horizontally arranged plan comparison; narrow captures retain horizontal plan browsing rather than showing every plan at once.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is static, 36px high, with 0px left and 0px right padding. The sampled nav is static, 36px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `114.641px 758.703px 114.656px` with gap `normal 64px`; `85px 85px 85px 85px 85px 85px 85px 85px 85px 85px 85px 85px` with gap `44px 12px`; `85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px 85.1562px` with gap `normal 12px`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use black pill actions, pale outlined companions, segmented product tabs, rounded demonstration panels, compact playback controls and lightly outlined pricing columns. Keep the neutral control system separate from the vivid media artwork.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 14px / 14px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 16px, radius 0px, background rgb(255, 255, 255), and border 0px rgb(229, 229, 229). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses luminous textured spheres and audio or video demonstrations. Create original abstract media forms and generic playback interfaces without copying artwork, voices, recordings, screenshots or brand marks.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, text-decoration-color, fill, stroke 0.2s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `background-color, color, box-shadow, border-color 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, concise and product-oriented, with practical labels for creation, playback and integration.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
