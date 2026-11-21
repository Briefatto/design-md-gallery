---
version: alpha
name: "HeyGen"
description: "HeyGen's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with HeyGen."
colors:
  primary: "rgb(0, 195, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(250, 250, 250)"
  foreground: "rgb(23, 23, 23)"
  muted: "oklab(0.32109 0.0000146329 0.0000064075 / 0.8)"
  border: "oklab(0 0 0 / 0.1)"
  on-primary: "rgb(3, 51, 55)"
typography:
  display:
    fontFamily: '"ABC Solar Display", "TT Norms Pro", Arial, Helvetica, sans-serif'
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"ABC Solar Display", "TT Norms Pro", Arial, Helvetica, sans-serif'
    fontSize: 31px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: 0em
  heading:
    fontFamily: '"ABC Solar Display", "TT Norms Pro", Arial, Helvetica, sans-serif'
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.025em
  body:
    fontFamily: '"TT Norms Pro", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
  action:
    fontFamily: '"TT Norms Pro", Arial, Helvetica, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 12px
  card: 28px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 60px
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

# HeyGen DESIGN.md

## Overview

An avatar-video platform uses heavy rounded display type, bright cyan actions, pale neutral surfaces and playful iridescent accents. Tall media cards and bold section headings provide the main visual rhythm.

