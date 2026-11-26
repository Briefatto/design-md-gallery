---
version: alpha
name: "Annnimate"
description: "Annnimate's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Annnimate."
colors:
  primary: "rgb(251, 70, 13)"
  background: "rgb(20, 19, 20)"
  surface: "rgb(20, 19, 20)"
  foreground: "rgb(238, 238, 238)"
  muted: "oklab(0.949113 0.0000431836 0.0000190735 / 0.7)"
  border: "oklab(0.949113 0.0000431836 0.0000190735 / 0.15)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: 'aktivGrotesk, "aktivGrotesk Fallback", geistSans, "geistSans Fallback", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", sans-serif'
    fontSize: 59.298px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.035em
  display-mobile:
    fontFamily: 'aktivGrotesk, "aktivGrotesk Fallback", geistSans, "geistSans Fallback", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", sans-serif'
    fontSize: 28.4408px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.035em
  heading:
    fontFamily: 'aktivGrotesk, "aktivGrotesk Fallback", geistSans, "geistSans Fallback", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", sans-serif'
    fontSize: 37.9102px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.04em
  body:
    fontFamily: 'aktivGrotesk, "aktivGrotesk Fallback", geistSans, "geistSans Fallback", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: 0em
  action:
    fontFamily: 'aktivGrotesk, "aktivGrotesk Fallback", geistSans, "geistSans Fallback", -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: 0em
rounded:
  control: 0px
  card: 0px
spacing:
  xs: 1px
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

# Annnimate DESIGN.md

## Overview

A motion-component library uses charcoal and pale gray section changes, compact grotesk typography, square orange actions and a large animated gallery of interface examples.

Built from [/](https://annnimate.com/) and [/pricing](https://annnimate.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(251, 70, 13)` | Priority actions and selected emphasis |
| background | `rgb(20, 19, 20)` | Page canvas |
| surface | `rgb(20, 19, 20)` | Panels and cards |
| foreground | `rgb(238, 238, 238)` | Primary text |
| muted | `oklab(0.949113 0.0000431836 0.0000190735 / 0.7)` | Supporting text |
| border | `oklab(0.949113 0.0000431836 0.0000190735 / 0.15)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | aktivGrotesk | 59.298px | 500 | 1 | -0.035em |
| display-mobile | aktivGrotesk | 28.4408px | 500 | 1 | -0.035em |
| heading | aktivGrotesk | 37.9102px | 500 | 1.13 | -0.04em |
| body | aktivGrotesk | 14px | 400 | 1.45 | 0em |
| action | aktivGrotesk | 14px | 400 | 1.45 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: geistSans; src: url("https://annnimate.com/_next/static/immutable/media/GeistVariable-s.1plo5k2nsh1rt.woff2") format("woff2"); font-display: swap; font-weight: 100 900; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Light-s.241hdiyvu0-ww.woff2") format("woff2"); font-display: swap; font-weight: 300; font-style: normal; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Regular-s.00xshevomojyj.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Italic-s.3ccbmoue5g73i.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Medium-s.0ema6zs-uz0tm.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_MediumItalic-s.36_nafc1itez-.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: italic; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Bold-s.0de_fosrffxgg.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: normal; }
@font-face { font-family: aktivGrotesk; src: url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_BoldItalic-s.26_4_n0cqc3cw.woff2") format("woff2"); font-display: swap; font-weight: 700; font-style: italic; }
@font-face{font-family:geistSans;src:url("https://annnimate.com/_next/static/immutable/media/GeistVariable-s.1plo5k2nsh1rt.woff2")format("woff2");font-display:swap;font-weight:100 900}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Light-s.241hdiyvu0-ww.woff2")format("woff2");font-display:swap;font-weight:300;font-style:normal}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Regular-s.00xshevomojyj.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Italic-s.3ccbmoue5g73i.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Medium-s.0ema6zs-uz0tm.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_MediumItalic-s.36_nafc1itez-.woff2")format("woff2");font-display:swap;font-weight:500;font-style:italic}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_Bold-s.0de_fosrffxgg.woff2")format("woff2");font-display:swap;font-weight:700;font-style:normal}
@font-face{font-family:aktivGrotesk;src:url("https://annnimate.com/_next/static/immutable/media/AktivGroteskCorp_BoldItalic-s.26_4_n0cqc3cw.woff2")format("woff2");font-display:swap;font-weight:700;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Center a concise homepage introduction above a wide, layered demonstration gallery. Pricing switches to a light ground and asymmetrical plan columns, with a black featured panel and unboxed secondary offers. On mobile, maintain readable plan access rather than treating the captured horizontal overflow as a desired pattern.

Spacing scale: xs 1px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 72px high, with 0px left and 0px right padding. The sampled nav is relative, 72px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `100px 100px 100px 100px 100px 100px 100px 100px 100px 100px 100px 100px` with gap `16px`; `92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px` with gap `48px 24px`; `92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px 92.6562px` with gap `48px 24px`. Build them as a fluid grid. Sampled container maximum widths: `772.193px`, `403.969px`, `448.854px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `0px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use square filled orange actions, quiet gray companions, small plan badges, thin vertical dividers, compact billing toggles and restrained wireframe product symbols. Keep the plan hierarchy clear through surface and type contrast.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 28px, horizontal padding 10px / 10px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 38px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgba(238, 238, 238, 0.1). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses animated UI examples, image thumbnails and fine wireframe geometry. Build original neutral component demonstrations and simple diagrams, excluding source artwork and customer marks.

**Motion.** Observed CSS transition declarations include `color, background-color 0.8s, 0.8s`, `transform, padding-top 0.4s, 0.3s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.15s`, `color, background-color, border-color, outline-color, text-decoration-color, fill, stroke, --tw-gradient-from, --tw-gradient-via, --tw-gradient-to 0.4s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, creative and implementation-oriented, with short action labels and clear component descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
