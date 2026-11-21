---
version: alpha
name: "Asana"
description: "Asana's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Asana."
colors:
  primary: "rgb(13, 13, 13)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(250, 250, 250)"
  foreground: "rgb(13, 14, 16)"
  muted: "rgba(62, 62, 62, 0.8)"
  border: "rgb(213, 220, 224)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"TWK Lausanne", "Helvetica Neue", Helvetica, sans-serif'
    fontSize: 102px
    fontWeight: 300
    lineHeight: 0.9
    letterSpacing: -0.025em
  display-mobile:
    fontFamily: '"TWK Lausanne", "Helvetica Neue", Helvetica, sans-serif'
    fontSize: 48px
    fontWeight: 300
    lineHeight: 0.9
    letterSpacing: -0.02em
  heading:
    fontFamily: '"TWK Lausanne", "Helvetica Neue", Helvetica, sans-serif'
    fontSize: 30px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  body:
    fontFamily: '"TWK Lausanne", "Helvetica Neue", Helvetica, sans-serif'
    fontSize: 20px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: 0.02em
  action:
    fontFamily: '"TWK Lausanne", "Helvetica Neue", Helvetica, sans-serif'
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 100px
  card: 20px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 56px
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

# Asana DESIGN.md

## Overview

A work-management site uses very large open sans-serif headlines, black priority actions, white surfaces and fine gray structure. Small pastel workflow markers add selective color within an otherwise restrained interface.

Built from [/](https://asana.com/) and [/pricing](https://asana.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(13, 13, 13)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(250, 250, 250)` | Panels and cards |
| foreground | `rgb(13, 14, 16)` | Primary text |
| muted | `rgba(62, 62, 62, 0.8)` | Supporting text |
| border | `rgb(213, 220, 224)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "TWK Lausanne" | 102px | 300 | 0.9 | -0.025em |
| display-mobile | "TWK Lausanne" | 48px | 300 | 0.9 | -0.02em |
| heading | "TWK Lausanne" | 30px | 300 | 1.1 | -0.02em |
| body | "TWK Lausanne" | 20px | 300 | 1.5 | 0.02em |
| action | "TWK Lausanne" | 16px | 500 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-250.otf") format("truetype"); font-weight: 250; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-300.otf") format("truetype"); font-weight: 300; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-350.otf") format("truetype"); font-weight: 350; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-400.otf") format("truetype"); font-weight: 400; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-450.otf") format("truetype"); font-weight: 450; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-500.otf") format("truetype"); font-weight: 500; font-style: normal; font-display: block; }
@font-face { font-family: "TWK Lausanne"; src: url("https://asana.com/fonts/lausanne/TWKLausanne-550.otf") format("truetype"); font-weight: 550; font-style: normal; font-display: block; }
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage title above social sign-in and email-entry controls, then introduce workflow diagrams and spacious proof sections. Pricing uses a wide row of clearly divided plan panels that become a vertical sequence on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 56px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 68px high, with 0px left and 0px right padding. The sampled nav is relative, 68px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `[full-width-start] 64px [content-start] 1312px [content-end] 64px [full-width-end]` with gap `normal`; `[full-width-start] 64px [content-start] 1312px [content-end] 64px [full-width-end]` with gap `normal`; `32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px 32.1562px` with gap `normal 32px`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `900px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgb(13, 13, 13) 0px 0px 0px 1px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `100px`; the reusable card treatment uses `20px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact black pill actions, pale neutral companions, fine outlined fields, restrained plan panels and small feature checks. The pricing panels have subtly clipped upper corners; a portable radius token simplifies that visual treatment rather than defining an exact clip path.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 50px, horizontal padding 32px / 32px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(100, 111, 121). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses workflow diagrams, task panels and small colorful illustrations. Create original generic project diagrams and neutral work-management specimens without copying screenshots, characters, logos or customer marks.

**Motion.** Observed CSS transition declarations include `transform, opacity 0.15s, 0.15s`, `background-color, color 0.15s, 0.15s`, `none 0.3s`, `color, border 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, practical and collaborative, with concise actions and straightforward feature explanations.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
