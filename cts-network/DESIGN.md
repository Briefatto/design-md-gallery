---
version: alpha
name: "CTS Network"
description: "CTS Network's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with CTS Network."
colors:
  primary: "rgb(237, 167, 32)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(240, 239, 248)"
  foreground: "rgb(44, 43, 81)"
  muted: "rgb(136, 136, 136)"
  border: "rgb(221, 221, 221)"
  on-primary: "rgb(44, 43, 81)"
typography:
  display:
    fontFamily: 'Figtree, sans-serif'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Figtree, sans-serif'
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: 0em
  heading:
    fontFamily: 'Figtree, sans-serif'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: 0em
  body:
    fontFamily: 'system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: 0em
  action:
    fontFamily: 'system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 15.2px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 8px
  card: 6px
spacing:
  xs: 5px
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

# CTS Network DESIGN.md

## Overview

An engineering knowledge platform pairs a deep navy-and-gold introduction with clean white editorial surfaces. Bold Figtree headings, fine technical grid lines, compact navigation, and restrained rounded blocks give it a practical institutional character.

Built from [/](https://ctsnetwork.id/) and [/about](https://ctsnetwork.id/about), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(237, 167, 32)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(240, 239, 248)` | Panels and cards |
| foreground | `rgb(44, 43, 81)` | Primary text |
| muted | `rgb(136, 136, 136)` | Supporting text |
| border | `rgb(221, 221, 221)` | Quiet separators and outlines |
| on-primary | `rgb(44, 43, 81)` | Text on the primary action |

Use navy for reading text and major identity fields, gold for priority actions and selective emphasis, and white for long-form reading. The hero inverts to light text over navy; preserve that pairing as a separate context. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Figtree | 48px | 700 | 1.15 | 0em |
| display-mobile | Figtree | 28px | 700 | 1.15 | 0em |
| heading | Figtree | 48px | 700 | 1.15 | 0em |
| body | system-ui | 18px | 400 | 1.7 | 0em |
| action | system-ui | 15.2px | 600 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4q9DaRvziissg.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4S9DaRvzig.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4q9DaRvziissg.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4S9DaRvzig.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4q9DaRvziissg.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 600;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4S9DaRvzig.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4q9DaRvziissg.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Figtree';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/figtree/v9/_Xms-HUzqDCFdgfMm4S9DaRvzig.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Use a broad desktop header with navigation and search, a split navy hero with a fine grid, and aligned editorial sections. Mobile centers and stacks the hero content. About uses a centered introduction, a three-part metric band, and repeated informational panels.

Spacing scale: xs 5px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 107px high, with 0px left and 0px right padding. The sampled nav is relative, 83px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `421.5px 421.5px` with gap `20px`; `421.5px 421.5px` with gap `20px`; `379.141px 252.766px 252.766px 303.328px` with gap `36px`. Build them as a fluid grid. Sampled container maximum widths: `520px`, `1320px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `6px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rounded actions, a filled gold priority button, an outlined companion, small category labels, and quiet bordered information panels. Keep the navigation hierarchy and search easy to scan.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 54.7969px, horizontal padding 32px / 32px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 22.3906px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(26, 26, 46). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original engineering diagrams, technical geometry, and licensed construction photography.

**Motion.** Observed CSS transition declarations include `color, background-color 0.25s, 0.25s`, `transform, box-shadow, background-color 0.2s, 0.2s, 0.2s`, `border-color, background-color, color 0.2s, 0.2s, 0.2s`, `opacity, transform 0.5s, 0.5s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Informative, community-oriented, and technically literate. Use short navigation labels and clear descriptions of what a reader can find or do.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't turn the measured navy-and-gold hierarchy into an unrelated neon or heavily illustrated consumer interface.

