---
version: alpha
name: "Semrush"
description: "Semrush's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Semrush."
colors:
  primary: "rgb(193, 144, 255)"
  background: "oklab(0.934924 -0.0193309 -0.00164258)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(24, 30, 21)"
  muted: "rgb(108, 110, 121)"
  border: "rgb(243, 246, 246)"
  on-primary: "rgb(24, 30, 21)"
typography:
  display:
    fontFamily: 'Lazzer, sans-serif'
    fontSize: 84px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'Lazzer, sans-serif'
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  heading:
    fontFamily: 'Lazzer, sans-serif'
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  body:
    fontFamily: 'Lazzer, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.02em
  action:
    fontFamily: 'Lazzer, sans-serif'
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
rounded:
  control: 100px
  card: 0px
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

# Semrush DESIGN.md

## Overview

The captured analytics site uses bold Lazzer typography, a pale mint atmosphere, lavender feature blocks, and dark green-black text. Rounded actions and large type make the opening approachable, while product modules and pricing retain a practical information hierarchy.

Built from [/](https://www.semrush.com/) and [/pricing/](https://www.semrush.com/pricing/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(193, 144, 255)` | Priority actions and selected emphasis |
| background | `oklab(0.934924 -0.0193309 -0.00164258)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(24, 30, 21)` | Primary text |
| muted | `rgb(108, 110, 121)` | Supporting text |
| border | `rgb(243, 246, 246)` | Quiet separators and outlines |
| on-primary | `rgb(24, 30, 21)` | Text on the primary action |



Use mint as a quiet page atmosphere, lavender as an energetic action or feature-field accent, and green-black for text and alternate pricing actions. The small sample follows the lavender hero-action context. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Lazzer | 84px | 600 | 1.1 | -0.04em |
| display-mobile | Lazzer | 52px | 600 | 1.1 | -0.04em |
| heading | Lazzer | 32px | 600 | 1.1 | -0.04em |
| body | Lazzer | 16px | 500 | 1.5 | -0.02em |
| action | Lazzer | 14px | 600 | 1.2 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Lazzer; font-weight: 100; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/thin.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 100; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/thin_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 300; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/light.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 300; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/light_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 400; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/regular.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 400; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/regular_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 500; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/medium.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 500; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/medium_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 600; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/semibold.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 600; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/semibold_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 700; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/bold.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 700; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/bold_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 900; font-style: normal; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/heavy.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face { font-family: Lazzer; font-weight: 900; font-style: italic; font-display: swap; src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/heavy_italic.woff2") format("woff2"); unicode-range: U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA, U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6, U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328, U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0, U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2, U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E, U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070, U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4, U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126, U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202, U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248, U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF, U+2776-277E, U+E132, U+E133, U+FB01, U+FB02; }
@font-face {
  font-family: Lazzer;
  font-weight: 100;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/thin.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 100;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/thin_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 300;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/light.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 300;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/light_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 400;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/regular.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 400;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/regular_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 500;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/medium.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 500;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/medium_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 600;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/semibold.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 600;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/semibold_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 700;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/bold.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 700;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/bold_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 900;
  font-style: normal;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/heavy.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
@font-face {
  font-family: Lazzer;
  font-weight: 900;
  font-style: italic;
  font-display: swap;
  src: url("https://www.semrush.com/__static__/fonts/lazzer/v2/heavy_italic.woff2") format('woff2');
  unicode-range:
    U+D, U+20-7E, U+A0-148, U+14A-17F, U+18F, U+192, U+19D, U+1E6, U+1E7, U+1EA,
    U+1EB, U+1FA-1FF, U+218-21B, U+232, U+233, U+237, U+259, U+272, U+2C6,
    U+2C7, U+2D8-2DD, U+300-304, U+306-308, U+30A-30C, U+312, U+323, U+326-328,
    U+335-338, U+3A9, U+3C0, U+E3F, U+1E20, U+1E21, U+1E80-1E85, U+1E9E, U+1EA0,
    U+1EA1, U+1EB8, U+1EB9, U+1EBC, U+1EBD, U+1ECA-1ECD, U+1EE4, U+1EE5, U+1EF2,
    U+1EF3, U+1EF8, U+1EF9, U+2009, U+2013, U+2014, U+2018-201A, U+201C-201E,
    U+2020-2022, U+2026, U+2030, U+2032, U+2033, U+2039, U+203A, U+2044, U+2070,
    U+2074-2079, U+2080-2089, U+20A3, U+20A6, U+20A9-20AC, U+20B1, U+20B4,
    U+20B9, U+20BA, U+20BD, U+20BF, U+2113, U+2116, U+2117, U+2122, U+2126,
    U+212E, U+2153, U+2154, U+215B-215E, U+2190-2193, U+2196-2199, U+2202,
    U+2205, U+2206, U+220F, U+2211, U+2212, U+221A, U+221E, U+222B, U+2248,
    U+2260, U+2264, U+2265, U+2460-2468, U+24EA, U+24FF, U+25CA, U+25CB, U+25CF,
    U+2776-277E, U+E132, U+E133, U+FB01, U+FB02;
}
```

The full fallback stacks are in the front matter.

## Layout

Use a narrow lavender announcement band and a pale navigation, then an oversized centered headline above a rounded URL-entry composer. Follow with broad product modules, white data panels, and alternating dark chapters. Pricing starts with a compact introduction and selectors above aligned white tier cards that stack on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 84px high, with 24px left and 24px right padding. The sampled header is sticky, 84px high, with 24px left and 24px right padding.

Measured desktop grid tracks: `93px 93px 93px 93px 93px 93px 93px 93px 93px 93px 93px 93px` with gap `normal 12px`; `93px 93px 93px 93px 93px 93px 93px 93px 93px 93px 93px 93px` with gap `normal 12px`; `971.109px 404.891px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `1145px`, `600px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `100px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use pill actions, a white rounded URL field with a compact region selector, small tab groups, softly rounded white comparison cards, and restrained feature lists. The hero action uses lavender with dark text; pricing priority actions use dark fill with white text. Keep those contexts distinct.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 60px, horizontal padding 32px / 32px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 58px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(24, 30, 21). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original analytics charts, generic metric tiles, abstract visibility diagrams, and fine diagonal stripe accents. Dark sections can use luminous vertical geometry.

**Motion.** Observed CSS transition declarations include `background-color, border-color, color 0.2s`, `width 0.4s`, `width, min-width, max-width 0.1s, 0.1s, 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, practical, and explicit about useful outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
