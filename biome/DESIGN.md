---
version: alpha
name: "Biome"
description: "Biome's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Biome."
colors:
  primary: "rgb(0, 101, 218)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(245, 246, 248)"
  foreground: "rgb(23, 24, 28)"
  muted: "rgb(93, 99, 118)"
  border: "rgba(120, 139, 148, 0.2)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(96, 165, 250)"
typography:
  display:
    fontFamily: 'Geist-b17c5c92c1d3a205, "Geist-b17c5c92c1d3a205 fallback: Arial", "Geist-b17c5c92c1d3a205 fallback: Arial Bold", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Geist-b17c5c92c1d3a205, "Geist-b17c5c92c1d3a205 fallback: Arial", "Geist-b17c5c92c1d3a205 fallback: Arial Bold", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 29px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: 'Geist-b17c5c92c1d3a205, "Geist-b17c5c92c1d3a205 fallback: Arial", "Geist-b17c5c92c1d3a205 fallback: Arial Bold", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: 'Geist-b17c5c92c1d3a205, "Geist-b17c5c92c1d3a205 fallback: Arial", "Geist-b17c5c92c1d3a205 fallback: Arial Bold", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
    letterSpacing: 0em
  action:
    fontFamily: 'Geist-b17c5c92c1d3a205, "Geist-b17c5c92c1d3a205 fallback: Arial", "Geist-b17c5c92c1d3a205 fallback: Arial Bold", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.75
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 1px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 40px
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

# Biome DESIGN.md

## Overview

A developer toolchain site combines bold Geist headings, a pale blue atmospheric hero and practical, high-contrast documentation. Bright blue actions and links organize a mostly white interface with neutral code surfaces.

Built from [/](https://biomejs.dev/) and [/guides/getting-started/](https://biomejs.dev/guides/getting-started/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 101, 218)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(245, 246, 248)` | Panels and cards |
| foreground | `rgb(23, 24, 28)` | Primary text |
| muted | `rgb(93, 99, 118)` | Supporting text |
| border | `rgba(120, 139, 148, 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(96, 165, 250)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Geist-b17c5c92c1d3a205 | 64px | 600 | 1.2 | 0em |
| display-mobile | Geist-b17c5c92c1d3a205 | 29px | 600 | 1.2 | 0em |
| heading | Geist-b17c5c92c1d3a205 | 20px | 600 | 1.2 | 0em |
| body | Geist-b17c5c92c1d3a205 | 16px | 400 | 1.75 | 0em |
| action | Geist-b17c5c92c1d3a205 | 12px | 400 | 1.75 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/7f97bb65dd9f1634.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 400; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/8fd29b159fde333c.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 500; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/4d8fe12540ba86a7.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 600; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/c180d128d32fa5e3.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 700; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/239b7e40d3f6618f.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 400; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/3f543f3ed3505597.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 500; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/bf5a498a9e97e1a0.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 600; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/044f2de48dff0043.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; font-weight: 700; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/7da97a36b5aa3bc9.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 400; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/ddb059ff33462a1e.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 500; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/59ad670b898671c0.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 600; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/1aed7c347e31ffc8.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 700; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/672027e32d868276.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 400; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/37e026139db216ab.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 500; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/2be3cd24992547c2.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 600; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/957ae6fded79b1cb.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; font-weight: 700; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/449c90b56963a9f9.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 400; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/b105d30a39969418.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 500; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/9c2930200334a3f5.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 600; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/b573acfc293e6c75.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 700; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/126eb60e12f76787.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 400; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/e394ab832505a1ba.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 500; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/2a4df90d9a50348f.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 600; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/8ae7881c607dbb39.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; font-weight: 700; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/0cce95e00f2df873.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 400; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/9771e811a1a4dc0e.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 500; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/a63f3b7520c25837.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 600; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/2c3bd3a2052cca5f.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 700; font-style: normal; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/2ff1d20ee85ba9f7.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 400; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/f1724003580a093e.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 500; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/20fb6ffcff6b38f5.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 600; font-style: italic; }
@font-face { font-family: Geist-b17c5c92c1d3a205; src: url("https://biomejs.dev/_astro/fonts/d6f37a7f14ce0b26.woff2?dpl=6affe1e3b8b6702dfb33c293") format("woff2"); font-display: swap; unicode-range: U+460-52F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; font-weight: 700; font-style: italic; }
```

The full fallback stacks are in the front matter.

## Layout

Place the desktop hero copy beside a large brand visual, with a prominent demonstration and installation controls below. Documentation adds a left category rail and a clear reading column with numbered steps; mobile collapses navigation and stacks code panels.

Spacing scale: xs 1px, sm 8px, md 16px, lg 24px, xl 32px, section 40px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 64px high, with 24px left and 24px right padding. The sampled header is fixed, 64px high, with 24px left and 24px right padding.

Measured desktop grid tracks: `38.7969px` with gap `normal`; `528px 528px` with gap `24px`; `528px 528px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `2185.6px`, `1080px`, `720px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small rounded blue actions, outlined companions, segmented package-manager tabs, bordered terminal panels, numbered step markers and pale blue information callouts. Keep body text, code and navigation roles visibly distinct.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 56px, horizontal padding 20px / 20px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses a mascot, explanatory video and technical examples. Use original code demonstrations and simple toolchain diagrams without copying the mascot, logos or source screenshots.

**Motion.** Observed CSS transition declarations include `opacity 0.2s`, `opacity, background, border-color 0.2s`, `background-color, color 0.12s, 0.12s`, `background-color, color 0.15s, 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, practical and technical, with clear installation steps and concise feature explanations.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
