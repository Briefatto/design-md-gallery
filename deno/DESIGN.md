---
version: alpha
name: "Deno"
description: "Deno's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Deno."
colors:
  primary: "rgb(112, 255, 175)"
  background: "rgb(11, 13, 17)"
  surface: "rgb(18, 20, 23)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(176, 178, 182)"
  border: "rgb(37, 39, 43)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(112, 255, 175)"
typography:
  display:
    fontFamily: 'Inter, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif'
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  display-mobile:
    fontFamily: 'Inter, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif'
    fontSize: 39.25px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  heading:
    fontFamily: 'Inter, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif'
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  body:
    fontFamily: 'Inter, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 0px
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

# Deno DESIGN.md

## Overview

A developer runtime site contrasts a dark, atmospheric homepage hero with a light deployment-pricing page. Bright mint announcements and technical monospace details frame a bold sans-serif product introduction.

Built from [/](https://deno.com/) and [/pricing](https://deno.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(112, 255, 175)` | Priority actions and selected emphasis |
| background | `rgb(11, 13, 17)` | Page canvas |
| surface | `rgb(18, 20, 23)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(176, 178, 182)` | Supporting text |
| border | `rgb(37, 39, 43)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(112, 255, 175)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Inter | 72px | 700 | 1.1 | -0.025em |
| display-mobile | Inter | 39.25px | 700 | 1.1 | -0.025em |
| heading | Inter | 44px | 700 | 1.1 | -0.025em |
| body | Inter | 14px | 400 | 1.43 | 0em |
| action | Menlo | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: Inter; font-style: normal; font-weight: 400; font-display: swap; src: url("https://deno.com/fonts/inter/Inter-Regular.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2"); }
@font-face { font-family: Inter; font-style: italic; font-weight: 400; font-display: swap; src: url("https://deno.com/fonts/inter/Inter-Italic.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2"); }
@font-face { font-family: Inter; font-style: normal; font-weight: 700; font-display: swap; src: url("https://deno.com/fonts/inter/Inter-SemiBold.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2"); }
@font-face { font-family: Inter; font-style: italic; font-weight: 700; font-display: swap; src: url("https://deno.com/fonts/inter/Inter-SemiBoldItalic.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2"); }
@font-face {
  font-family: "Inter";
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://deno.com/fonts/inter/Inter-Regular.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2");
}
@font-face {
  font-family: "Inter";
  font-style: italic;
  font-weight: 400;
  font-display: swap;
  src: url("https://deno.com/fonts/inter/Inter-Italic.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2");
}
@font-face {
  font-family: "Inter";
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url("https://deno.com/fonts/inter/Inter-SemiBold.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2");
}
@font-face {
  font-family: "Inter";
  font-style: italic;
  font-weight: 700;
  font-display: swap;
  src: url("https://deno.com/fonts/inter/Inter-SemiBoldItalic.woff2?__frsh_c=2c7be834343e725c25fa21f2d98d4350fa3b3f96") format("woff2");
}
```

The full fallback stacks are in the front matter.

## Layout

Place the desktop hero copy beside a vertical technical capability display, with installation content below. On mobile, the visual sits above the text and actions. Pricing centers a large serif headline over a spacious comparison table; preserve that route-specific typography rather than applying it across the homepage.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 96px high, with 0px left and 0px right padding. The sampled nav is static, 48px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `1440px` with gap `normal`; `1440px` with gap `normal`; `624px 416px` with gap `128px`. Build them as a fluid grid. 

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact announcement bars, rounded dark actions, small release badges, code-oriented panels and fine technical rules. Pricing uses light blue accents, understated plan columns and restrained comparison rows.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 29px, horizontal padding 16px / 16px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 34px, radius 8px, background rgba(0, 0, 0, 0), and border 1px rgb(134, 135, 137). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses subtle dark color fields, technical text animation and runtime illustrations. Use original abstract technical diagrams and geometric texture without copying the mascot, screenshots or partner marks.

**Motion.** Observed CSS transition declarations include `all 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `all 0.15s`, `all 0.5s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct and developer-focused, with practical capability descriptions and clear installation steps.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
