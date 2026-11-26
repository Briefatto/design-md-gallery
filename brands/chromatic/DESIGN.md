---
version: alpha
name: "Chromatic"
description: "Chromatic's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Chromatic."
colors:
  primary: "rgb(0, 115, 255)"
  background: "rgb(20, 28, 36)"
  surface: "oklch(0.221252318656 0.019053898353 252.055477410204 / 0.8)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(178, 190, 205)"
  border: "rgba(255, 255, 255, 0.1)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(232, 90, 80)"
typography:
  display:
    fontFamily: '"Nunito Sans", "Nunito Sans Fallback", "Nunito Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Nunito Sans", "Nunito Sans Fallback", "Nunito Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.27
    letterSpacing: 0em
  heading:
    fontFamily: '"Nunito Sans", "Nunito Sans Fallback", "Nunito Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: 0em
  body:
    fontFamily: '"Nunito Sans", "Nunito Sans Fallback", "Nunito Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
    letterSpacing: 0em
  action:
    fontFamily: '"Nunito Sans", "Nunito Sans Fallback", "Nunito Sans", "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 4px
  card: 8px
spacing:
  xs: 6px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 32px
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

# Chromatic DESIGN.md

## Overview

A frontend testing platform uses dark blue-gray surfaces, friendly rounded sans-serif typography, bright blue actions and selective multicolor workflow graphics. Pale content bands and detailed interface examples break up the dark presentation.

Built from [/](https://chromatic.com/) and [/pricing](https://chromatic.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 115, 255)` | Priority actions and selected emphasis |
| background | `rgb(20, 28, 36)` | Page canvas |
| surface | `oklch(0.221252318656 0.019053898353 252.055477410204 / 0.8)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(178, 190, 205)` | Supporting text |
| border | `rgba(255, 255, 255, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(232, 90, 80)` | Selective emphasis in headings, graphics, and small signals |

The source uses CSS Color Level 4 functional declarations that this Google linter version cannot parse. Equivalent OKLCH notation preserves the color gamut and opacity; tokens.json retains each original computed declaration and conversion provenance.

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Nunito Sans" | 48px | 600 | 1.33 | 0em |
| display-mobile | "Nunito Sans" | 30px | 600 | 1.27 | 0em |
| heading | "Nunito Sans" | 48px | 600 | 1.33 | 0em |
| body | "Nunito Sans" | 16px | 400 | 1.75 | 0em |
| action | "Nunito Sans" | 14px | 700 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:400;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/aa1b27f9e325731f-s.woff2") format("woff2");unicode-range:U+0460-052f,U+1c80-1c8a,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:400;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/c126d80dc21dff90-s.woff2") format("woff2");unicode-range:U+0301,U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:400;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/e850464f9dfbb75b-s.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:400;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/357067f10075d686-s.woff2") format("woff2");unicode-range:U+0100-02ba,U+02bd-02c5,U+02c7-02cc,U+02ce-02d7,U+02dd-02ff,U+0304,U+0308,U+0329,U+1d00-1dbf,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20c4,U+2113,U+2c60-2c7f,U+a720-a7ff}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:400;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/68180864d7f93f02-s.p.woff2") format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:700;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/aa1b27f9e325731f-s.woff2") format("woff2");unicode-range:U+0460-052f,U+1c80-1c8a,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:700;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/c126d80dc21dff90-s.woff2") format("woff2");unicode-range:U+0301,U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:700;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/e850464f9dfbb75b-s.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:700;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/357067f10075d686-s.woff2") format("woff2");unicode-range:U+0100-02ba,U+02bd-02c5,U+02c7-02cc,U+02ce-02d7,U+02dd-02ff,U+0304,U+0308,U+0329,U+1d00-1dbf,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20c4,U+2113,U+2c60-2c7f,U+a720-a7ff}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:700;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/68180864d7f93f02-s.p.woff2") format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:800;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/aa1b27f9e325731f-s.woff2") format("woff2");unicode-range:U+0460-052f,U+1c80-1c8a,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:800;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/c126d80dc21dff90-s.woff2") format("woff2");unicode-range:U+0301,U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:800;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/e850464f9dfbb75b-s.woff2") format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:800;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/357067f10075d686-s.woff2") format("woff2");unicode-range:U+0100-02ba,U+02bd-02c5,U+02c7-02cc,U+02ce-02d7,U+02dd-02ff,U+0304,U+0308,U+0329,U+1d00-1dbf,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20c4,U+2113,U+2c60-2c7f,U+a720-a7ff}
@font-face{font-family:Nunito Sans;font-style:normal;font-weight:800;font-stretch:100%;font-display:swap;src:url("https://www2.chromatic.com/_next/static/media/68180864d7f93f02-s.p.woff2") format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column desktop introduction with title on one side and explanatory copy and actions on the other. Follow with a full-width sequence of visual test examples. Pricing centers the introduction over four aligned plan columns; mobile stacks copy, demonstrations and plans.

Spacing scale: xs 6px, sm 8px, md 16px, lg 24px, xl 32px, section 32px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is relative, 32px high, with 0px left and 0px right padding. The sampled nav is relative, 32px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `450px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgb(255, 255, 255) 0px 0px 0px 1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact blue pill actions, fine outlined companions, small announcement chips, softly bordered plan panels and clear feature checks. Let vivid color appear inside demonstrations while navigation and reading surfaces remain restrained.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 8px / 8px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses UI specimens, visual comparison diagrams and colorful workflow bands. Create original generic interface examples and test-state diagrams without copying screenshots, product content or customer marks.

**Motion.** Observed CSS transition declarations include `color, background-color 0.2s, 0.2s`, `all 0.15s`, `all 0.16s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, confident and practical, with clear testing, review and collaboration terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
