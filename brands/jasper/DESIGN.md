---
version: alpha
name: "Jasper"
description: "Jasper's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Jasper."
colors:
  primary: "rgb(0, 6, 61)"
  background: "rgb(197, 231, 255)"
  surface: "rgb(249, 250, 250)"
  foreground: "rgb(0, 6, 61)"
  muted: "rgb(0, 6, 61)"
  border: "rgba(255, 255, 255, 0.2)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(250, 64, 40)"
typography:
  display:
    fontFamily: 'Feature, Georgia, sans-serif'
    fontSize: 88px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.045em
  display-mobile:
    fontFamily: 'Feature, Georgia, sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.031em
  heading:
    fontFamily: 'Feature, Georgia, sans-serif'
    fontSize: 38px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.026em
  body:
    fontFamily: '"ABC ROM", Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.016em
  action:
    fontFamily: '"ABC ROM", Arial, sans-serif'
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.4
    letterSpacing: -0.01em
rounded:
  control: 0px
  card: 0px
spacing:
  xs: 6px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 64px
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

# Jasper DESIGN.md

## Overview

An enterprise marketing site pairs large editorial serif headlines with precise sans-serif interface text, pale blue fields, deep navy ink and vivid coral accents. Fine grids and square controls give the expressive typography a disciplined structure.

