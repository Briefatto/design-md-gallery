---
version: alpha
name: "GitHub"
description: "GitHub's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with GitHub."
colors:
  primary: "rgb(8, 135, 43)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(242, 245, 243)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgb(88, 99, 91)"
  border: "rgb(228, 235, 230)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Mona Sans", MonaSansFallback, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 56px
    fontWeight: 440
    lineHeight: 1.1
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Mona Sans", MonaSansFallback, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 36px
    fontWeight: 440
    lineHeight: 1.2
    letterSpacing: 0em
  heading:
    fontFamily: '"Mona Sans", MonaSansFallback, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  body:
    fontFamily: '"Mona Sans", MonaSansFallback, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.015em
  action:
    fontFamily: '"Mona Sans", MonaSansFallback, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.017em
rounded:
  control: 6px
  card: 8px
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
---

# GitHub DESIGN.md

## Overview

A developer platform mixes a high-impact product introduction with highly structured navigation and practical supporting content.

Built from [/](https://github.com/) and [/pricing](https://github.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(8, 135, 43)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(242, 245, 243)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgb(88, 99, 91)` | Supporting text |
| border | `rgb(228, 235, 230)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Mona Sans" | 56px | 440 | 1.1 | 0em |
| display-mobile | "Mona Sans" | 36px | 440 | 1.2 | 0em |
| heading | "Mona Sans" | 20px | 400 | 1.3 | 0em |
| body | "Mona Sans" | 16px | 400 | 1.5 | 0.015em |
| action | "Mona Sans" | 14px | 400 | 1.5 | 0.017em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face { font-family: "Mona Sans"; src: url("https://github.githubassets.com/assets/MonaSansVF-wdth-wght-opsz-7a868ff47c93bd97.woff2") format("woff2-variations"); font-weight: 200 900; font-display: swap; font-feature-settings: "liga" 0; }
```

The full fallback stacks are in the front matter.

## Layout

Use a broad content container, a clear hero hierarchy, grouped calls to action, and modular feature sections; pricing uses comparable columns. A fine grid and small pixel-like accents structure the opening feature area; use original geometry to suggest that technical rhythm.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 68px high, with 0px left and 0px right padding. The sampled nav is static, 28px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `182px` with gap `12px`; `303.484px` with gap `normal`; `182px` with gap `12px`. Build them as a fluid grid. Sampled container maximum widths: `924px`, `562.621px`, `600px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Build compact rounded actions, bordered feature panels, structured pricing cards, and carefully grouped navigation links.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 43px, horizontal padding 20px / 20px, and gap 12px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 41px, radius 8px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Original code examples, small line icons, and abstract technical diagrams can support the story without copying product screens.

**Motion.** Observed CSS transition declarations include `background-color, border-color 0.2s, 0.2s`, `background-color 0.2s`, `color, background-color, box-shadow 0.08s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful and developer-literate; pair a clear benefit with a concrete next action.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

