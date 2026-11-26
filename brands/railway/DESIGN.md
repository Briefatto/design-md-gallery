---
version: alpha
name: "Railway"
description: "Railway's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Railway."
colors:
  primary: "rgb(85, 63, 131)"
  background: "rgb(19, 17, 28)"
  surface: "rgb(19, 17, 28)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgba(255, 255, 255, 0.65)"
  border: "rgba(255, 255, 255, 0.15)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"IBM Plex Serif", Georgia, Cambria, "Times New Roman", serif, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.036em
  display-mobile:
    fontFamily: '"IBM Plex Serif", Georgia, Cambria, "Times New Roman", serif, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.049em
  heading:
    fontFamily: '"IBM Plex Serif", Georgia, Cambria, "Times New Roman", serif, ui-serif, Georgia, Cambria, "Times New Roman", Times, serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.02em
  body:
    fontFamily: 'Inter, -apple-system, "system-ui", "Segoe UI", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: -0.005em
  action:
    fontFamily: 'Inter, -apple-system, "system-ui", "Segoe UI", sans-serif, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 8px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 76px
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

# Railway DESIGN.md

## Overview

A developer cloud site combines a near-black violet canvas, editorial IBM Plex Serif headings, practical Inter interface text, and muted purple actions. Fine borders and layered dark panels keep the technical content calm.

Built from [/](https://railway.com/) and [/pricing](https://railway.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(85, 63, 131)` | Priority actions and selected emphasis |
| background | `rgb(19, 17, 28)` | Page canvas |
| surface | `rgb(19, 17, 28)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgba(255, 255, 255, 0.65)` | Supporting text |
| border | `rgba(255, 255, 255, 0.15)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "IBM Plex Serif" | 54px | 500 | 1.12 | -0.036em |
| display-mobile | "IBM Plex Serif" | 40px | 500 | 1.12 | -0.049em |
| heading | "IBM Plex Serif" | 36px | 400 | 1.33 | -0.02em |
| body | Inter | 18px | 500 | 1.6 | -0.005em |
| action | Inter | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvvYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvmYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvuYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvhYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvtYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcvsYwYZ8UA3J58.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300 800;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/inter/v20/UcCo3FwrK3iLTcviYwYZ8UA3.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizBREVNn1dOx-zrZ2X3pZvkTiUa6zgTjnTLgNuZ5w.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizBREVNn1dOx-zrZ2X3pZvkTiUa6zETjnTLgNuZ5w.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizBREVNn1dOx-zrZ2X3pZvkTiUa6zoTjnTLgNuZ5w.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizBREVNn1dOx-zrZ2X3pZvkTiUa6zsTjnTLgNuZ5w.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizBREVNn1dOx-zrZ2X3pZvkTiUa6zUTjnTLgNs.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizDREVNn1dOx-zrZ2X3pZvkTiUS2zcZiVbJsNo.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizDREVNn1dOx-zrZ2X3pZvkTiUb2zcZiVbJsNo.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizDREVNn1dOx-zrZ2X3pZvkTiUQ2zcZiVbJsNo.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizDREVNn1dOx-zrZ2X3pZvkTiUR2zcZiVbJsNo.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizDREVNn1dOx-zrZ2X3pZvkTiUf2zcZiVbJ.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3s-CI5q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3s-CIwq1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3s-CI7q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3s-CI6q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3s-CI0q1vjitOh.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3A_yI5q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3A_yIwq1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3A_yI7q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3A_yI6q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi3A_yI0q1vjitOh.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi2k_iI5q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi2k_iIwq1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi2k_iI7q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi2k_iI6q1vjitOh3oc.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'IBM Plex Serif';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/ibmplexserif/v20/jizAREVNn1dOx-zrZ2X3pZvkTi2k_iI0q1vjitOh.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Use a compact top bar and a centered hero above a large product demonstration. Follow with aligned dark feature panels and a consistent reading grid. Pricing moves to a left-aligned serif introduction, usage illustration, and structured plan panels; mobile stacks the same hierarchy.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 76px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 32px high, with 0px left and 0px right padding. The sampled header is static, 209.5px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `124px 1160px 124px` with gap `normal`; `234.656px 234.672px 234.672px 234.656px 234.672px 234.672px` with gap `0px`; `67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px 67.3281px` with gap `normal 32px`. Build them as a fluid grid. Sampled container maximum widths: `1160px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use quiet dark panels, compact actions, thin separators, and clear pricing groupings.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 58px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original illustrated night skies, restrained atmospheric color, point grids, and neutral deployment diagrams.

**Motion.** Observed CSS transition declarations include `filter 0.15s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `filter, border-color 0.2s`, `transform 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Developer-focused, concise, and practical.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
