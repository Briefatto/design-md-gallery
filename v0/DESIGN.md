---
version: alpha
name: "v0"
description: "v0's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with v0."
colors:
  primary: "rgb(23, 23, 23)"
  background: "rgb(250, 250, 250)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(23, 23, 23)"
  muted: "rgb(77, 77, 77)"
  border: "rgb(228, 228, 231)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'GeistSans, "GeistSans Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'GeistSans, "GeistSans Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.04em
  heading:
    fontFamily: 'GeistSans, "GeistSans Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.04em
  body:
    fontFamily: 'Inter, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, -apple-system, "system-ui", "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
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
  section: 72px
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

# v0 DESIGN.md

## Overview

An AI app-building interface uses a restrained neutral palette, compact sans-serif typography, fine outlines and a large centered prompt composer. A public template gallery adds visual variety beneath the quiet creation interface.

Built from [/](https://v0.app/) and [/pricing](https://v0.app/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(23, 23, 23)` | Priority actions and selected emphasis |
| background | `rgb(250, 250, 250)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(23, 23, 23)` | Primary text |
| muted | `rgb(77, 77, 77)` | Supporting text |
| border | `rgb(228, 228, 231)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | GeistSans | 32px | 600 | 1.25 | -0.04em |
| display-mobile | GeistSans | 24px | 600 | 1.33 | -0.04em |
| heading | GeistSans | 24px | 600 | 1.33 | -0.04em |
| body | Inter | 14px | 500 | 1.43 | 0em |
| action | Inter | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: GeistSans; src: url("https://v0.app/chat-static/_next/static/immutable/media/Geist_Variable-s.p.2v-cf9syxr5ni.woff2") format("woff2"); font-display: swap; font-weight: 100 900; }
@font-face{font-family:GeistSans;src:url("https://v0.app/chat-static/_next/static/immutable/media/Geist_Variable-s.p.2v-cf9syxr5ni.woff2")format("woff2");font-display:swap;font-weight:100 900}
```

The full fallback stacks are in the front matter.

For body and action, the captured first-choice font was unavailable on the public source pages and no resolvable loading reference was observed. The generic preview starts those roles at -apple-system, an available fallback from the captured CSS stack; other roles retain their observed families. The guide and tokens retain the original declared stacks and measured metrics. Preview font substitution is an adaptation.

## Layout

Center the introduction, prompt field and suggestion chips above a multi-column template gallery with category controls. Pricing switches to a large left-aligned title and lightly divided plan columns, with a pale featured-plan surface. Mobile stacks the gallery and pricing plans while keeping the composer prominent.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 72px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 0px left and 0px right padding. The sampled nav is static, 32px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `26px` with gap `normal`; `389.328px 389.328px 389.344px` with gap `24px`; `388.656px 388.672px 388.656px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`, `1448px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.02) 0px 1px 1px 0px, rgba(0, 0, 0, 0.04) 0px 4px 8px -4px, rgba(0, 0, 0, 0.06) 0px 16px 24px -8px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use rounded outlined prompt fields, small pill suggestions, compact model and voice controls, quiet template cards and economical dark priority actions. Keep borders and subtle surface changes as the main grouping devices.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 20px / 20px, and gap 6px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source displays community template thumbnails and interface examples. Create original generic application specimens and diagrams without copying templates, screenshots, avatars or source marks.

**Motion.** Observed CSS transition declarations include `box-shadow 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.15s`, `all 0.15s`, `border-color, background, color 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Concise, practical and creation-oriented, with clear prompt and next-step labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
