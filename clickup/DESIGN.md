---
version: alpha
name: "ClickUp"
description: "ClickUp's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with ClickUp."
colors:
  primary: "rgb(32, 32, 32)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(248, 249, 250)"
  foreground: "rgb(32, 32, 32)"
  muted: "rgb(100, 100, 100)"
  border: "rgb(212, 212, 212)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Plus Jakarta Sans"'
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  display-mobile:
    fontFamily: '"Plus Jakarta Sans"'
    fontSize: 34px
    fontWeight: 650
    lineHeight: 1.18
    letterSpacing: -0.047em
  heading:
    fontFamily: '"Plus Jakarta Sans", -apple-system, Roboto, Helvetica, sans-serif'
    fontSize: 48px
    fontWeight: 650
    lineHeight: 1.25
    letterSpacing: -0.035em
  body:
    fontFamily: 'Inter'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.011em
  action:
    fontFamily: 'Inter, sans-serif'
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 8px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 28px
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

# ClickUp DESIGN.md

## Overview

A bright productivity canvas pairs heavy Plus Jakarta Sans statements with compact Inter controls, neutral surfaces and vivid gradient accents in selected feature regions.

Built from [/](https://clickup.com/) and [/pricing](https://clickup.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(32, 32, 32)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(248, 249, 250)` | Panels and cards |
| foreground | `rgb(32, 32, 32)` | Primary text |
| muted | `rgb(100, 100, 100)` | Supporting text |
| border | `rgb(212, 212, 212)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Plus Jakarta Sans" | 60px | 700 | 1.1 | -0.035em |
| display-mobile | "Plus Jakarta Sans" | 34px | 650 | 1.18 | -0.047em |
| heading | "Plus Jakarta Sans" | 48px | 650 | 1.25 | -0.035em |
| body | Inter | 14px | 500 | 1.43 | -0.011em |
| action | Inter | 14px | 600 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-weight: 100 900; font-style: normal; font-family: Inter; src: url("https://clickup.com/assets/fonts/Inter.woff2") format("woff2"), url("https://clickup.com/assets/fonts/Inter.woff") format("woff"), url("https://clickup.com/assets/fonts/Inter.ttf") format("truetype"); font-display: swap; }
@font-face { font-weight: 100 900; font-style: italic; font-family: Inter; src: url("https://clickup.com/assets/fonts/Inter-Italic.woff2") format("woff2"), url("https://clickup.com/assets/fonts/Inter-Italic.woff") format("woff"), url("https://clickup.com/assets/fonts/Inter-Italic.ttf") format("truetype"); font-display: swap; }
@font-face { font-weight: 200 800; font-style: normal; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.woff2") format("woff2"), url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.woff") format("woff"), url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.ttf") format("truetype"); font-display: swap; }
@font-face { font-weight: 200 800; font-style: italic; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.woff2") format("woff2"), url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.woff") format("woff"), url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.ttf") format("truetype"); font-display: swap; }
@font-face { font-weight: 100 900; font-style: normal; font-family: Inter; src: url("https://clickup.com/assets/fonts/subset/Inter.latin.woff2") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-weight: 100 900; font-style: normal; font-family: Inter; src: url("https://clickup.com/assets/fonts/subset/Inter.latin-ext.woff2") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-weight: 100 900; font-style: italic; font-family: Inter; src: url("https://clickup.com/assets/fonts/subset/Inter-Italic.latin.woff2") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-weight: 100 900; font-style: italic; font-family: Inter; src: url("https://clickup.com/assets/fonts/subset/Inter-Italic.latin-ext.woff2") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-weight: 200 800; font-style: normal; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/subset/PlusJakartaSans.latin.woff2") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-weight: 200 800; font-style: normal; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/subset/PlusJakartaSans.latin-ext.woff2") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-weight: 200 800; font-style: italic; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/subset/PlusJakartaSans-Italic.latin.woff2") format("woff2"); font-display: swap; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+304, U+308, U+329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-weight: 200 800; font-style: italic; font-family: "Plus Jakarta Sans"; src: url("https://clickup.com/assets/fonts/subset/PlusJakartaSans-Italic.latin-ext.woff2") format("woff2"); font-display: swap; unicode-range: U+100-2BA, U+2BD-2C5, U+2C7-2CC, U+2CE-2D7, U+2DD-2FF, U+304, U+308, U+329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face{font-weight:100 900;font-style:normal;font-family:Inter;src:url("https://clickup.com/assets/fonts/Inter.woff2") format("woff2"),url("https://clickup.com/assets/fonts/Inter.woff") format("woff"),url("https://clickup.com/assets/fonts/Inter.ttf") format("truetype");font-display:swap}
@font-face{font-weight:100 900;font-style:italic;font-family:Inter;src:url("https://clickup.com/assets/fonts/Inter-Italic.woff2") format("woff2"),url("https://clickup.com/assets/fonts/Inter-Italic.woff") format("woff"),url("https://clickup.com/assets/fonts/Inter-Italic.ttf") format("truetype");font-display:swap}
@font-face{font-weight:200 800;font-style:normal;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.woff2") format("woff2"),url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.woff") format("woff"),url("https://clickup.com/assets/fonts/PlusJakartaSans-VariableFont_wght.ttf") format("truetype");font-display:swap}
@font-face{font-weight:200 800;font-style:italic;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.woff2") format("woff2"),url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.woff") format("woff"),url("https://clickup.com/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.ttf") format("truetype");font-display:swap}
@font-face{font-weight:100 900;font-style:normal;font-family:Inter;src:url("https://clickup.com/assets/fonts/subset/Inter.latin.woff2") format("woff2");font-display:swap;unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+2074,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-weight:100 900;font-style:normal;font-family:Inter;src:url("https://clickup.com/assets/fonts/subset/Inter.latin-ext.woff2") format("woff2");font-display:swap;unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-weight:100 900;font-style:italic;font-family:Inter;src:url("https://clickup.com/assets/fonts/subset/Inter-Italic.latin.woff2") format("woff2");font-display:swap;unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+2074,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-weight:100 900;font-style:italic;font-family:Inter;src:url("https://clickup.com/assets/fonts/subset/Inter-Italic.latin-ext.woff2") format("woff2");font-display:swap;unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-weight:200 800;font-style:normal;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/subset/PlusJakartaSans.latin.woff2") format("woff2");font-display:swap;unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+2074,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-weight:200 800;font-style:normal;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/subset/PlusJakartaSans.latin-ext.woff2") format("woff2");font-display:swap;unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-weight:200 800;font-style:italic;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/subset/PlusJakartaSans-Italic.latin.woff2") format("woff2");font-display:swap;unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+2074,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-weight:200 800;font-style:italic;font-family:Plus Jakarta Sans;src:url("https://clickup.com/assets/fonts/subset/PlusJakartaSans-Italic.latin-ext.woff2") format("woff2");font-display:swap;unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
```

The full fallback stacks are in the front matter.

## Layout

Use a narrow navigation, left-aligned homepage hero and broad demonstration panel, then alternate dark feature sections and white explanatory blocks. Pricing centers the headline above aligned plan cards; the mobile capture retains horizontally arranged cards with the next card partially visible.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 28px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 308px high, with 0px left and 0px right padding. The sampled header is static, 224.406px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `358.656px 358.672px 358.656px` with gap `1px`; `138.125px 138.125px 138.125px 138.125px 138.125px 138.125px 138.125px 138.125px 138.125px 138.125px` with gap `normal`; `358.656px 358.672px 358.656px` with gap `1px`. Build them as a fluid grid. Sampled container maximum widths: `820px`, `720px`, `760px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Dark rounded actions, pale gray secondary controls, pill billing selectors and thin card borders keep dense content organized. A black featured plan reverses the text and action colors; small multicolor icons distinguish product capabilities.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 12px / 12px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 4px, radius 12px, background rgba(0, 0, 0, 0), and border 0px rgb(16, 16, 16). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Product interface demonstrations, an icon grid, vivid AI gradient fields and selected customer portraits provide variety. Keep the main reading canvas quiet.

**Motion.** Observed CSS transition declarations include `background-color 0.2s`, `all 0.3s`, `all 0.25s`, `background-color, color 0.2s, 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Energetic and compact, emphasizing connected work and practical productivity.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
