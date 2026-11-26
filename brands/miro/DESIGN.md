---
version: alpha
name: "Miro"
description: "Miro's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Miro."
colors:
  primary: "rgb(25, 24, 18)"
  background: "rgb(251, 250, 247)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(28, 28, 30)"
  muted: "rgb(102, 102, 102)"
  border: "rgb(233, 234, 239)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Apris Regular", "Apris Regular Placeholder", sans-serif'
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Apris Regular", "Apris Regular Placeholder", sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: 0em
  heading:
    fontFamily: '"Roobert PRO Regular", "Roobert PRO Regular Placeholder", sans-serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: 0em
  body:
    fontFamily: '"Roobert PRO Regular", "Roobert PRO Regular Placeholder", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Roobert PRO Medium", Helvetica, Arial, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0.01em
rounded:
  control: 8px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 48px
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

# Miro DESIGN.md

## Overview

A warm collaborative canvas uses an elegant Apris serif statement, clean Roobert text and small colorful objects on a faint dotted ground.

Built from [/](https://miro.com/) and [/pricing](https://miro.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(25, 24, 18)` | Priority actions and selected emphasis |
| background | `rgb(251, 250, 247)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(28, 28, 30)` | Primary text |
| muted | `rgb(102, 102, 102)` | Supporting text |
| border | `rgb(233, 234, 239)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Apris Regular" | 56px | 400 | 1.1 | 0em |
| display-mobile | "Apris Regular" | 40px | 400 | 1.1 | 0em |
| heading | "Roobert PRO Regular" | 36px | 400 | 1.15 | 0em |
| body | "Roobert PRO Regular" | 16px | 400 | 1.5 | 0em |
| action | "Roobert PRO Medium" | 18px | 400 | 1.2 | 0.01em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Roobert PRO Regular"; src: url("https://framerusercontent.com/assets/ydBr7kp9mqNBSElJ9WM908UYMc.woff2"); font-display: swap; font-style: normal; font-weight: 400; }
@font-face { font-family: "Apris Regular"; src: url("https://framerusercontent.com/assets/ZIRrvVTVbbK4wwTutIbU2O5U.woff2"); font-display: swap; font-style: normal; font-weight: 400; }
@font-face { font-family: "Roobert PRO Medium"; src: url("https://framerusercontent.com/assets/IWIJ9TEwVer0sH7Pi9PuwiGLfPI.woff2"); font-display: swap; font-style: normal; font-weight: 500; }
@font-face { font-family: "Roobert PRO Medium"; src: url("https://framerusercontent.com/assets/EpLn9agwfi64Kvr9InHDUx8Ufw.woff2"); font-display: swap; }
```

The full fallback stacks are in the front matter.

## Layout

Float a rounded white navigation bar beneath a dark announcement strip. Center the homepage hero inside a large rounded panel, with scattered connected interface snippets. Pricing turns into a regular grid of tall white cards and stacks them on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is absolute, 1px high, with 0px left and 0px right padding. The sampled nav is relative, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `90.3281px 90.3281px 90.3438px 90.3281px 90.3281px 90.3438px` with gap `32px 24px`; `90.3281px 90.3281px 90.3438px 90.3281px 90.3281px 90.3438px` with gap `32px 24px`; `470px` with gap `6px`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `1366px`, `800px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use dark priority actions on the homepage, light outlined alternatives and modest corner radii. The pricing system introduces a blue featured-plan outline and blue action; keep that route-specific emphasis distinct.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 12px / 12px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 48px, radius 8px, background rgb(255, 255, 255), and border 1px rgb(233, 234, 239). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Canvas diagrams, sticky-note colors, app icons and connecting curves explain collaboration. Preserve generous breathing room around each illustration.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `background-color 0.6s`, `transform 0.2s`, `opacity 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Human, clear and collaborative, with short outcome-led statements.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
