---
version: alpha
name: "Porsche"
description: "Porsche's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Porsche."
colors:
  primary: "rgb(1, 2, 5)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgba(26, 26, 30, 0.7)"
  border: "rgb(255, 255, 255)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Porsche Next", "Arial Narrow", Arial, "Heiti SC", SimHei, sans-serif'
    fontSize: 43.104px
    fontWeight: 400
    lineHeight: 1.26
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Porsche Next", "Arial Narrow", Arial, "Heiti SC", SimHei, sans-serif'
    fontSize: 26.724px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: 0em
  heading:
    fontFamily: '"Porsche Next", "Arial Narrow", Arial, "Heiti SC", SimHei, sans-serif'
    fontSize: 25.904px
    fontWeight: 400
    lineHeight: 1.36
    letterSpacing: 0em
  body:
    fontFamily: '"Porsche Next", "Arial Narrow", Arial, "Heiti SC", SimHei, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Porsche Next", "Arial Narrow", Arial, "Heiti SC", SimHei, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 0px
  card: 12px
spacing:
  xs: 2.4px
  sm: 6.6px
  md: 16px
  lg: 30px
  xl: 32.6px
  section: 62.6px
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

# Porsche DESIGN.md

## Overview

An automotive product presentation combines cinematic media, Porsche Next typography, monochrome actions, and precise model information. Large visual chapters contrast with pale configurator surfaces, softly rounded model panels, and carefully aligned technical labels.

