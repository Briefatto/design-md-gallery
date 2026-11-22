---
version: alpha
name: "Abridge"
description: "Abridge's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Abridge."
colors:
  primary: "rgb(234, 44, 0)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(247, 242, 237)"
  foreground: "rgb(20, 19, 18)"
  muted: "rgb(109, 100, 90)"
  border: "rgb(238, 229, 221)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'haffer, "haffer Fallback", Haffer, system-ui, -apple-system, sans-serif'
    fontSize: 58px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.01em
  display-mobile:
    fontFamily: 'haffer, "haffer Fallback", Haffer, system-ui, -apple-system, sans-serif'
    fontSize: 28.0001px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.02em
  heading:
    fontFamily: 'haffer, "haffer Fallback", Haffer, system-ui, -apple-system, sans-serif'
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  body:
    fontFamily: 'haffer, "haffer Fallback", Haffer, system-ui, -apple-system, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0em
  action:
    fontFamily: 'haffer, "haffer Fallback", Haffer, system-ui, -apple-system, sans-serif'
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 60px
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

# Abridge DESIGN.md

## Overview

A healthcare technology site combines large human-focused photography, spacious white editorial sections, warm neutral panels and bright orange priority actions. Haffer typography keeps the display and interface roles closely related.

Built from [/](https://abridge.com/) and [/platform/clinicians](https://abridge.com/platform/clinicians), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(234, 44, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(247, 242, 237)` | Panels and cards |
| foreground | `rgb(20, 19, 18)` | Primary text |
| muted | `rgb(109, 100, 90)` | Supporting text |
| border | `rgb(238, 229, 221)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | haffer | 58px | 400 | 0.93 | -0.01em |
| display-mobile | haffer | 28.0001px | 400 | 0.93 | -0.02em |
| heading | haffer | 48px | 400 | 1 | -0.02em |
| body | haffer | 16px | 400 | 1.38 | 0em |
| action | haffer | 18px | 500 | 1.22 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_Regular-s.p.2rr87ky_v0il9.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: normal; }
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_RegularItalic-s.p.34lfgm-vjhvjz.woff2") format("woff2"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_Medium-s.p.2ue_4a56cu4yq.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: normal; }
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_MediumItalic-s.p.41vjvspgeafmm.woff2") format("woff2"); font-display: swap; font-weight: 500; font-style: italic; }
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_SemiBold-s.p.0ii6tc11guwxq.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: normal; }
@font-face { font-family: haffer; src: url("https://www.abridge.com/_next/static/immutable/media/Haffer_SemiBoldItalic-s.p.2hmiqqdc--yaf.woff2") format("woff2"); font-display: swap; font-weight: 600; font-style: italic; }
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_Regular-s.p.2rr87ky_v0il9.woff2")format("woff2");font-display:swap;font-weight:400;font-style:normal}
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_RegularItalic-s.p.34lfgm-vjhvjz.woff2")format("woff2");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_Medium-s.p.2ue_4a56cu4yq.woff2")format("woff2");font-display:swap;font-weight:500;font-style:normal}
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_MediumItalic-s.p.41vjvspgeafmm.woff2")format("woff2");font-display:swap;font-weight:500;font-style:italic}
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_SemiBold-s.p.0ii6tc11guwxq.woff2")format("woff2");font-display:swap;font-weight:600;font-style:normal}
@font-face{font-family:haffer;src:url("https://www.abridge.com/_next/static/immutable/media/Haffer_SemiBoldItalic-s.p.2hmiqqdc--yaf.woff2")format("woff2");font-display:swap;font-weight:600;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use a full-width photographic or video homepage introduction with readable text anchored over a darkened lower area. The clinician route switches to a centered white introduction above alternating media and product panels. Mobile stacks those panels and preserves clear text contrast over imagery.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 94px high, with 0px left and 0px right padding. The sampled header is relative, 176.953px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px 82.5px` with gap `normal 30px`; `24px` with gap `normal`; `42px` with gap `normal`. Build them as a fluid grid. Sampled container maximum widths: `520px`, `500px`, `1670px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact rectangular orange actions, quiet outlined companions, fine section boundaries, modestly rounded media panels and softly elevated demonstration cards. Keep dense product examples distinct from the broad editorial reading sections.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 32px / 32px, and gap 4px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(109, 100, 90). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source relies on healthcare photography, clinician stories and product demonstrations. Use original licensed imagery and generic workflow diagrams without copying people, patient examples, screenshots, illustrations or organization marks.

**Motion.** Observed CSS transition declarations include `background-color, box-shadow 0.3s, 0.3s`, `background-color 0.15s`, `background-color, color, border-color, box-shadow, transform 0.15s, 0.15s, 0.15s, 0.15s, 0.15s`, `transform 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Calm, clear and human-oriented, with concise capability descriptions and straightforward actions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
