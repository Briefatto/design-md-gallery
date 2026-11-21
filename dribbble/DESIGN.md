---
version: alpha
name: "Dribbble"
description: "Dribbble's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Dribbble."
colors:
  primary: "#ea4c89"
  background: "#ffffff"
  surface: "#f8f8fc"
  foreground: "#0d0c22"
  muted: "#655c7a"
  border: "#ffffff"
  on-primary: "#000000"
typography:
  display:
    fontFamily: '"Mona Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Mona Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 27px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: '"Mona Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 27px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Mona Sans", "Mona Sans Placeholder", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.21
    letterSpacing: 0em
  action:
    fontFamily: '"Mona Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0em
rounded:
  control: 12px
  card: 24px
spacing:
  xs: 8px
  sm: 8px
  md: 16px
  lg: 16px
  xl: 16px
  section: 16px
components:
  primary-button:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.control}"
---

# Dribbble DESIGN.md

## Overview

A design marketplace pairs editorial headline typography with a clean discovery interface and a colorful, image-led project grid.

Built from [/](https://dribbble.com/) and [/pro](https://dribbble.com/pro), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `#ea4c89` | Priority actions and selected emphasis |
| background | `#ffffff` | Page canvas |
| surface | `#f8f8fc` | Panels and cards |
| foreground | `#0d0c22` | Primary text |
| muted | `#655c7a` | Supporting text |
| border | `#ffffff` | Quiet separators and outlines |
| on-primary | `#000000` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Mona Sans" | 52px | 600 | 1.2 | 0em |
| display-mobile | "Mona Sans" | 27px | 600 | 1.2 | 0em |
| heading | "Mona Sans" | 27px | 600 | 1.2 | 0em |
| body | "Mona Sans" | 14px | 400 | 1.21 | 0em |
| action | "Mona Sans" | 12px | 500 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-family: "Mona Sans"; font-style: italic; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0kIpQmx24alC5A4PNr4C5OaxRsfNNlKbCePevHtVtX57DGjDU1QOkZ2V_SyFtY.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: italic; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0kIpQmx24alC5A4PNr4C5OaxRsfNNlKbCePevHtVtX57DGjDU1QOkZ2V7SyFtY.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: italic; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0kIpQmx24alC5A4PNr4C5OaxRsfNNlKbCePevHtVtX57DGjDU1QOkZ2VDSyA.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 400; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aHdu2ui.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 400; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aDdu2ui.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 400; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5a7duw.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 500; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aHdu2ui.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 500; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aDdu2ui.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 500; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5a7duw.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aHdu2ui.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aDdu2ui.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 600; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5a7duw.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 700; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aHdu2ui.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 700; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aDdu2ui.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 700; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5a7duw.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 800; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aHdu2ui.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 800; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5aDdu2ui.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 800; font-stretch: 100%; font-display: swap; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0bIpQmx24alC5A4PNB6Ryti20_6n1iPHjc5a7duw.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 200; font-stretch: 100%; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0mIpQmx24alC5A4PNB6Ryti20_6n1iPHjcz6L1SoM-jCpoiyB9A-9V6VLKzA.woff2") format("woff2"); unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+300-301, U+303-304, U+308-309, U+323, U+329, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 200; font-stretch: 100%; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0mIpQmx24alC5A4PNB6Ryti20_6n1iPHjcz6L1SoM-jCpoiyB9A-9U6VLKzA.woff2") format("woff2"); unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: "Mona Sans"; font-style: normal; font-weight: 200; font-stretch: 100%; src: url("https://fonts.gstatic.com/s/monasans/v4/o-0mIpQmx24alC5A4PNB6Ryti20_6n1iPHjcz6L1SoM-jCpoiyB9A-9a6VI.woff2") format("woff2"); unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
```

The full fallback stacks are in the front matter.

## Layout

Separate the roomy introduction and search area from the denser gallery. Give navigation and category controls a clear horizontal rhythm.

Spacing scale: xs 8px, sm 8px, md 16px, lg 16px, xl 16px, section 16px. Use smaller steps within a control and larger steps between content groups.



At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `24px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use rounded search controls, quiet category filters, compact actions, and large project thumbnails with modest metadata.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Original project artwork carries the color; use simple interface icons around it.

**Motion.** Observed CSS transition declarations include `background-color, color, border-color 0.4s, 0.4s, 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Creative, welcoming, and direct; discovery labels should remain short.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

