---
version: alpha
name: "Bulma"
description: "Bulma's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Bulma."
colors:
  primary: "rgb(0, 209, 178)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(249, 250, 251)"
  foreground: "rgb(31, 34, 41)"
  muted: "rgb(117, 119, 99)"
  border: "rgb(214, 217, 224)"
  on-primary: "rgb(0, 31, 26)"
  accent: "rgb(66, 88, 255)"
typography:
  display:
    fontFamily: 'Inter, "SF Pro", "Segoe UI", Roboto, Oxygen, Ubuntu, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 64px
    fontWeight: 800
    lineHeight: 1.13
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Inter, "SF Pro", "Segoe UI", Roboto, Oxygen, Ubuntu, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 48px
    fontWeight: 800
    lineHeight: 1.13
    letterSpacing: 0em
  heading:
    fontFamily: 'Inter, "SF Pro", "Segoe UI", Roboto, Oxygen, Ubuntu, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 48px
    fontWeight: 800
    lineHeight: 1.13
    letterSpacing: 0em
  body:
    fontFamily: 'Inter, "SF Pro", "Segoe UI", Roboto, Oxygen, Ubuntu, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, "SF Pro", "Segoe UI", Roboto, Oxygen, Ubuntu, "Helvetica Neue", Helvetica, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0em
rounded:
  control: 6px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 48px
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

# Bulma DESIGN.md

## Overview

A CSS framework site combines bright turquoise actions, approachable Inter typography, white surfaces and colorful supporting category signals. Documentation turns that vocabulary into a structured reading interface with fine borders and modest rounded cards.

Built from [/](https://bulma.io/) and [/documentation/](https://bulma.io/documentation/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 209, 178)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(249, 250, 251)` | Panels and cards |
| foreground | `rgb(31, 34, 41)` | Primary text |
| muted | `rgb(117, 119, 99)` | Supporting text |
| border | `rgb(214, 217, 224)` | Quiet separators and outlines |
| on-primary | `rgb(0, 31, 26)` | Text on the primary action |
| accent | `rgb(66, 88, 255)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Inter | 64px | 800 | 1.13 | 0em |
| display-mobile | Inter | 48px | 800 | 1.13 | 0em |
| heading | Inter | 48px | 800 | 1.13 | 0em |
| body | Inter | 18px | 400 | 1.5 | 0em |
| action | Inter | 16px | 500 | 1.25 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

The captured stack resolves through installed/system fonts. No font download is required for the fallback stack.

The full fallback stacks are in the front matter.

The captured first-choice font was unavailable on the public source pages and no resolvable loading reference was observed. The generic preview explicitly starts at Arial, an available fallback from the captured CSS stack. The guide and tokens retain the original declared stack and measured metrics; preview font substitution is an adaptation.

## Layout

Use a centered homepage introduction above feature summaries and component demonstrations. Documentation adds a dense left category rail and a main article column with repeated topic cards. On mobile, collapse the rail and stack cards with a clear reading measure.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 104px high, with 32px left and 32px right padding. The sampled header is static, 40.5px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `320px 320px 320px 320px` with gap `32px`; `256px 1184px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `1344px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(51, 51, 51, 0.05) 0px 0.875px 1.75px 0px, rgba(51, 51, 51, 0.05) 0px 1.75px 3.5px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use turquoise filled actions, outlined companions, small multicolor badges, lightly rounded white cards, subtle shadows and distinct code panels. Keep category colors purposeful and maintain a stable neutral text hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 40px, radius 6px, background rgb(20, 22, 26), and border 1px rgb(53, 58, 70). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source shows interface specimens, code and occasional promotional media. Use original component examples and simple functional icons, excluding brand marks, source thumbnails and third-party advertisement imagery.

**Motion.** Observed CSS transition declarations include `background-image 0.294s`, `background-color, color 0.294s`, `opacity 0.294s`, `background-color, border-color, box-shadow, color 0.294s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Friendly, instructional and practical, with concise labels and clear explanations of implementation options.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