Built from [/](https://jasper.ai/) and [/pricing](https://jasper.ai/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 6, 61)` | Priority actions and selected emphasis |
| background | `rgb(197, 231, 255)` | Page canvas |
| surface | `rgb(249, 250, 250)` | Panels and cards |
| foreground | `rgb(0, 6, 61)` | Primary text |
| muted | `rgb(0, 6, 61)` | Supporting text |
| border | `rgba(255, 255, 255, 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(250, 64, 40)` | Selective emphasis in headings, graphics, and small signals |



Use pale blue as a broad editorial field, white for reading and comparison surfaces, and deep navy for text and selected dark sections. Coral marks small signals and priority accents rather than tinting every control. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Feature | 88px | 400 | 1.1 | -0.045em |
| display-mobile | Feature | 40px | 400 | 1.1 | -0.031em |
| heading | Feature | 38px | 400 | 1.1 | -0.026em |
| body | "ABC ROM" | 16px | 400 | 1.4 | -0.016em |
| action | "ABC ROM" | 16px | 450 | 1.4 | -0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bb555e630d835bb44_ABC%20ROM%20-%20Bold%20Italic.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b45d4733c1bef54ad_ABC%20ROM%20-%20Bold%20Italic.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b74d687afe2829f28_ABC%20ROM%20-%20Bold%20Italic.otf") format("opentype"); font-weight: 700; font-style: italic; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b81991652a5490b89_ABC%20ROM%20-%20Bold.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1b1cb01796ef29ee_ABC%20ROM%20-%20Bold.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bc98d84759aca6334_ABC%20ROM%20-%20Bold.otf") format("opentype"); font-weight: 700; font-style: normal; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b3014ca98f774dbcd_ABC%20ROM%20-%20Medium%20Italic.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b11519d24edd5a155_ABC%20ROM%20-%20Medium%20Italic.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1c5b46e544920b1256_ABC%20ROM%20-%20Medium%20Italic.otf") format("opentype"); font-weight: 600; font-style: italic; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bb4c3114f43c7773d_ABC%20ROM%20-%20Regular.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b7d3d4344d34f17fa_ABC%20ROM%20-%20Regular.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1c45d4733c1bef55c1_ABC%20ROM%20-%20Regular.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b5b46e544920b1218_ABC%20ROM%20-%20Regular%20Italic.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b14e9b0b83c7833a4_ABC%20ROM%20-%20Regular%20Italic.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1baa7a781ca2423a0b_ABC%20ROM%20-%20Regular%20Italic.otf") format("opentype"); font-weight: 400; font-style: italic; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b5b46e544920b120b_ABC%20ROM%20-%20Medium.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bee1b984e7f43dad7_ABC%20ROM%20-%20Medium.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b8d4fd6f40d4a760d_ABC%20ROM%20-%20Medium.otf") format("opentype"); font-weight: 600; font-style: normal; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1b1cb01796ef29db_ABC%20ROM%20-%20Book%20Italic.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b6148f4b9841144f8_ABC%20ROM%20-%20Book%20Italic.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1be59ad68818336d14_ABC%20ROM%20-%20Book%20Italic.otf") format("opentype"); font-weight: 500; font-style: italic; font-display: swap; }
@font-face { font-family: "ABC ROM"; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b9bf5c756898300bd_ABC%20ROM%20-%20Book.woff2") format("woff2"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1cee1884a2d19320_ABC%20ROM%20-%20Book.woff") format("woff"), url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1cd79e341aa5fc04ee_ABC%20ROM%20-%20Book.otf") format("opentype"); font-weight: 500; font-style: normal; font-display: swap; }
@font-face { font-family: Feature; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e72729f546840cd17798a_FeatureHeadline-Upright-VF_wght_wdth_opsz.ttf") format("truetype"); font-weight: 100 900; font-style: normal; font-display: swap; }
@font-face { font-family: Feature; src: url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e72724948de7118957fe7_FeatureHeadline-Italic-VF_wght_wdth_opsz.ttf") format("truetype"); font-weight: 100 900; font-style: italic; font-display: swap; }
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bb555e630d835bb44_ABC%20ROM%20-%20Bold%20Italic.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b45d4733c1bef54ad_ABC%20ROM%20-%20Bold%20Italic.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b74d687afe2829f28_ABC%20ROM%20-%20Bold%20Italic.otf")format("opentype");font-weight:700;font-style:italic;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b81991652a5490b89_ABC%20ROM%20-%20Bold.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1b1cb01796ef29ee_ABC%20ROM%20-%20Bold.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bc98d84759aca6334_ABC%20ROM%20-%20Bold.otf")format("opentype");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b3014ca98f774dbcd_ABC%20ROM%20-%20Medium%20Italic.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b11519d24edd5a155_ABC%20ROM%20-%20Medium%20Italic.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1c5b46e544920b1256_ABC%20ROM%20-%20Medium%20Italic.otf")format("opentype");font-weight:600;font-style:italic;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bb4c3114f43c7773d_ABC%20ROM%20-%20Regular.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b7d3d4344d34f17fa_ABC%20ROM%20-%20Regular.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1c45d4733c1bef55c1_ABC%20ROM%20-%20Regular.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b5b46e544920b1218_ABC%20ROM%20-%20Regular%20Italic.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b14e9b0b83c7833a4_ABC%20ROM%20-%20Regular%20Italic.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1baa7a781ca2423a0b_ABC%20ROM%20-%20Regular%20Italic.otf")format("opentype");font-weight:400;font-style:italic;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b5b46e544920b120b_ABC%20ROM%20-%20Medium.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1bee1b984e7f43dad7_ABC%20ROM%20-%20Medium.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b8d4fd6f40d4a760d_ABC%20ROM%20-%20Medium.otf")format("opentype");font-weight:600;font-style:normal;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1b1cb01796ef29db_ABC%20ROM%20-%20Book%20Italic.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b6148f4b9841144f8_ABC%20ROM%20-%20Book%20Italic.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1be59ad68818336d14_ABC%20ROM%20-%20Book%20Italic.otf")format("opentype");font-weight:500;font-style:italic;font-display:swap}
@font-face{font-family:ABC ROM;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b9bf5c756898300bd_ABC%20ROM%20-%20Book.woff2")format("woff2"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1b1cee1884a2d19320_ABC%20ROM%20-%20Book.woff")format("woff"),url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e6f1cd79e341aa5fc04ee_ABC%20ROM%20-%20Book.otf")format("opentype");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:Feature;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e72729f546840cd17798a_FeatureHeadline-Upright-VF_wght_wdth_opsz.ttf")format("truetype");font-weight:100 900;font-style:normal;font-display:swap}
@font-face{font-family:Feature;src:url("https://cdn.prod.website-files.com/6807ee8d73c233fb82842313/680e72724948de7118957fe7_FeatureHeadline-Italic-VF_wght_wdth_opsz.ttf")format("truetype");font-weight:100 900;font-style:italic;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction above a large portrait-and-interface composition on a fine grid. Alternate broad blue, white and dark navy sections with generous reading space. Pricing centers its title above a billing switch and two square plan columns that stack on mobile.

Spacing scale: xs 6px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.



Measured desktop grid tracks: `456px 456px 456px` with gap `16px`; `318px 318px 318px 318px` with gap `16px`; `429.328px 429.328px 429.344px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `680px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use square dark actions, thin outlined companions, coral announcement labels, fine grid lines and white pricing panels. Keep display serif roles distinct from compact navigation, body copy and feature lists.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48.1875px, horizontal padding 18px / 18px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source combines editorial portraits, graphic grids and marketing workflow diagrams. Use original licensed photography and generic diagrams without copying portraits, screenshots, logos or source illustrations.

**Motion.** Observed CSS transition declarations include `transform, box-shadow, background-color 0.2s, 0.2s, 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident and practical, with clear enterprise capability descriptions and concise actions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
