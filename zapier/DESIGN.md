---
version: alpha
name: "Zapier"
description: "Zapier's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Zapier."
colors:
  primary: "rgb(255, 79, 0)"
  background: "rgb(255, 254, 251)"
  surface: "rgb(248, 244, 240)"
  foreground: "rgb(32, 21, 21)"
  muted: "rgb(96, 93, 82)"
  border: "rgb(223, 220, 210)"
  on-primary: "rgb(255, 254, 251)"
typography:
  display:
    fontFamily: '"Degular Display", DegularDisplay, "DegularDisplay Fallback", Inter, "Inter Fallback", system-ui, ui-sans-serif, sans-serif, sans-serif'
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Degular Display", DegularDisplay, "DegularDisplay Fallback", Inter, "Inter Fallback", system-ui, ui-sans-serif, sans-serif, sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0em
  heading:
    fontFamily: 'Serrif, Serrif, "Serrif Fallback", serif'
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.02em
  body:
    fontFamily: 'Inter, Inter, "Inter Fallback", system-ui, ui-sans-serif, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, Inter, "Inter Fallback", system-ui, ui-sans-serif, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 18px
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

# Zapier DESIGN.md

## Overview

Warm paper-like neutrals, dense dark ink and bright orange actions frame a precise automation system with Degular Display headings and Inter reading text.

Built from [/](https://zapier.com/) and [/pricing](https://zapier.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 79, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 254, 251)` | Page canvas |
| surface | `rgb(248, 244, 240)` | Panels and cards |
| foreground | `rgb(32, 21, 21)` | Primary text |
| muted | `rgb(96, 93, 82)` | Supporting text |
| border | `rgb(223, 220, 210)` | Quiet separators and outlines |
| on-primary | `rgb(255, 254, 251)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Degular Display" | 56px | 500 | 1 | 0em |
| display-mobile | "Degular Display" | 40px | 500 | 1 | 0em |
| heading | Serrif | 32px | 300 | 1.2 | -0.02em |
| body | Inter | 14px | 400 | 1.5 | 0em |
| action | Inter | 14px | 400 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/ba9851c3c22cd980-s.woff2") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/21350d82a1f187e9-s.woff2") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/c5fe6dc8356a8c31-s.woff2") format("woff2");unicode-range:u+1f??}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/19cfc7226ec3afaa-s.woff2") format("woff2");unicode-range:u+0370-0377,u+037a-037f,u+0384-038a,u+038c,u+038e-03a1,u+03a3-03ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/df0a9ae256c0569c-s.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/8e9860b6e62d6359-s.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c4,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/e4af272ccee01ff0-s.p.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-family:DegularDisplay;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/b9a37491f5c9eb6c-s.p.woff2") format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:DegularDisplay;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/15d6d500777bacc6-s.p.woff2") format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:DegularDisplay;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/c82ad8494f7a57ee-s.p.woff2") format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:Serrif;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/ec71a0abebc51e3c-s.p.woff2") format("woff2");font-display:swap;font-weight:300;font-style:normal}
@font-face{font-family:Serrif;src:url("https://marketing-site.vercel.zapier.com/_next/static/media/097bec17c4bcefb5-s.p.woff2") format("woff2");font-display:swap;font-weight:300;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use generous centered homepage spacing above wide media. Pricing becomes a left-aligned editorial header, large product tabs, task-volume selector and fine-ruled plan columns; mobile replaces the slider with a select control and stacks the sections.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 56px high, with 40px left and 40px right padding. The sampled header is static, 205px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `20px` with gap `normal`; `308px 308px 308px 308px` with gap `16px`; `369.219px 830.781px` with gap `80px`. Build them as a fluid grid. Sampled container maximum widths: `720px`, `768px`, `1024px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `18px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Orange priority actions, dark selected tabs, quiet outlines and compact rounded rectangles keep interactive elements clear. Thin warm-gray rules structure the dense comparison and small mono-like eyebrow labels establish hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 12px / 12px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 18px, radius 50%, background rgba(0, 0, 0, 0), and border 1px rgb(147, 144, 132). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Soft photographic motion backdrops support interface notifications and workflow demonstrations. Keep colorful app marks confined to illustrative or integration contexts.

**Motion.** Observed CSS transition declarations include `all 0.25s`, `background-color, border-color, box-shadow 0.2s, 0.2s, 0.2s`, `background-color 0.25s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Practical and optimistic, with short action labels and clear descriptions of workflow outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
