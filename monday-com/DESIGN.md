---
version: alpha
name: "Monday.com"
description: "Monday.com's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Monday.com."
colors:
  primary: "rgb(97, 97, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(243, 244, 245)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(103, 104, 121)"
  border: "rgb(220, 223, 236)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Poppins, Arial, sans-serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'Poppins, Arial, sans-serif'
    fontSize: 33.25px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.04em
  heading:
    fontFamily: 'Poppins, Arial, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
  body:
    fontFamily: 'Poppins, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0em
  action:
    fontFamily: 'Poppins, Arial, sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 160px
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

# Monday.com DESIGN.md

## Overview

Poppins typography, vivid violet actions and a bright white canvas support a friendly, colorful work-management system.

Built from [/](https://monday.com/) and [/pricing](https://monday.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(97, 97, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(243, 244, 245)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(103, 104, 121)` | Supporting text |
| border | `rgb(220, 223, 236)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Poppins | 56px | 400 | 1.2 | -0.04em |
| display-mobile | Poppins | 33.25px | 400 | 1.2 | -0.04em |
| heading | Poppins | 48px | 400 | 1.1 | -0.03em |
| body | Poppins | 16px | 400 | 1.6 | 0em |
| action | Poppins | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3af2eec68d392405c0_Poppins-Light.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/69945795a31d97bc97c5055d_Poppins-Light.ttf")format("truetype");font-weight:300;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3adc600dc2a24bf3bc_Poppins-Bold.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/69945795a31d97bc97c50559_Poppins-Bold.ttf")format("truetype");font-weight:700;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3a92438adb2f958793_Poppins-Regular.woff2")format("woff2");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3abb9aeb58f85c10e4_Poppins-Medium.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/69945795a31d97bc97c50558_Poppins-Medium.ttf")format("truetype");font-weight:500;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3ada9d81bb39a02675_Poppins-Thin.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/663929e7212567566e7ee9f9_Poppins-Thin.ttf")format("truetype");font-weight:100;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3a162d1dda5f21f02c_Poppins-SemiBold.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/69945795a31d97bc97c5055b_Poppins-SemiBold.ttf")format("truetype");font-weight:600;font-style:normal;font-display:swap}
@font-face{font-family:Poppins;src:url("https://cdn.prod.website-files.com/656da6fea306219773d04208/6a355f3a19333dc78ac4b87d_Poppins-ExtraLight.woff2")format("woff2"),url("https://cdn.prod.website-files.com/656da6fea306219773d04208/69945795a31d97bc97c5055a_Poppins-ExtraLight.ttf")format("truetype");font-weight:200;font-style:normal;font-display:swap}
```

The full fallback stacks are in the front matter.

## Layout

Use a broad split homepage hero with human and agent cards, followed by logo rows and modular feature demonstrations. Pricing aligns tall plan columns under a team-size selector; the mobile capture shows a horizontal carousel centered on the featured plan.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 41.5938px high, with 0px left and 0px right padding. The sampled header is static, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `178.656px 178.672px 223.328px 178.672px 178.672px 134px` with gap `36px 16px`. Build them as a fluid grid. Sampled container maximum widths: `1372px`, `984.704px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `160px`; the reusable card treatment uses `24px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Violet pill actions, small neutral category chips, fine plan dividers and a dark featured-plan ribbon create hierarchy. Feature packs use subtle lavender surfaces and multicolor outlines, with compact icons and dense lists.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 41.5938px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 46px, radius 6px, background rgb(255, 255, 255), and border 1px rgb(197, 199, 208). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Human portraits, stylized agent characters, colorful boards and application panels explain collaborative work. Keep the illustrations framed within the otherwise spacious neutral layout.

**Motion.** Observed CSS transition declarations include `opacity 0.5s`, `all 0.25s`, `all 0.5s`, `background-color 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Friendly and action-oriented, using simple benefit statements and approachable labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