Built from [/usa/](https://www.porsche.com/usa/) and [/usa/models/](https://www.porsche.com/usa/models/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(1, 2, 5)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgba(26, 26, 30, 0.7)` | Supporting text |
| border | `rgb(255, 255, 255)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Porsche Next" | 43.104px | 400 | 1.26 | 0em |
| display-mobile | "Porsche Next" | 26.724px | 400 | 1.35 | 0em |
| heading | "Porsche Next" | 25.904px | 400 | 1.36 | 0em |
| body | "Porsche Next" | 16px | 400 | 1.5 | 0em |
| action | "Porsche Next" | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-bold.1796b39.woff2") format("woff2"); unicode-range: U+600-671, U+6A1, U+6A4, U+6BA, U+6CC, U+6D5, U+6F8-6F9; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-regular.413b375.woff2") format("woff2"); unicode-range: U+600-671, U+6A1, U+6A4, U+6BA, U+6CC, U+6D5, U+6F8-6F9; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-bold.4cb90bb.woff2") format("woff2"); unicode-range: U+400-4FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-regular.b845952.woff2") format("woff2"); unicode-range: U+400-4FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-semi-bold.378f7d5.woff2") format("woff2"); unicode-range: U+400-4FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-bold.d2546b1.woff2") format("woff2"); unicode-range: U+370-3FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-regular.0b3d9b3.woff2") format("woff2"); unicode-range: U+370-3FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-semi-bold.f3a9ae0.woff2") format("woff2"); unicode-range: U+370-3FF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-bold.0fbdc6d.woff2") format("woff2"); unicode-range: U+20-36F, U+1E00-1EFF, U+2000-20CF, U+2100-22FF, U+25A0-26FF, U+FB00-FB4F, U+FE70-FEFF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-regular.b8f1c20.woff2") format("woff2"); unicode-range: U+20-36F, U+1E00-1EFF, U+2000-20CF, U+2100-22FF, U+25A0-26FF, U+FB00-FB4F, U+FE70-FEFF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-semi-bold.b5f6fca.woff2") format("woff2"); unicode-range: U+20-36F, U+1E00-1EFF, U+2000-20CF, U+2100-22FF, U+25A0-26FF, U+FB00-FB4F, U+FE70-FEFF; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-bold.f30f194.woff2") format("woff2"); unicode-range: U+67C, U+67E, U+681-682, U+685-686, U+689, U+693, U+696, U+698, U+69A, U+6A9, U+6AB, U+6AF, U+6BC, U+6CD, U+6D0; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-regular.3989814.woff2") format("woff2"); unicode-range: U+67C, U+67E, U+681-682, U+685-686, U+689, U+693, U+696, U+698, U+69A, U+6A9, U+6AB, U+6AF, U+6BC, U+6CD, U+6D0; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-bold.b9e9f23.woff2") format("woff2"); unicode-range: U+E00-E7F; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-regular.ac04c30.woff2") format("woff2"); unicode-range: U+E00-E7F; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-semi-bold.8d53572.woff2") format("woff2"); unicode-range: U+E00-E7F; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 700; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-bold.49a86a4.woff2") format("woff2"); unicode-range: U+679, U+688, U+691, U+6BE, U+6C0-6C3, U+6D2-6D5, U+6F0-6F9; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 400; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-regular.ad23819.woff2") format("woff2"); unicode-range: U+679, U+688, U+691, U+6BE, U+6C0-6C3, U+6D2-6D5, U+6F0-6F9; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-bold.1796b39.woff2") format("woff2"); unicode-range: U+600-671, U+6A1, U+6A4, U+6BA, U+6CC, U+6D5, U+6F8-6F9; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-bold.f30f194.woff2") format("woff2"); unicode-range: U+67C, U+67E, U+681-682, U+685-686, U+689, U+693, U+696, U+698, U+69A, U+6A9, U+6AB, U+6AF, U+6BC, U+6CD, U+6D0; font-display: swap; }
@font-face { font-family: "Porsche Next"; font-style: normal; font-weight: 600; src: url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-bold.49a86a4.woff2") format("woff2"); unicode-range: U+679, U+688, U+691, U+6BE, U+6C0-6C3, U+6D2-6D5, U+6F0-6F9; font-display: swap; }
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-bold.1796b39.woff2")format("woff2");unicode-range:U+600-671,U+6A1,U+6A4,U+6BA,U+6CC,U+6D5,U+6F8-6F9;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-regular.413b375.woff2")format("woff2");unicode-range:U+600-671,U+6A1,U+6A4,U+6BA,U+6CC,U+6D5,U+6F8-6F9;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-bold.4cb90bb.woff2")format("woff2");unicode-range:U+4??;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-regular.b845952.woff2")format("woff2");unicode-range:U+4??;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-cyril-semi-bold.378f7d5.woff2")format("woff2");unicode-range:U+4??;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-bold.d2546b1.woff2")format("woff2");unicode-range:U+370-3FF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-regular.0b3d9b3.woff2")format("woff2");unicode-range:U+370-3FF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-greek-semi-bold.f3a9ae0.woff2")format("woff2");unicode-range:U+370-3FF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-bold.0fbdc6d.woff2")format("woff2");unicode-range:U+20-36F,U+1E??,U+2000-20CF,U+2100-22FF,U+25A0-26FF,U+FB00-FB4F,U+FE70-FEFF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-regular.b8f1c20.woff2")format("woff2");unicode-range:U+20-36F,U+1E??,U+2000-20CF,U+2100-22FF,U+25A0-26FF,U+FB00-FB4F,U+FE70-FEFF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-latin-semi-bold.b5f6fca.woff2")format("woff2");unicode-range:U+20-36F,U+1E??,U+2000-20CF,U+2100-22FF,U+25A0-26FF,U+FB00-FB4F,U+FE70-FEFF;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-bold.f30f194.woff2")format("woff2");unicode-range:U+67C,U+67E,U+681-682,U+685-686,U+689,U+693,U+696,U+698,U+69A,U+6A9,U+6AB,U+6AF,U+6BC,U+6CD,U+6D0;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-regular.3989814.woff2")format("woff2");unicode-range:U+67C,U+67E,U+681-682,U+685-686,U+689,U+693,U+696,U+698,U+69A,U+6A9,U+6AB,U+6AF,U+6BC,U+6CD,U+6D0;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-bold.b9e9f23.woff2")format("woff2");unicode-range:U+E00-E7F;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-regular.ac04c30.woff2")format("woff2");unicode-range:U+E00-E7F;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-thai-semi-bold.8d53572.woff2")format("woff2");unicode-range:U+E00-E7F;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:700;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-bold.49a86a4.woff2")format("woff2");unicode-range:U+679,U+688,U+691,U+6BE,U+6C0-6C3,U+6D2-6D5,U+6F0-6F9;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:400;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-regular.ad23819.woff2")format("woff2");unicode-range:U+679,U+688,U+691,U+6BE,U+6C0-6C3,U+6D2-6D5,U+6F0-6F9;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-arabic-bold.1796b39.woff2")format("woff2");unicode-range:U+600-671,U+6A1,U+6A4,U+6BA,U+6CC,U+6D5,U+6F8-6F9;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-pashto-bold.f30f194.woff2")format("woff2");unicode-range:U+67C,U+67E,U+681-682,U+685-686,U+689,U+693,U+696,U+698,U+69A,U+6A9,U+6AB,U+6AF,U+6BC,U+6CD,U+6D0;font-display:swap}
@font-face{font-family:Porsche Next;font-style:normal;font-weight:600;src:url("https://cdn.ui.porsche.com/porsche-design-system/fonts/porsche-next-urdu-bold.49a86a4.woff2")format("woff2");unicode-range:U+679,U+688,U+691,U+6BE,U+6C0-6C3,U+6D2-6D5,U+6F0-6F9;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a sparse overlay navigation on a full-width visual opening, followed by large model or editorial tiles and broad feature chapters. The model overview introduces a filter rail beside a multi-column vehicle grid, with key specifications and paired actions grouped consistently. Stack models and expose filters compactly on mobile.

Spacing scale: xs 2.4px, sm 6.6px, md 16px, lg 30px, xl 32.6px, section 62.6px. Use smaller steps within a control and larger steps between content groups.



Measured desktop grid tracks: `[full-start] 26px [wide-start] 54.875px [extended-start] 54.875px [basic-start] 54.875px 54.875px [narrow-start] 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px [narrow-end] 54.875px 54.875px [basic-end] 54.875px [extended-end] 54.875px [wide-end] 26px [full-end]` with gap `0px 30px`; `[full-start] 26px [wide-start] 54.875px [extended-start] 54.875px [basic-start] 54.875px 54.875px [narrow-start] 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px [narrow-end] 54.875px 54.875px [basic-end] 54.875px [extended-end] 54.875px [wide-end] 26px [full-end]` with gap `0px 30px`; `[full-start] 26px [wide-start] 54.875px [extended-start] 54.875px [basic-start] 54.875px 54.875px [narrow-start] 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px 54.875px [narrow-end] 54.875px 54.875px [basic-end] 54.875px [extended-end] 54.875px [wide-end] 26px [full-end]` with gap `0px 30px`. Build them as a fluid grid. Sampled container maximum widths: `2560px`, `1880px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use clear dark primary and light or outlined secondary actions, image-led rounded model cards, concise specification rows, conventional labeled filters, and comparison checkboxes. Preserve compact control geometry and more generous panel rounding as separate roles.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 85.4531px, horizontal padding 13.2px / 13.2px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original studio or landscape photography, neutral material detail, and generic vehicle silhouettes. Product media may fill wide cinematic frames. Do not reproduce vehicle renders, source photographs, wordmarks, crests, or model lettering.

**Motion.** Observed CSS transition declarations include `width 0.6s`, `opacity, transform, background-color 0.4s, 0.6s, 0.25s`, `scale, opacity, visibility, translate 0.4s, 0.4s, 0.4s, 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident, concise, and technically specific.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
