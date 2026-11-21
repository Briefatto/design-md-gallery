---
version: alpha
name: "Clerk"
description: "Clerk's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Clerk."
colors:
  primary: "rgb(19, 19, 22)"
  background: "rgb(247, 247, 248)"
  surface: "rgba(248, 248, 248, 0.9)"
  foreground: "rgb(19, 19, 22)"
  muted: "rgb(94, 95, 110)"
  border: "rgb(217, 217, 222)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(108, 71, 255)"
typography:
  display:
    fontFamily: 'geistNumbers, suisse, "suisse Fallback"'
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.14
    letterSpacing: -0.035em
  display-mobile:
    fontFamily: 'geistNumbers, suisse, "suisse Fallback"'
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: -0.015em
  heading:
    fontFamily: 'geistNumbers, suisse, "suisse Fallback"'
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: -0.015em
  body:
    fontFamily: 'geistNumbers, suisse, "suisse Fallback"'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0em
  action:
    fontFamily: 'geistNumbers, suisse, "suisse Fallback"'
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 12px
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

# Clerk DESIGN.md

## Overview

An authentication site pairs strong neutral headlines with precise, softly elevated interface demonstrations. The light homepage and dark pricing route share compact controls, fine borders and selective violet emphasis.

Built from [/](https://clerk.com/) and [/pricing](https://clerk.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(19, 19, 22)` | Priority actions and selected emphasis |
| background | `rgb(247, 247, 248)` | Page canvas |
| surface | `rgba(248, 248, 248, 0.9)` | Panels and cards |
| foreground | `rgb(19, 19, 22)` | Primary text |
| muted | `rgb(94, 95, 110)` | Supporting text |
| border | `rgb(217, 217, 222)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(108, 71, 255)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | geistNumbers | 56px | 700 | 1.14 | -0.035em |
| display-mobile | geistNumbers | 32px | 600 | 1.12 | -0.015em |
| heading | geistNumbers | 32px | 600 | 1.12 | -0.015em |
| body | geistNumbers | 15px | 400 | 1.6 | 0em |
| action | geistNumbers | 15px | 500 | 1.6 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:geistNumbers;src:url("https://clerk.com/_next/static/immutable/media/GeistVariableVF_numbers.p.3we0i3od0iush.woff2")format("woff2");font-display:swap}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_Bold-s.p.3apq79xsdhsa_.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_BoldItalic-s.p.26zpp78ejlsbh.woff2")format("woff2");font-display:swap;font-weight:700;font-style:italic}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_SemiBold-s.p.3lstdh700wb75.woff2")format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_SemiBoldItalic-s.p.3pdf515_t0wa_.woff2")format("woff2");font-display:swap;font-weight:600;font-style:italic}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_Medium-s.p.3034-r-4niicv.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_MediumItalic-s.p.3grtn8jczn3z6.woff2")format("woff2");font-display:swap;font-weight:500;font-style:italic}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_Book-s.p.1tp558au52mp8.woff2")format("woff2");font-display:swap;font-weight:450;font-style:normal}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_BookItalic-s.p.1qky57xzagphu.woff2")format("woff2");font-display:swap;font-weight:450;font-style:italic}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_Regular-s.p.0z_z2ccbdvksh.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:suisse;src:url("https://clerk.com/_next/static/immutable/media/SuisseIntl_RegularItalic-s.p.3rfru8unvf3x7.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}

```

The full fallback stacks are in the front matter.

## Layout

Start with a left-aligned introduction above a wide tabbed demonstration panel. Arrange light form examples as layered product scenes. Pricing switches to a dark technical backdrop and four aligned plan columns; mobile stacks demonstrations and plans.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 42px high, with 0px left and 0px right padding. The sampled header is relative, 155.688px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `297px 297px 297px 297px` with gap `4px`; `89.3906px` with gap `normal`; `30px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `1136px`, `614.4px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(66, 67, 77) 0px 0px 0px 0.5px, oklab(0.999994 0.0000455678 0.0000200868 / 0.07) 0px 1px 0px 0px inset, oklab(0.249859 0.00254738 -0.00901626 / 0.2) 0px 1px 3px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use segmented tabs, small rounded inputs, compact dark actions, violet priority accents and subtle inset outlines. Form demos have distinct headers, social actions and footer rows; plan cards use repeated feature checks and billing selectors.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 30px, horizontal padding 6.24px / 12px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 50%, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The site illustrates authentication with real product forms and subtle technical linework. Use original generic form diagrams and abstract circuit geometry rather than copying screens, brand marks or example account data.

**Motion.** Observed CSS transition declarations include `grid-template-columns, background-color, color 0.13s, 0.1s, 0.1s`, `color, background-color, border-color, box-shadow 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, practical and developer-oriented, with concise action labels and explicit feature descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
