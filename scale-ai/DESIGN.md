---
version: alpha
name: "Scale AI"
description: "Scale AI's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Scale AI."
colors:
  primary: "rgb(25, 58, 41)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(234, 234, 234)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(87, 87, 87)"
  border: "rgb(199, 199, 199)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'aeonik, "aeonik Fallback", -apple-system, Arial, sans-serif'
    fontSize: 116px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'aeonik, "aeonik Fallback", -apple-system, Arial, sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -0.01em
  heading:
    fontFamily: 'aeonik, "aeonik Fallback", -apple-system, Arial, sans-serif'
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.07
    letterSpacing: -0.01em
  body:
    fontFamily: 'aeonik, "aeonik Fallback", -apple-system, Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  action:
    fontFamily: 'aeonik, "aeonik Fallback", ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0em
rounded:
  control: 8px
  card: 16px
spacing:
  xs: 8px
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

# Scale AI DESIGN.md

## Overview

An enterprise AI site uses restrained Aeonik typography, white and black section changes, deep green priority actions and large photographic media. Small technical labels and fine boundaries give the expansive layout a precise feel.

Built from [/](https://scale.com/) and [/enterprise](https://scale.com/enterprise), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(25, 58, 41)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(234, 234, 234)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(87, 87, 87)` | Supporting text |
| border | `rgb(199, 199, 199)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | aeonik | 116px | 400 | 1 | -0.01em |
| display-mobile | aeonik | 32px | 400 | 1.05 | -0.01em |
| heading | aeonik | 28px | 400 | 1.07 | -0.01em |
| body | aeonik | 16px | 400 | 1.3 | -0.01em |
| action | aeonik | 14px | 400 | 1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: aeonik; src: url("https://scale.com/_next/static/immutable/media/AeonikPro_Regular-s.p.00jgyx3zdprqc.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face{font-family:aeonik;src:url("https://scale.com/_next/static/immutable/media/AeonikPro_Regular-s.p.00jgyx3zdprqc.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Frame the homepage introduction within a large cinematic media panel below a compact header. The enterprise route centers its title within a loose network of industry image tiles, then moves into broad alternating feature sections. Mobile stacks or crops media while keeping the main reading column clear.

Spacing scale: xs 8px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 88px high, with 0px left and 0px right padding. The sampled nav is relative, 40px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px` with gap `8px`; `1280px 96px` with gap `16px`; `108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px 108.656px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `1392px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact dark green or neutral actions, modest corner radii, fine section rules, small technical labels and broadly rounded image tiles. Let media and section contrast supply depth rather than adding heavy shadows to every panel.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses industry photography, technical media and loosely connected image tiles. Use original licensed industry imagery and generic system diagrams without copying source photos, videos, screenshots or customer marks.

**Motion.** Observed CSS transition declarations include `scrollbar-color 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.3s`, `all 0.5s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Precise, technical and enterprise-oriented, with clear capability and deployment descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
