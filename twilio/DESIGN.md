---
version: alpha
name: "Twilio"
description: "Twilio's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Twilio."
colors:
  primary: "rgb(24, 102, 238)"
  background: "rgb(0, 13, 37)"
  surface: "rgb(13, 18, 43)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(202, 205, 216)"
  border: "rgb(221, 224, 230)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(239, 34, 58)"
typography:
  display:
    fontFamily: '"Whitney SSm", helvetica, arial, sans-serif'
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.18
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: '"Whitney SSm", helvetica, arial, sans-serif'
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.18
    letterSpacing: -0.03em
  heading:
    fontFamily: '"Whitney SSm", helvetica, arial, sans-serif'
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.02em
  body:
    fontFamily: '"Whitney SSm", helvetica, arial, sans-serif'
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
    letterSpacing: 0em
  action:
    fontFamily: '"Whitney SSm", helvetica, arial, sans-serif'
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.75
    letterSpacing: 0em
rounded:
  control: 50px
  card: 0px
spacing:
  xs: 5px
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

# Twilio DESIGN.md

## Overview

A communications platform uses a deep navy foundation, sturdy rounded sans-serif headings, vivid blue actions and selective red signals. The bright navigation bar contrasts with dark marketing sections and pale pricing content.

Built from [/](https://twilio.com/) and [/pricing](https://twilio.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(24, 102, 238)` | Priority actions and selected emphasis |
| background | `rgb(0, 13, 37)` | Page canvas |
| surface | `rgb(13, 18, 43)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(202, 205, 216)` | Supporting text |
| border | `rgb(221, 224, 230)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(239, 34, 58)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Whitney SSm" | 56px | 700 | 1.18 | -0.03em |
| display-mobile | "Whitney SSm" | 34px | 700 | 1.18 | -0.03em |
| heading | "Whitney SSm" | 40px | 700 | 1.3 | -0.02em |
| body | "Whitney SSm" | 18px | 400 | 1.56 | 0em |
| action | "Whitney SSm" | 12px | 500 | 1.75 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Whitney SSm"; font-style: normal; font-weight: 300; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/fb8f4bd387fe17e372e0.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/225c43e15a2cf82b0ba3.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: italic; font-weight: 300; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/6e83af88a1232bcc2c28.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/9f0d44653a9a38942cd6.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: normal; font-weight: 400; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/a20a647d19af27011c7c.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/baa1fb0a9acc37d8398c.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: italic; font-weight: 400; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/d014274f22c83861153d.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/957854b7b3ed7dd92d10.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: normal; font-weight: 500; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/e408c138892b0f08a23d.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/476694f8f4b125f1739a.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: italic; font-weight: 500; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/95d647818722fea84b04.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/59f0a6164869bb619acf.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: normal; font-weight: 600; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/220e5b59f8588716f4d8.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/6260018dfa67c718436c.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: italic; font-weight: 600; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/7a3152fe74a79983fb95.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/ebbecace6167b8dc12a2.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: normal; font-weight: 700; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/ee7a891efcbc6ef61942.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/7bc3eac03c524eec69aa.woff") format("woff"); }
@font-face { font-family: "Whitney SSm"; font-style: italic; font-weight: 700; src: url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/1718c0d39436f219238f.woff2") format("woff2"), url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/c1ed7551272b423fefca.woff") format("woff"); }
@font-face{font-family:Whitney SSm;font-style:normal;font-weight:300;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/fb8f4bd387fe17e372e0.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/225c43e15a2cf82b0ba3.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:italic;font-weight:300;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/6e83af88a1232bcc2c28.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/9f0d44653a9a38942cd6.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:normal;font-weight:400;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/a20a647d19af27011c7c.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/baa1fb0a9acc37d8398c.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:italic;font-weight:400;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/d014274f22c83861153d.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/957854b7b3ed7dd92d10.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:normal;font-weight:500;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/e408c138892b0f08a23d.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/476694f8f4b125f1739a.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:italic;font-weight:500;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/95d647818722fea84b04.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/59f0a6164869bb619acf.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:normal;font-weight:600;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/220e5b59f8588716f4d8.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/6260018dfa67c718436c.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:italic;font-weight:600;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/7a3152fe74a79983fb95.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/ebbecace6167b8dc12a2.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:normal;font-weight:700;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/ee7a891efcbc6ef61942.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/7bc3eac03c524eec69aa.woff") format("woff")}
@font-face{font-family:Whitney SSm;font-style:italic;font-weight:700;src:url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/1718c0d39436f219238f.woff2") format("woff2"),url("https://www.twilio.com/etc.clientlibs/twilio-foundation/clientlibs/clientlib-site/resources/c1ed7551272b423fefca.woff") format("woff")}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column desktop hero with copy and actions beside a media panel. Follow with grouped capability blocks and editorial imagery. Pricing centers its introduction above a section-jump row and repeated product-rate groups; mobile stacks the columns and rate descriptions.

Spacing scale: xs 5px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 112px high, with 0px left and 0px right padding. The sampled nav is static, 80px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `107.938px 111px 123.891px 117.438px 94.2344px` with gap `normal`; `107.938px 111px 123.891px 117.438px 94.2344px` with gap `normal`; `16px 41.9844px 10px` with gap `8px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `50px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small blue pill actions, underlined supporting links, generous rounded media panels, compact proof points and clear pricing category headings. Keep red status and category accents selective rather than applying them to every action.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The site uses abstract dimensional conversation scenes, product panels and customer photography. Use original geometric scenes and generic communication diagrams, excluding logos, source photos and screenshots.

**Motion.** Observed CSS transition declarations include `transform, -webkit-transform 0.3s, 0.3s`, `opacity 0.3s`, `border-color, color 0.3s, 0.3s`, `background-color, color, border-color, box-shadow, color, border-color 0.3s, 0.3s, 0.3s, 0.3s, 0.3s, 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear and business-oriented, with practical channel, capability and usage descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
