---
version: alpha
name: "Mintlify"
description: "Mintlify's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Mintlify."
colors:
  primary: "lab(2.42579 -0.165291 -0.470081)"
  background: "lab(100 0 0)"
  surface: "rgb(250, 248, 245)"
  foreground: "rgb(18, 23, 21)"
  muted: "lab(2.42579 -0.165291 -0.470081 / 0.6)"
  border: "lab(2.42579 -0.165291 -0.470081 / 0.07)"
  on-primary: "lab(100 0 0)"
  accent: "rgb(12, 140, 94)"
typography:
  display:
    fontFamily: 'arizonaFlare, "arizonaFlare Fallback", serif'
    fontSize: 50px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.04em
  display-mobile:
    fontFamily: 'arizonaFlare, "arizonaFlare Fallback", serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  heading:
    fontFamily: 'inter, "inter Fallback"'
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.02em
  body:
    fontFamily: 'inter, "inter Fallback"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'inter, "inter Fallback"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 4px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 80px
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

# Mintlify DESIGN.md

## Overview

A documentation platform combines expressive serif-like display lettering with a precise sans-serif interface, airy white space and selective green accents. Fine luminous lines and pale product surfaces provide the visual atmosphere.

Built from [/](https://mintlify.com/) and [/pricing](https://mintlify.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `lab(2.42579 -0.165291 -0.470081)` | Priority actions and selected emphasis |
| background | `lab(100 0 0)` | Page canvas |
| surface | `rgb(250, 248, 245)` | Panels and cards |
| foreground | `rgb(18, 23, 21)` | Primary text |
| muted | `lab(2.42579 -0.165291 -0.470081 / 0.6)` | Supporting text |
| border | `lab(2.42579 -0.165291 -0.470081 / 0.07)` | Quiet separators and outlines |
| on-primary | `lab(100 0 0)` | Text on the primary action |
| accent | `rgb(12, 140, 94)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | arizonaFlare | 50px | 400 | 1.04 | -0.04em |
| display-mobile | arizonaFlare | 40px | 400 | 1.1 | -0.02em |
| heading | inter | 36px | 500 | 1.11 | -0.02em |
| body | inter | 16px | 400 | 1.5 | 0em |
| action | inter | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: inter; src: url("https://www.mintlify.com/_next/static/media/InterVariable-s.p.494bb210.ttf") format("truetype"); font-display: swap; }
@font-face { font-family: arizonaFlare; src: url("https://www.mintlify.com/_next/static/media/ABCArizonaFlare_Regular-s.p.fb4e034f.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face{font-family:inter;src:url("https://www.mintlify.com/_next/static/media/InterVariable-s.p.494bb210.ttf")format("truetype");font-display:swap}
@font-face{font-family:arizonaFlare;src:url("https://www.mintlify.com/_next/static/media/ABCArizonaFlare_Regular-s.p.fb4e034f.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column hero with a short left-aligned title and actions beside a documentation demonstration. Sweep thin geometric lines through the surrounding whitespace. Pricing centers its heading above a four-column plan row that becomes stacked cards on mobile.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 80px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 65px high, with 0px left and 0px right padding. The sampled header is static, 120px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px` with gap `normal 16px`; `30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px 30px` with gap `0px 16px`; `29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px 29.9062px` with gap `normal 16px`. Build them as a fluid grid. Sampled container maximum widths: `1088px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Favor near-square dark actions, tiny status badges, understated billing selectors, warm neutral plan cards and fine grid separators. The documentation demonstration includes a sidebar, tab strip and compact article panels.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 34px, horizontal padding 14px / 14px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The site uses delicate green line fields and documentation screenshots. Recreate the line concept and document structure with original geometry and generic content; omit source screenshots, logos and customer marks.

**Motion.** Observed CSS transition declarations include `background-color 0.3s`, `color, background-color, border-color, outline-color, -webkit-text-decoration-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.1s`, `transform, color, background-color, border-color 0.1s`, `color, background-color, border-color 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm, helpful and direct, with concise documentation and setup terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
