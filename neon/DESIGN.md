---
version: alpha
name: "Neon"
description: "Neon's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Neon."
colors:
  primary: "rgb(255, 255, 255)"
  background: "rgb(0, 0, 0)"
  surface: "rgb(24, 25, 27)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(172, 172, 172)"
  border: "rgb(48, 50, 54)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(52, 213, 154)"
typography:
  display:
    fontFamily: 'Inter, "Inter Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'Inter, "Inter Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  heading:
    fontFamily: 'Inter, "Inter Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  body:
    fontFamily: 'Inter, "Inter Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
  action:
    fontFamily: 'Inter, "Inter Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
rounded:
  control: 33554400px
  card: 10px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 26px
  xl: 28px
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

# Neon DESIGN.md

## Overview

A black-ground database site combines large, restrained Inter headlines with green luminous technical imagery, compact monospace labels and fine gray structure. The pricing route keeps the same dark, economical language.

Built from [/](https://neon.com/) and [/pricing](https://neon.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 255, 255)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 0)` | Page canvas |
| surface | `rgb(24, 25, 27)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(172, 172, 172)` | Supporting text |
| border | `rgb(48, 50, 54)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(52, 213, 154)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Inter | 56px | 400 | 1.13 | -0.04em |
| display-mobile | Inter | 32px | 400 | 1.13 | -0.04em |
| heading | Inter | 28px | 400 | 1.13 | -0.04em |
| body | Inter | 16px | 400 | 1.25 | -0.02em |
| action | Inter | 15px | 400 | 1.5 | -0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 300; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 500; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 600; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2") format("woff2"); unicode-range: U+370-377, U+37A-37F, U+384-38A, U+38C, U+38E-3A1, U+3A3-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:300;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:400;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:500;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:600;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2c55a0e60120577a-s.03ez25a9g3i0n.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C8A,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/9c72aa0f40e4eef8-s.3i9rha7jpxn0q.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/ad66f9afd8947f86-s.2o7ko1d-5m1xu.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/5476f68d60460930-s.1ee5w62fj497l.woff2")format("woff2");unicode-range:U+370-377,U+37A-37F,U+384-38A,U+38C,U+38E-3A1,U+3A3-3FF}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/2bbe8d2671613f1f-s.1way2z9fj6cig.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/1bffadaabf893a1e-s.0szrwpqb9mkwe.woff2")format("woff2");unicode-range:U+100-2BA,U+2BD-2C5,U+2C7-2CC,U+2CE-2D7,U+2DD-2FF,U+304,U+308,U+329,U+1D00-1DBF,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C4,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Inter;font-style:normal;font-weight:700;font-display:swap;src:url("https://neon.com/_next/static/immutable/media/83afe278b6a6bb3c-s.p.45535valc9rzk.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2JL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa0ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2ZL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa2pL7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa25L7W0Q5n-wU.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 900;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcC73FwrK3iLTeHuS_nVMrMxCp50SjIa1ZL7W0Q5nw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Let a large atmospheric hero image frame left-aligned copy and small actions. Use numbered feature sections and occasional pale mint panels below. Pricing centers its introduction above three rule-separated plan columns; narrow views stack plans without changing the hierarchy.

Spacing scale: xs 4px, sm 8px, md 16px, lg 26px, xl 28px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 0px left and 0px right padding. The sampled header is static, 172px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `352.562px 14px` with gap `normal 6px`; `265.375px` with gap `8px normal`; `265.375px` with gap `8px normal`. Build them as a fluid grid. Sampled container maximum widths: `1152px`, `1184px`, `1182px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact pill actions, thin outline alternatives, small uppercase technical labels, precise feature bullets and quiet plan selectors. Let separators and typography establish the grid instead of strong shadows or nested cards.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 18px / 18px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The homepage uses green scan-line and light-bar imagery with technical diagrams. Use original luminous line fields and generic infrastructure diagrams, omitting product screenshots and customer or partner marks.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Technical and concise, with concrete capability and usage descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
