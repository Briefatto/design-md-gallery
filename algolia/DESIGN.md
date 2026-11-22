---
version: alpha
name: "Algolia"
description: "Algolia's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Algolia."
colors:
  primary: "rgb(0, 61, 255)"
  background: "rgb(0, 0, 51)"
  surface: "rgb(6, 19, 61)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(150, 152, 195)"
  border: "rgba(255, 255, 255, 0.14)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Sora, sans-serif'
    fontSize: 77px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.052em
  display-mobile:
    fontFamily: 'Sora, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.1em
  heading:
    fontFamily: 'Sora, sans-serif'
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.31
    letterSpacing: -0.01em
  body:
    fontFamily: 'Inter, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, sans-serif'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
rounded:
  control: 9999px
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

# Algolia DESIGN.md

## Overview

A search platform site uses a midnight-blue hero, substantial rounded Sora headlines and electric blue actions, with neon green and cyan signals around product imagery. White and pale gray sections follow the darker introduction.

Built from [/](https://algolia.com/) and [/pricing](https://algolia.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 61, 255)` | Priority actions and selected emphasis |
| background | `rgb(0, 0, 51)` | Page canvas |
| surface | `rgb(6, 19, 61)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(150, 152, 195)` | Supporting text |
| border | `rgba(255, 255, 255, 0.14)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Sora | 77px | 700 | 1.05 | -0.052em |
| display-mobile | Sora | 40px | 700 | 1.05 | -0.1em |
| heading | Sora | 42px | 700 | 1.31 | -0.01em |
| body | Inter | 18px | 400 | 1.56 | 0em |
| action | Inter | 15px | 400 | 1.4 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Black.woff") format("woff"); font-weight: 900; font-display: swap; font-style: normal; }
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-ExtraBold.woff") format("woff"); font-weight: 800; font-display: swap; font-style: normal; }
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Bold.woff") format("woff"); font-weight: 700; font-display: swap; font-style: normal; }
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-SemiBold.woff") format("woff"); font-weight: 600; font-display: swap; font-style: normal; }
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Medium.woff") format("woff"); font-weight: 500; font-display: swap; font-style: normal; }
@font-face { font-family: Inter; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Regular.woff") format("woff"); font-weight: 400; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-ExtraBold.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-ExtraBold.woff") format("woff"); font-weight: 900; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Bold.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Bold.woff") format("woff"); font-weight: 700; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-SemiBold.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-SemiBold.woff") format("woff"); font-weight: 600; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Medium.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Medium.woff") format("woff"); font-weight: 500; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Regular.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Regular.woff") format("woff"); font-weight: 400; font-display: swap; font-style: normal; }
@font-face { font-family: Sora; src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Light.woff2") format("woff2"), url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Light.woff") format("woff"); font-weight: 300; font-display: swap; font-style: normal; }
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Black.woff") format('woff');
    font-weight: 900;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-ExtraBold.woff") format('woff');
    font-weight: 800;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Bold.woff") format('woff');
    font-weight: 700;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-SemiBold.woff") format('woff');
    font-weight: 600;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Medium.woff") format('woff');
    font-weight: 500;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Inter';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/inter/Inter-Regular.woff") format('woff');
    font-weight: 400;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-ExtraBold.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-ExtraBold.woff") format('woff');
    font-weight: 900;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Bold.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Bold.woff") format('woff');
    font-weight: 700;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-SemiBold.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-SemiBold.woff") format('woff');
    font-weight: 600;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Medium.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Medium.woff") format('woff');
    font-weight: 500;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Regular.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Regular.woff") format('woff');
    font-weight: 400;
    font-display: swap;
    font-style: normal;
}
@font-face {
    font-family: 'Sora';
    src: url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Light.woff2") format('woff2'),
        url("https://www.algolia.com/modules/algolia-base-template/css/fonts/sora/Sora-Light.woff") format('woff');
    font-weight: 300;
    font-display: swap;
    font-style: normal;
}
@font-face{font-family:Inter;font-style:normal;font-weight:100 900;font-display:swap;src:url("https://cdn.arcade.software/fonts/InterVariable.woff2")format("woff2")}
```

The full fallback stacks are in the front matter.

## Layout

Place a large left-aligned headline and action beside an illustrated search experience. Pricing centers the introduction above usage sliders and aligned plan columns. Mobile centers the hero and stacks the calculator and plans.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 121px high, with 0px left and 0px right padding. The sampled header is sticky, 121px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `10px` with gap `normal`; `10px` with gap `normal`; `10px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `1440px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use filled electric-blue actions, outlined navigation and search pills, thin blue plan borders, compact usage inputs and small status labels. Keep strong display type separate from the smaller Inter navigation and body roles.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 28.7812px, horizontal padding 13.6px / 13.6px, and gap 6.4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 16px, radius 3px, background rgb(255, 255, 255), and border 1px rgba(15, 17, 40, 0.3). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source combines product demonstrations, photography and luminous search graphics. Use original search diagrams and licensed photography without reproducing the screenshots, customer logos or source images.

**Motion.** Observed CSS transition declarations include `border-color, background-color, color, box-shadow, transform 0.2s, 0.2s, 0.2s, 0.2s, 0.2s`, `border-color, box-shadow 0.2s, 0.2s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.3s`, `border-color, background-color 0.15s, 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Confident and outcome-oriented, with precise search and usage terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
