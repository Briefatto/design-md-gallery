---
version: alpha
name: "NASA"
description: "NASA's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with NASA."
colors:
  primary: "rgb(216, 57, 51)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(27, 27, 27)"
  muted: "rgb(113, 113, 115)"
  border: "rgb(239, 239, 239)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(11, 61, 145)"
typography:
  display:
    fontFamily: 'inter, sans-serif'
    fontSize: 29.008px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'inter, sans-serif'
    fontSize: 35.2px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: 0em
  heading:
    fontFamily: 'inter, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'inter'
    fontSize: 14.4px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  action:
    fontFamily: 'inter, sans-serif'
    fontSize: 17.6px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 59.76px
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

# NASA DESIGN.md

## Overview

A science institution combines bold Inter editorial headings, black navigation and media chapters, white reading sections, and red actions. Blue is an institutional announcement accent, while tiny tracked technical labels separate story categories and metadata.

Built from [/](https://www.nasa.gov/) and [/missions/](https://www.nasa.gov/missions/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(216, 57, 51)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(27, 27, 27)` | Primary text |
| muted | `rgb(113, 113, 115)` | Supporting text |
| border | `rgb(239, 239, 239)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(11, 61, 145)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | inter | 29.008px | 700 | 1.05 | 0em |
| display-mobile | inter | 35.2px | 700 | 1.05 | 0em |
| heading | inter | 40px | 700 | 1 | 0em |
| body | inter | 14.4px | 400 | 1.2 | 0em |
| action | inter | 17.6px | 600 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2JL7SUc.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa0ZL7SUc.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2ZL7SUc.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1pL7SUc.woff2") format("woff2"); unicode-range: U+370-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2pL7SUc.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa25L7SUc.woff2") format("woff2"); unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 200; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1ZL7.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZJhiI2B.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZthiI2B.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZNhiI2B.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZxhiI2B.woff2") format("woff2"); unicode-range: U+370-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZBhiI2B.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZFhiI2B.woff2") format("woff2"); unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZ9hiA.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2JL7SUc.woff2") format("woff2"); unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa0ZL7SUc.woff2") format("woff2"); unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2ZL7SUc.woff2") format("woff2"); unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1pL7SUc.woff2") format("woff2"); unicode-range: U+370-3FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2pL7SUc.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa25L7SUc.woff2") format("woff2"); unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1ZL7.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2JL7SUc.woff2") format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa0ZL7SUc.woff2") format("woff2");unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2ZL7SUc.woff2") format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1pL7SUc.woff2") format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2pL7SUc.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa25L7SUc.woff2") format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:200;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1ZL7.woff2") format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZJhiI2B.woff2") format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZthiI2B.woff2") format("woff2");unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZNhiI2B.woff2") format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZxhiI2B.woff2") format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZBhiI2B.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZFhiI2B.woff2") format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:400;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcCO3FwrK3iLTeHuS_fvQtMwCp50KnMw2boKoduKmMEVuLyfAZ9hiA.woff2") format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2JL7SUc.woff2") format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa0ZL7SUc.woff2") format("woff2");unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2ZL7SUc.woff2") format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1pL7SUc.woff2") format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa2pL7SUc.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa25L7SUc.woff2") format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:"Inter";font-style:normal;font-weight:700;font-display:swap;src:url("https://www.nasa.gov/wp-content/client-mu-plugins/uswds-framework/uswds/fonts-split/inter/UcC73FwrK3iLTeHuS_fvQtMwCp50KnMa1ZL7.woff2") format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
```

The full fallback stacks are in the front matter.

## Layout

Use a full-width black header with a centered identity position, search, and broad topic navigation. A large documentary hero carries a strong left-aligned title, an action, and a row of related links. News uses image-led editorial grids; mission browsing pairs a filter rail with a multi-column results grid that becomes a mobile filter control and stacked results.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 59.76px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 86.2812px high, with 16px left and 16px right padding. The sampled nav is relative, 50.625px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `640px`, `412.85px`, `1360px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use square red actions, compact circular arrow signals, bold text links, unframed editorial cards, clear search fields, and conventional labeled checkboxes. Preserve strong typographic hierarchy and wide gutters instead of nesting content in rounded panels.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 46.0781px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 32px, radius 0px, background rgb(0, 0, 0), and border 1px rgb(86, 92, 101). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use properly licensed original science photography or neutral educational diagrams, with large crops and dark overlays where text crosses imagery. Use small functional arrows and search/filter symbols. This collection redistributes no site images, program marks, or insignia.

**Motion.** Observed CSS transition declarations include `all 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Informative, factual, and accessible; keep labels clear and concrete.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

