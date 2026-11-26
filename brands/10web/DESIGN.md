---
version: alpha
name: "10Web"
description: "10Web's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with 10Web."
colors:
  primary: "rgb(51, 57, 241)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(248, 248, 248)"
  foreground: "rgb(20, 21, 31)"
  muted: "rgba(20, 21, 31, 0.7)"
  border: "rgba(20, 21, 31, 0.12)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Evergrow Sans", sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Evergrow Sans", sans-serif'
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0em
  heading:
    fontFamily: '"Evergrow Sans", "Plus Jakarta Sans", system-ui, -apple-system, "Segoe UI", sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0em
  body:
    fontFamily: '"Evergrow Sans", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Evergrow Sans", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 8px
  card: 24px
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

# 10Web DESIGN.md

## Overview

An AI website builder pairs open sans-serif typography, white surfaces, vivid indigo atmosphere and a large prompt-entry panel. The pricing route simplifies that expressive introduction into clear neutral comparison cards.

Built from [/](https://10web.io/) and [/pricing](https://10web.io/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(51, 57, 241)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(248, 248, 248)` | Panels and cards |
| foreground | `rgb(20, 21, 31)` | Primary text |
| muted | `rgba(20, 21, 31, 0.7)` | Supporting text |
| border | `rgba(20, 21, 31, 0.12)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Evergrow Sans" | 40px | 500 | 1.3 | 0em |
| display-mobile | "Evergrow Sans" | 30px | 500 | 1.33 | 0em |
| heading | "Evergrow Sans" | 40px | 500 | 1.3 | 0em |
| body | "Evergrow Sans" | 16px | 400 | 1.5 | 0em |
| action | "Evergrow Sans" | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Evergrow Sans"; font-weight: 300; font-display: swap; src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-light.woff") format("woff"); }
@font-face { font-family: "Evergrow Sans"; font-weight: 400; font-display: swap; src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-regular.woff") format("woff"); }
@font-face { font-family: "Evergrow Sans"; font-weight: 500; font-display: swap; src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-medium.woff") format("woff"); }
@font-face { font-family: "Evergrow Sans"; font-weight: 700; font-display: swap; src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-bold.woff") format("woff"); }
@font-face { font-family: "Evergrow Sans"; font-weight: 800; font-display: swap; src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-extrabold.woff") format("woff"); }
@font-face {
  font-family: 'Evergrow Sans';
  font-weight: 300;
  font-display: swap;;
  src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-light.woff")
    format('woff');
}
@font-face {
  font-family: 'Evergrow Sans';
  font-weight: 400;
  font-display: swap;;
  src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-regular.woff")
    format('woff');
}
@font-face {
  font-family: 'Evergrow Sans';
  font-weight: 500;
  font-display: swap;;
  src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-medium.woff")
    format('woff');
}
@font-face {
  font-family: 'Evergrow Sans';
  font-weight: 700;
  font-display: swap;;
  src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-bold.woff")
    format('woff');
}
@font-face {
  font-family: 'Evergrow Sans';
  font-weight: 800;
  font-display: swap;;
  src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-woff/evergrowsans-extrabold.woff")
    format('woff');
}
@font-face {
    font-family: 'Evergrow Sans';
    font-weight: 300;
    font-display: swap;;
    src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-ttf/evergrowsans-light.ttf") format('truetype');
}
@font-face {
    font-family: 'Evergrow Sans';
    font-weight: 400;
    font-display: swap;;
    src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-ttf/evergrowsans-regular.ttf") format('truetype');
}
@font-face {
    font-family: 'Evergrow Sans';
    font-weight: 500;
    font-display: swap;;
    src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-ttf/evergrowsans-medium.ttf") format('truetype');
}
@font-face {
    font-family: 'Evergrow Sans';
    font-weight: 700;
    font-display: swap;;
    src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-ttf/evergrowsans-bold.ttf") format('truetype');
}
@font-face {
    font-family: 'Evergrow Sans';
    font-weight: 800;
    font-display: swap;;
    src: url("https://10web.io/wp-content/themes/10web-theme/css/fonts/evergrow-sans/evergrow-sans-ttf/evergrowsans-extrabold.ttf") format('truetype');
}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage title and prompt panel over a textured indigo field, then introduce proof content and alternating product sections. Pricing places its introduction above business and billing selectors and a repeated plan grid. Mobile stacks plans and keeps the prompt controls compact.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 81px high, with 0px left and 0px right padding. The sampled nav is static, 48px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `408px 408px 408px` with gap `24px`; `624px 624px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `24px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use modestly rounded indigo creation actions, near-black pricing actions, softly outlined prompt fields, small attachment or link chips, thin plan borders and quiet discount badges. Keep vivid atmosphere outside dense reading and comparison areas.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 46px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(20, 21, 31). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses textured color fields, product demonstrations and review imagery. Create original abstract textures and generic builder-workflow diagrams without copying screenshots, portraits, artwork or customer marks.

**Motion.** Observed CSS transition declarations include `background 0.2s`, `background-color, color 0.2s, 0.2s`, `color, background-color 0.15s, 0.15s`, `color 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, practical and encouraging, with concise creation and upgrade labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
