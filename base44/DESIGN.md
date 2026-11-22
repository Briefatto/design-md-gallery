---
version: alpha
name: "Base44"
description: "Base44's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Base44."
colors:
  primary: "rgb(49, 47, 47)"
  background: "rgb(249, 248, 246)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(30, 30, 36)"
  muted: "rgb(109, 106, 103)"
  border: "rgb(238, 236, 235)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(255, 106, 0)"
typography:
  display:
    fontFamily: 'Dazzed, "Dazzed Fallback", sans-serif'
    fontSize: 93.744px
    fontWeight: 600
    lineHeight: 1.05
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'Dazzed, "Dazzed Fallback", sans-serif'
    fontSize: 49.842px
    fontWeight: 600
    lineHeight: 1.09
    letterSpacing: -0.02em
  heading:
    fontFamily: 'Dazzed, "Dazzed Fallback", sans-serif'
    fontSize: 39px
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: -0.02em
  body:
    fontFamily: 'Geist, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.01em
  action:
    fontFamily: 'Dazzed, "Dazzed Fallback", sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 8px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 63.7502px
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

# Base44 DESIGN.md

## Overview

A warm, lightly textured creation platform pairs oversized Dazzed type with a central prompt composer, compact utility controls, and a collage of app examples. Dark charcoal actions anchor the pale canvas; orange and electric blue punctuate selected states and large campaign sections.

Built from [/](https://base44.com/) and [/pricing](https://base44.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(49, 47, 47)` | Priority actions and selected emphasis |
| background | `rgb(249, 248, 246)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(30, 30, 36)` | Primary text |
| muted | `rgb(109, 106, 103)` | Supporting text |
| border | `rgb(238, 236, 235)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(255, 106, 0)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Dazzed | 93.744px | 600 | 1.05 | -0.04em |
| display-mobile | Dazzed | 49.842px | 600 | 1.09 | -0.02em |
| heading | Dazzed | 39px | 600 | 1.08 | -0.02em |
| body | Geist | 18px | 400 | 1.25 | -0.01em |
| action | Dazzed | 16px | 500 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Dazzed; src: url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-regular.woff2") format("woff2"), url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-regular.woff") format("woff"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: Dazzed; src: url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-medium.woff2") format("woff2"), url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-medium.woff") format("woff"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: Dazzed; src: url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-semibold.woff2") format("woff2"), url("https://media.base44.com/files/public/marketing-site-assets/fonts/dazzed/dazzed-semibold.woff") format("woff"); font-weight: 600; font-style: normal; font-display: swap; }
@font-face { font-family: Dazzed; src: url("https://base44.com/fonts/geist/geist-latin-wght-normal.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+24; }
@font-face { font-family: Dazzed; src: url("https://base44.com/fonts/geist/geist-latin-wght-normal.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+24; }
@font-face { font-family: Dazzed; src: url("https://base44.com/fonts/geist/geist-latin-wght-normal.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: swap; unicode-range: U+24; }
@font-face { font-family: Geist; src: url("https://base44.com/fonts/geist/geist-latin-wght-normal.woff2") format("woff2"); font-weight: 100 900; font-style: normal; font-display: swap; }
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwRGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwYGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwTGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwSGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 300;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwcGFWNOITd.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwRGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwYGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwTGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwSGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwcGFWNOITd.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwRGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwYGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwTGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwSGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwcGFWNOITd.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwRGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwYGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwTGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwSGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwcGFWNOITd.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwRGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwYGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwTGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwSGFWNOITddY4.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Geist';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/geist/v5/gyByhwUxId8gMEwcGFWNOITd.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Center the hero headline and prompt composer below a slim navigation. Use generous section gaps, asymmetric app-preview collages, split feature explanations, and multi-column pricing cards that stack on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 63.7502px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 86px high, with 0px left and 0px right padding. The sampled nav is static, 24px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `466px 466px 466px` with gap `21px`; `712.469px` with gap `normal`; `420px 420.016px 420px` with gap `20px`. Build them as a fluid grid. Sampled container maximum widths: `484.56px`, `726.768px`, `419.94px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use white prompt panels with a compact action row, low-radius charcoal buttons, pale category chips, and white pricing cards with thin rules, explicit prices, and concise feature lists. The billing toggle uses a warm orange active segment.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 38px, horizontal padding 15px / 15px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original abstract app mockups and geometric thumbnails arranged as a lively collage. A very fine neutral grain may soften large pale fields. Use small utilitarian line icons; do not copy the brand mark, app examples, or photographs.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, text-decoration-color, fill, stroke 0.3s`, `transform 1.1s`, `background-color, color 0.2s, 0.2s`, `background-color 0.16s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Encouraging, accessible, and action-oriented.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
