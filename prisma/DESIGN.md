---
version: alpha
name: "Prisma"
description: "Prisma's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Prisma."
colors:
  primary: "rgb(21, 21, 21)"
  background: "rgb(255, 255, 255)"
  surface: "oklab(0.969998 -0.00000959635 0.0000227094 / 0.6)"
  foreground: "rgb(21, 21, 21)"
  muted: "rgb(100, 101, 103)"
  border: "rgb(229, 229, 228)"
  on-primary: "rgb(249, 250, 245)"
  accent: "rgb(1, 215, 228)"
typography:
  display:
    fontFamily: 'Sora, "Sora Fallback"'
    fontSize: 62px
    fontWeight: 500
    lineHeight: 1.06
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Sora, "Sora Fallback"'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.06
    letterSpacing: 0em
  heading:
    fontFamily: 'Sora, "Sora Fallback"'
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0em
  body:
    fontFamily: 'Inter, "Inter Fallback"'
    fontSize: 14px
    fontWeight: 380
    lineHeight: 1.63
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, "Inter Fallback"'
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 18px
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

# Prisma DESIGN.md

## Overview

A light developer platform uses large geometric Sora headlines, fine neutral interface structure and soft cyan, yellow and coral color fields. The multicolor atmosphere remains secondary to compact dark actions and clear technical content.

Built from [/](https://prisma.io/) and [/pricing](https://prisma.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(21, 21, 21)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `oklab(0.969998 -0.00000959635 0.0000227094 / 0.6)` | Panels and cards |
| foreground | `rgb(21, 21, 21)` | Primary text |
| muted | `rgb(100, 101, 103)` | Supporting text |
| border | `rgb(229, 229, 228)` | Quiet separators and outlines |
| on-primary | `rgb(249, 250, 245)` | Text on the primary action |
| accent | `rgb(1, 215, 228)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Sora | 62px | 500 | 1.06 | 0em |
| display-mobile | Sora | 40px | 500 | 1.06 | 0em |
| heading | Sora | 38px | 500 | 1.1 | 0em |
| body | Inter | 14px | 380 | 1.63 | 0em |
| action | Inter | 14px | 700 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Sora; font-style: normal; font-weight: 100 800; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/b886574ba42c3409-s.0s8rfyfnf3ili.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Sora; font-style: normal; font-weight: 100 800; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/c41ca59f1c34ba31-s.p.2moef4a_pkre2.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 100 900; font-display: swap; src: url("https://www.prisma.io/site-static/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face{font-family:Sora;font-style:normal;font-weight:100 800;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/b886574ba42c3409-s.0s8rfyfnf3ili.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Sora;font-style:normal;font-weight:100 800;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/c41ca59f1c34ba31-s.p.2moef4a_pkre2.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://www.prisma.io/site-static/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
```

The full fallback stacks are in the front matter.

## Layout

Center the desktop homepage introduction above a large product walkthrough. Keep the mobile introduction left aligned and stack the demonstration below. Pricing uses a left-aligned title above four rounded plan cards that become a vertical list on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is static, 24px high, with 0px left and 0px right padding. The sampled nav is relative, 24px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `488px 488px` with gap `48px`; `445.328px 445.328px 445.344px` with gap `20px`; `24px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `929.38px`, `863.424px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 21, 21, 0.04) 0px 1px 2px 0px, rgba(21, 21, 21, 0.06) 0px 8px 16px -4px, rgba(21, 21, 21, 0.14) 0px 32px 64px -16px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `18px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact black priority actions, outlined companions, rounded white plan cards, fine dividers and small colored feature checks. Keep announcement strips distinct from the main navigation and use restrained badges to identify plan priority.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px lab(90.952 0 -0.0000119209). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses lightly textured multicolor atmosphere and large product demonstrations. Use original color fields and generic developer-workflow diagrams without copying screenshots, brand marks or account content.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, box-shadow 0.15s`, `all 0.15s`, `color 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, technical and practical; explain capability, usage and next steps in concise original language.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
