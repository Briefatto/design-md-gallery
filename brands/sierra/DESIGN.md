---
version: alpha
name: "Sierra"
description: "Sierra's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Sierra."
colors:
  primary: "rgb(0, 104, 56)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(246, 245, 243)"
  foreground: "rgb(48, 46, 45)"
  muted: "rgb(98, 94, 91)"
  border: "oklab(0.999994 0.0000455678 0.0000200868 / 0.2)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(52, 94, 178)"
typography:
  display:
    fontFamily: 'gtAmerica, "gtAmerica Fallback"'
    fontSize: 65px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'gtAmerica, "gtAmerica Fallback"'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.02em
  heading:
    fontFamily: 'gtAmerica, "gtAmerica Fallback"'
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.01em
  body:
    fontFamily: 'gtAmerica, "gtAmerica Fallback"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: 'gtAmerica, "gtAmerica Fallback"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 33554400px
  card: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 56px
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

# Sierra DESIGN.md

## Overview

A customer-experience platform pairs open GT America typography, deep green actions, warm neutral reading surfaces and large human-focused photography. Pale blue product demonstrations and quiet section transitions keep the interface approachable.

Built from [/](https://sierra.ai/) and [/platform](https://sierra.ai/platform), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 104, 56)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(246, 245, 243)` | Panels and cards |
| foreground | `rgb(48, 46, 45)` | Primary text |
| muted | `rgb(98, 94, 91)` | Supporting text |
| border | `oklab(0.999994 0.0000455678 0.0000200868 / 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(52, 94, 178)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | gtAmerica | 65px | 400 | 1.11 | -0.02em |
| display-mobile | gtAmerica | 32px | 400 | 1.13 | -0.02em |
| heading | gtAmerica | 26px | 400 | 1.15 | -0.01em |
| body | gtAmerica | 16px | 400 | 1.5 | 0em |
| action | gtAmerica | 14px | 400 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: gtAmerica; src: url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Regular-s.p.1zc5t_gvwny95.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: gtAmerica; src: url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Regular_Italic-s.p.0du5h8advea8t.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: gtAmerica; src: url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Medium-s.p.3u2zpkd3jquk2.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: gtAmerica; src: url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Medium_Italic-s.p.07wg2kjku1-c4.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: italic; }
@font-face{font-family:gtAmerica;src:url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Regular-s.p.1zc5t_gvwny95.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:gtAmerica;src:url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Regular_Italic-s.p.0du5h8advea8t.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:gtAmerica;src:url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Medium-s.p.3u2zpkd3jquk2.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:gtAmerica;src:url("https://sierra.ai/_next/static/immutable/media/GT_America_Standard_Medium_Italic-s.p.07wg2kjku1-c4.woff2")format("woff2");font-display:swap;font-weight:500;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Anchor the homepage introduction over a broad photographic media panel, then move into centered proof and feature sections. The Agent SDK route uses a left-aligned introduction above large demonstration panels and alternating explanatory blocks. Mobile stacks those roles and preserves a narrow reading column.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 56px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 700px high, with 0px left and 0px right padding. The sampled nav is sticky, 120px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `78px 78px 78px 78px 78px 78px 78px 78px 78px 78px 78px 78px` with gap `24px 16px`; `222.391px 222.406px 222.391px 222.406px 222.391px` with gap `normal`; `78px 78px 78px 78px 78px 78px 78px 78px 78px 78px 78px 78px` with gap `24px 16px`. Build them as a fluid grid. Sampled container maximum widths: `576px`, `484px`, `1160px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `33554400px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small green pill actions, quiet outlined companions, softly rounded media panels, pale blue conversation diagrams and restrained feature cards. Let photography and surface contrast provide depth rather than heavy decoration.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 16px / 16px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses human-centered photography and service-conversation demonstrations. Create original licensed photography and generic agent-workflow diagrams without copying people, conversations, screenshots, illustrations or customer marks.

**Motion.** Observed CSS transition declarations include `opacity 0.25s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.25s`, `background-color, color, outline-color 0.25s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to, opacity, box-shadow, transform, translate, scale, rotate, filter, -webkit-backdrop-filter, backdrop-filter, display, content-visibility, overlay, pointer-events 0.25s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm, helpful and practical, with concise service and capability descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
