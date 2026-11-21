---
version: alpha
name: "Hugging Face"
description: "Hugging Face's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Hugging Face."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(255, 255, 255)"
  surface: "oklch(0.985 0.002 247.839)"
  foreground: "oklch(0.21 0.034 264.665)"
  muted: "oklch(0.551 0.027 264.364)"
  border: "oklch(0.928 0.006 264.531)"
  on-primary: "rgb(255, 255, 255)"
  accent: "oklch(0.623 0.214 259.815)"
typography:
  display:
    fontFamily: '"Source Sans Pro", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Source Sans Pro", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
    letterSpacing: 0em
  heading:
    fontFamily: '"Source Sans Pro", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Source Sans Pro", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Source Sans Pro", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 8px
spacing:
  xs: 4px
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

# Hugging Face DESIGN.md

## Overview

A machine-learning community platform combines a clean white discovery interface with a large dark hero panel, Source Sans Pro typography and dense model or application metadata. Colorful demonstrations and small category signals sit within a restrained neutral shell.

Built from [/](https://huggingface.co/) and [/pricing](https://huggingface.co/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `oklch(0.985 0.002 247.839)` | Panels and cards |
| foreground | `oklch(0.21 0.034 264.665)` | Primary text |
| muted | `oklch(0.551 0.027 264.364)` | Supporting text |
| border | `oklch(0.928 0.006 264.531)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `oklch(0.623 0.214 259.815)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Source Sans Pro" | 48px | 700 | 1 | 0em |
| display-mobile | "Source Sans Pro" | 36px | 700 | 1.11 | 0em |
| heading | "Source Sans Pro" | 30px | 700 | 1.2 | 0em |
| body | "Source Sans Pro" | 16px | 400 | 1.5 | 0em |
| action | "Source Sans Pro" | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-ext-400-normal.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-400-normal.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-ext-400-normal.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-400-normal.woff2")format("woff2");unicode-range:U+370-3FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-vietnamese-400-normal.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-ext-400-normal.woff2")format("woff2");unicode-range:U+100-2AF,U+304,U+308,U+329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-400-normal.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-ext-600-normal.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-600-normal.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-ext-600-normal.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-600-normal.woff2")format("woff2");unicode-range:U+370-3FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-vietnamese-600-normal.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-ext-600-normal.woff2")format("woff2");unicode-range:U+100-2AF,U+304,U+308,U+329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:600;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-600-normal.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-ext-700-normal.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-700-normal.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-ext-700-normal.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-700-normal.woff2")format("woff2");unicode-range:U+370-3FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-vietnamese-700-normal.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-ext-700-normal.woff2")format("woff2");unicode-range:U+100-2AF,U+304,U+308,U+329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Source Sans Pro;font-style:normal;font-weight:700 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-700-normal.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-ext-400-italic.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-400-italic.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-ext-400-italic.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-400-italic.woff2")format("woff2");unicode-range:U+370-3FF}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-vietnamese-400-italic.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-ext-400-italic.woff2")format("woff2");unicode-range:U+100-2AF,U+304,U+308,U+329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:400;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-400-italic.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-ext-700-italic.woff2")format("woff2");unicode-range:U+460-52F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-cyrillic-700-italic.woff2")format("woff2");unicode-range:U+301,U+400-45F,U+490-491,U+4B0-4B1,U+2116}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-ext-700-italic.woff2")format("woff2");unicode-range:U+1F??}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-greek-700-italic.woff2")format("woff2");unicode-range:U+370-3FF}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-vietnamese-700-italic.woff2")format("woff2");unicode-range:U+102-103,U+110-111,U+128-129,U+168-169,U+1A0-1A1,U+1AF-1B0,U+300-301,U+303-304,U+308-309,U+323,U+329,U+1EA0-1EF9,U+20AB}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-ext-700-italic.woff2")format("woff2");unicode-range:U+100-2AF,U+304,U+308,U+329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:Source Sans Pro;font-style:italic;font-weight:600 900;font-display:swap;src:url("https://huggingface.co/front/assets/fonts/source-sans-pro-latin-700-italic.woff2")format("woff2");unicode-range:U+??,U+131,U+152-153,U+2BB-2BC,U+2C6,U+2DA,U+2DC,U+304,U+308,U+329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
```

The full fallback stacks are in the front matter.

## Layout

Keep a compact search-led header above a rounded dark homepage introduction and repeated model, application and dataset cards. Pricing uses three primary account columns separated by fine rules, followed by detailed usage tables. Mobile stacks the cards and account summaries while retaining readable access to dense comparisons.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 65px high, with 0px left and 0px right padding. The sampled header is static, 24px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `400px 400px 400px` with gap `24px`; `320px 320px 320px` with gap `32px`; `232px 232px 232px 232px` with gap `32px`. Build them as a fluid grid. Sampled container maximum widths: `512px`, `1280px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 2px 4px 0px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact outlined search fields, small category chips, softly bordered discovery cards, quiet pill actions and precise metadata rows. Premium and featured surfaces may use selective gradients, while tabular pricing details use monospace roles for alignment.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 30px, horizontal padding 8px / 10px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgb(255, 255, 255), and border 0px oklch(0.551 0.027 264.364). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses an emoji-like mascot, community application thumbnails and technical product diagrams. Use original generic model and dataset specimens without copying the mascot, thumbnails, screenshots or organization marks.

**Motion.** Observed CSS transition declarations include `all 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, technical and community-oriented, with concise labels and specific model, dataset and compute terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
