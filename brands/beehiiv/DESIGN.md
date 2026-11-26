---
version: alpha
name: "beehiiv"
description: "beehiiv's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with beehiiv."
colors:
  primary: "rgb(47, 57, 186)"
  background: "rgb(6, 4, 25)"
  surface: "rgb(6, 4, 25)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(147, 147, 169)"
  border: "rgba(255, 255, 255, 0.12)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(240, 146, 221)"
typography:
  display:
    fontFamily: 'ClashGroteskFont, "ClashGroteskFont Fallback", sans-serif'
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'ClashGroteskFont, "ClashGroteskFont Fallback", sans-serif'
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: 0em
  heading:
    fontFamily: 'ClashGroteskFont, "ClashGroteskFont Fallback", sans-serif'
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0em
  body:
    fontFamily: 'SatoshiFont, "SatoshiFont Fallback", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'SatoshiFont, "SatoshiFont Fallback", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 6px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 64px
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

# beehiiv DESIGN.md

## Overview

A newsletter platform uses a near-black violet canvas, tightly stacked uppercase Clash Grotesk headings, crisp Satoshi body text, and luminous pink and blue accents. The mood is entrepreneurial and energetic, with practical interface previews balancing the bold opening.

Built from [/](https://www.beehiiv.com/) and [/pricing](https://www.beehiiv.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(47, 57, 186)` | Priority actions and selected emphasis |
| background | `rgb(6, 4, 25)` | Page canvas |
| surface | `rgb(6, 4, 25)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(147, 147, 169)` | Supporting text |
| border | `rgba(255, 255, 255, 0.12)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(240, 146, 221)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | ClashGroteskFont | 60px | 700 | 1 | 0em |
| display-mobile | ClashGroteskFont | 42px | 700 | 1.05 | 0em |
| heading | ClashGroteskFont | 48px | 700 | 1 | 0em |
| body | SatoshiFont | 14px | 500 | 1.43 | 0em |
| action | SatoshiFont | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `uppercase` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-family:SatoshiFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/Satoshi_Light-s.p.40f53fa-bgouz.woff2")format("woff2");font-display:swap;font-weight:300;font-style:normal}
@font-face{font-family:SatoshiFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/Satoshi_Regular-s.p.2oultpqxb_gh9.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:SatoshiFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/Satoshi_Medium-s.p.2gbh8zsgu5xby.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:SatoshiFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/Satoshi_Bold-s.p.19z5sx2nusz2v.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:SatoshiFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/Satoshi_Black-s.p.03d7m3bcbsl0m.woff2")format("woff2");font-display:swap;font-weight:900;font-style:normal}
@font-face{font-family:ClashGroteskFont;src:url("https://www.beehiiv.com/_next/static/immutable/media/ClashGrotesk_Bold-s.p.425v0mrw2cfn5.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
```

The full fallback stacks are in the front matter.

## Layout

Use a slim ruled navigation and split desktop hero with left-aligned copy and layered product panels. Mobile stacks the hero. Alternate spacious product chapters and testimonial rows; pricing centers the introduction above a subscriber slider and white plan cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is sticky, 77px high, with 128px left and 128px right padding. The sampled nav is static, 36px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `576px 576px` with gap `32px`; `227.547px 227.562px 227.562px` with gap `12px`; `227.547px 227.562px 227.562px` with gap `12px`. Build them as a fluid grid. Sampled container maximum widths: `569px`, `750px`, `512px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `6px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact blue filled actions, thin outlined alternatives, small utility badges, and softly rounded white pricing cards. Pricing adds a pink recommended-tier outline and clear dark price typography. Keep dark-page borders low-contrast and reserve bright accents for selected states.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 46px, horizontal padding 24px / 24px, and gap 10px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 28px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original generic publication and analytics mockups layered over violet glows, with simple line icons for content types.

**Motion.** Observed CSS transition declarations include `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `transform 0.5s`, `transform 0.125s`, `transform 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Energetic, entrepreneurial, and direct about outcomes.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
