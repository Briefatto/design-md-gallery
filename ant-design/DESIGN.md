---
version: alpha
name: "Ant Design"
description: "Ant Design's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Ant Design."
colors:
  primary: "rgb(22, 119, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(240, 243, 250)"
  foreground: "rgba(0, 0, 0, 0.88)"
  muted: "rgba(0, 0, 0, 0.65)"
  border: "rgb(217, 217, 217)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'AlibabaSans, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 76px
    fontWeight: 900
    lineHeight: 1.21
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'AlibabaSans, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 76px
    fontWeight: 900
    lineHeight: 1.21
    letterSpacing: 0em
  heading:
    fontFamily: 'Avenir, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji", sans-serif'
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0em
  body:
    fontFamily: 'AlibabaSans, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
    letterSpacing: 0em
  action:
    fontFamily: 'AlibabaSans, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
    letterSpacing: 0em
rounded:
  control: 6px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 50px
components:
  primary-button:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.control}"
---

# Ant Design DESIGN.md

## Overview

A light enterprise interface balances a spacious, centered marketing introduction with dense, practical component documentation. Soft pastel atmosphere appears behind the hero; the controls stay crisp, economical, and blue-led.

Built from [/](https://ant.design/) and [/components/button/](https://ant.design/components/button/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(22, 119, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(240, 243, 250)` | Panels and cards |
| foreground | `rgba(0, 0, 0, 0.88)` | Primary text |
| muted | `rgba(0, 0, 0, 0.65)` | Supporting text |
| border | `rgb(217, 217, 217)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | AlibabaSans | 76px | 900 | 1.21 | 0em |
| display-mobile | AlibabaSans | 76px | 900 | 1.21 | 0em |
| heading | Avenir | 24px | 500 | 1.33 | 0em |
| body | AlibabaSans | 14px | 400 | 2 | 0em |
| action | AlibabaSans | 14px | 400 | 1.57 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-family: AlibabaSans; font-style: normal; font-weight: 300; font-display: optional; src: url("https://mdn.alipayobjects.com/huamei_iwk9zp/afts/file/A*1GSgSYDD_aIAAAAAQsAAAAgAegCCAQ/AlibabaSans-Light.woff2") format("woff2"); }
@font-face { font-family: AlibabaSans; font-style: normal; font-weight: 400; font-display: optional; src: url("https://mdn.alipayobjects.com/huamei_iwk9zp/afts/file/A*2zEUQqnPNesAAAAAQtAAAAgAegCCAQ/AlibabaSans-Regular.woff2") format("woff2"); }
@font-face { font-family: AlibabaSans; font-style: normal; font-weight: 500; font-display: optional; src: url("https://mdn.alipayobjects.com/huamei_iwk9zp/afts/file/A*E_cxRbMlZqUAAAAAQuAAAAgAegCCAQ/AlibabaSans-Bold.woff2") format("woff2"); }
@font-face { font-family: AlibabaSans; font-style: normal; font-weight: 600; font-display: optional; src: url("https://mdn.alipayobjects.com/huamei_iwk9zp/afts/file/A*E_cxRbMlZqUAAAAAQuAAAAgAegCCAQ/AlibabaSans-Bold.woff2") format("woff2"); }
@font-face { font-family: AlibabaSans; font-style: normal; font-weight: 700; font-display: optional; src: url("https://mdn.alipayobjects.com/huamei_iwk9zp/afts/file/A*E_cxRbMlZqUAAAAAQuAAAAgAegCCAQ/AlibabaSans-Bold.woff2") format("woff2"); }
```

The full fallback stacks are in the front matter.

## Layout

Use a full-width top navigation, centered introductory copy, and a horizontal row of announcement cards. Documentation introduces a left component rail, a main reading column, and a slim in-page contents rail. The captured mobile documentation keeps several rails crowded together; improve reading access in an adaptation rather than preserving that compression.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 50px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 0px left and 0px right padding. The sampled header is sticky, 64px high, with 0px left and 0px right padding.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0.08) 0px 4px 12px 0px, rgba(0, 0, 0, 0.08) 0px 12px 32px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

The defining vocabulary is a compact blue filled action, a quiet outlined companion, short-radius white cards, small status badges, and many narrowly spaced documentation controls. Keep explanatory examples visibly separated from the page chrome.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 32px, horizontal padding 15px / 15px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 32px, radius 20px, background rgba(0, 0, 0, 0), and border 0px rgba(0, 0, 0, 0.88). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use abstract pastel glows, simple geometric diagrams, and small outlined interface icons. Product demonstrations may be represented with original neutral UI diagrams; do not copy the site's icons, logos, or example artwork.

**Motion.** Observed CSS transition declarations include `background-color 1s`, `all 0.2s`, `color 0.3s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful, instructional, and specific. Use short action labels and concise explanations of component purpose and behavior.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't turn the restrained enterprise controls into oversized pill buttons or add heavy shadows to every documentation block.