Built from [/](https://heygen.com/) and [/pricing](https://heygen.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 195, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(250, 250, 250)` | Panels and cards |
| foreground | `rgb(23, 23, 23)` | Primary text |
| muted | `oklab(0.32109 0.0000146329 0.0000064075 / 0.8)` | Supporting text |
| border | `oklab(0 0 0 / 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(3, 51, 55)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "ABC Solar Display" | 60px | 400 | 1.05 | 0em |
| display-mobile | "ABC Solar Display" | 31px | 400 | 1.05 | 0em |
| heading | "ABC Solar Display" | 32px | 700 | 1.05 | -0.025em |
| body | "TT Norms Pro" | 16px | 400 | 1.5 | -0.01em |
| action | "TT Norms Pro" | 18px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Light.latin.4f33a746.woff2") format("woff2"); font-weight: 300; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.latin.30154419.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.latin-ext.a04da199.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.cyrillic.43f5176b.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+400-52F, U+1C80-1C88, U+20B4, U+2116, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.greek.a08acc43.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+370-3FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.vietnamese.8714124e.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.symbols.4746b446.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+E000-F8FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.latin.6e7c29f5.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.latin-ext.9f204d21.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.cyrillic.4526f3bd.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+400-52F, U+1C80-1C88, U+20B4, U+2116, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.greek.50637020.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+370-3FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.vietnamese.170c3373.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.symbols.730d1c26.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+E000-F8FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.latin.d5851e25.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.latin-ext.77b55a92.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.cyrillic.fc0164e7.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+400-52F, U+1C80-1C88, U+20B4, U+2116, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.greek.0ca57702.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+370-3FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.vietnamese.64d0cb4e.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.symbols.7580ad91.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+E000-F8FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.latin.ce4f166c.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.latin-ext.091cbc56.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.cyrillic.57f98643.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+400-52F, U+1C80-1C88, U+20B4, U+2116, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.greek.43bf4a1a.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+370-3FF; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.vietnamese.de1b7330.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "TT Norms Pro"; src: url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.symbols.d41eeafb.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+E000-F8FF; }
@font-face { font-family: "ABC Solar Display"; src: url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.latin.6ff709c5.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+289, U+2BB-2BC, U+2C6-2C7, U+2D8-2DD, U+300-304, U+306-30C, U+312, U+31B, U+323, U+326-328, U+335, U+337-338, U+E3F, U+2000-2070, U+2074-2079, U+2080-2089, U+20AC, U+2117, U+2122, U+2126, U+212E, U+2150-215F, U+2190-2199, U+2202, U+2205-2206, U+220F, U+2211-2212, U+2215, U+2219-221A, U+221E, U+222B, U+2248, U+2260, U+2264-2265, U+2318, U+2329-232A, U+2460-2473, U+24EA-24F4, U+24FF, U+25CA, U+2776-277F, U+2E18, U+300A-3011, U+3014-3015, U+FB00-FB03, U+FB06, U+FEFF, U+FFFD; }
@font-face { font-family: "ABC Solar Display"; src: url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.latin-ext.b72c5676.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "ABC Solar Display"; src: url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.vietnamese.f4630ee9.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Light.latin.4f33a746.woff2")format("woff2");font-weight:300;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.latin.30154419.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.latin-ext.a04da199.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+100-24F,U+259,U+1E??,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.cyrillic.43f5176b.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+400-52F,U+1C80-1C88,U+20B4,U+2116,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.greek.a08acc43.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+370-3FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.vietnamese.8714124e.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Normal.symbols.4746b446.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+E000-F8FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.latin.6e7c29f5.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.latin-ext.9f204d21.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+100-24F,U+259,U+1E??,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.cyrillic.4526f3bd.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+400-52F,U+1C80-1C88,U+20B4,U+2116,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.greek.50637020.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+370-3FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.vietnamese.170c3373.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Medium.symbols.730d1c26.woff2")format("woff2");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+E000-F8FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.latin.d5851e25.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.latin-ext.77b55a92.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+100-24F,U+259,U+1E??,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.cyrillic.fc0164e7.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+400-52F,U+1C80-1C88,U+20B4,U+2116,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.greek.0ca57702.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+370-3FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.vietnamese.64d0cb4e.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_DemiBold.symbols.7580ad91.woff2")format("woff2");font-weight:600;font-style:normal;font-display:swap;unicode-range:U+E000-F8FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.latin.ce4f166c.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.latin-ext.091cbc56.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+100-24F,U+259,U+1E??,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.cyrillic.57f98643.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+400-52F,U+1C80-1C88,U+20B4,U+2116,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.greek.43bf4a1a.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+370-3FF}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.vietnamese.de1b7330.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:TT Norms Pro;src:url("https://www.heygen.com/fonts/tt-norms/TT_Norms_Pro_Bold.symbols.d41eeafb.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+E000-F8FF}
@font-face{font-family:ABC Solar Display;src:url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.latin.6ff709c5.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+??,U+131,U+152-153,U+289,U+2BB-2BC,U+2C6-2C7,U+2D8-2DD,U+300-304,U+306-30C,U+312,U+31B,U+323,U+326-328,U+335,U+337-338,U+E3F,U+2000-2070,U+2074-2079,U+2080-2089,U+20AC,U+2117,U+2122,U+2126,U+212E,U+215?,U+2190-2199,U+2202,U+2205-2206,U+220F,U+2211-2212,U+2215,U+2219-221A,U+221E,U+222B,U+2248,U+2260,U+2264-2265,U+2318,U+2329-232A,U+2460-2473,U+24EA-24F4,U+24FF,U+25CA,U+2776-277F,U+2E18,U+300A-3011,U+3014-3015,U+FB00-FB03,U+FB06,U+FEFF,U+FFFD}
@font-face{font-family:ABC Solar Display;src:url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.latin-ext.b72c5676.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+100-24F,U+259,U+1E??,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:ABC Solar Display;src:url("https://www.heygen.com/fonts/solar-display/ABCSolarDisplay-Bold.vietnamese.f4630ee9.woff2")format("woff2");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+1EA0-1EF9,U+20AB}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction above a wide portrait-media carousel, with compact actions and an announcement strip. Pricing uses large rounded plan cards, audience controls and billing selectors. On mobile, a plan tab selector focuses the comparison on one plan at a time.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 84px high, with 0px left and 0px right padding. The sampled nav is static, 38px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `91.7969px 745.016px 339.188px` with gap `16px`; `449.328px 898.672px` with gap `60px`; `425.328px 425.344px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `1280px`, `860px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `28px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use cyan filled actions, quiet neutral companions, rounded media cards, compact segmented selectors and subtle colorful outlines. Keep the display face distinct from practical body and comparison text.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source relies on avatar and portrait videos, dimensional decorative forms and product demonstrations. Use original licensed media and abstract forms without copying people, avatars, recordings, screenshots or source artwork.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, visibility, content-visibility, overlay, pointer-events 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, upbeat and practical, with simple creation and plan-selection labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
