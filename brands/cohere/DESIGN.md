---
version: alpha
name: "Cohere"
description: "Cohere's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Cohere."
colors:
  primary: "rgb(0, 0, 0)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(240, 238, 233)"
  foreground: "rgb(33, 33, 33)"
  muted: "rgb(147, 147, 159)"
  border: "rgb(229, 231, 235)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(6, 44, 34)"
typography:
  display:
    fontFamily: 'CohereText, "Space Grotesk", Inter, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: 'CohereText, "Space Grotesk", Inter, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  heading:
    fontFamily: 'CohereText, "Space Grotesk", Inter, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  body:
    fontFamily: '"Unica77 Cohere Web", Inter, Arial, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0em
  action:
    fontFamily: '"Unica77 Cohere Web", Inter, Arial, ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 4px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
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

# Cohere DESIGN.md

## Overview

An enterprise AI site combines unusually open display lettering with compact practical interface type, white and warm-gray surfaces, and deep forest-green product sections. Large media and textural imagery provide most of the visual variety.

Built from [/](https://cohere.com/) and [/command](https://cohere.com/command), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 0, 0)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(240, 238, 233)` | Panels and cards |
| foreground | `rgb(33, 33, 33)` | Primary text |
| muted | `rgb(147, 147, 159)` | Supporting text |
| border | `rgb(229, 231, 235)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(6, 44, 34)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | CohereText | 96px | 400 | 1 | -0.02em |
| display-mobile | CohereText | 60px | 400 | 1 | -0.02em |
| heading | CohereText | 32px | 400 | 1 | -0.02em |
| body | "Unica77 Cohere Web" | 14px | 400 | 1.4 | 0em |
| action | "Unica77 Cohere Web" | 14px | 500 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: CohereText; src: url("https://cohere.com/_next/static/immutable/media/CohereText-Regular.2hnqq9npo38r1.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/CohereText-Regular.1336anz7ld1a-.woff") format("woff"); font-weight: 400; font-style: normal; font-display: swap; }
@font-face { font-family: CohereText; src: url("https://cohere.com/_next/static/immutable/media/CohereVariable.14rd3idw_4066.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/CohereVariable.30x2vo9-09iqm.woff") format("woff"); font-weight: 500 525; font-style: normal; font-display: swap; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Thin.0zauujyc9klux.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Thin.1vzfyjt31y07x.woff") format("woff"); font-display: swap; font-weight: 100; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-ThinItalic.2z2vm2w-sc7sa.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-ThinItalic.2xm5rmgbm-m-h.woff") format("woff"); font-display: swap; font-weight: 100; font-style: italic; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Light.2pvjt0p0kya26.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Light.3tdanau4bp9yg.woff") format("woff"); font-display: swap; font-weight: 300; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-LightItalic.2lcix7mv4jhvi.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-LightItalic.1pr3rabxdr3_9.woff") format("woff"); font-display: swap; font-weight: 300; font-style: italic; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Regular.08nli527722ku.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Regular.0s7p5tqg488vh.woff") format("woff"); font-display: swap; font-weight: 400; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Italic.05iyzcnc64eis.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Italic.23h51ctzlsrmj.woff") format("woff"); font-display: swap; font-weight: 400; font-style: italic; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Medium.2d_f6bxov-n_b.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Medium.0779qubp1wt-l.woff") format("woff"); font-display: swap; font-weight: 500; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-MediumItalic.2a9yhz7r1c3sp.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-MediumItalic.2m9xxzietnwvo.woff") format("woff"); font-display: swap; font-weight: 500; font-style: italic; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Bold.0ifnon1g78mmk.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Bold.1j4rc78-gwmn-.woff") format("woff"); font-display: swap; font-weight: 700; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-BoldItalic.310xu8zec83lw.woff2") format("woff2"), url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-BoldItalic.13aee300oqm1o.woff") format("woff"); font-display: swap; font-weight: 700; font-style: italic; }
@font-face { font-family: CohereText; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Regular.2w5c73mttyaq7.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: CohereText; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Medium.1zxxsez8l1wma.otf") format("opentype"); font-weight: 500 525; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Thin.34jrckrwjosgr.otf") format("opentype"); font-weight: 100; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Light.3159m1qdpc1cs.otf") format("opentype"); font-weight: 300; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Regular.2w5c73mttyaq7.otf") format("opentype"); font-weight: 400; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Medium.1zxxsez8l1wma.otf") format("opentype"); font-weight: 500; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face { font-family: "Unica77 Cohere Web"; src: url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Bold.0kweqe_824x4b.otf") format("opentype"); font-weight: 700; font-style: normal; font-display: swap; unicode-range: U+600-6FF, U+750-77F, U+8A0-8FF, U+FB50-FDFF, U+FE70-FEFF; }
@font-face{font-family:CohereText;src:url("https://cohere.com/_next/static/immutable/media/CohereText-Regular.2hnqq9npo38r1.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/CohereText-Regular.1336anz7ld1a-.woff")format("woff");font-weight:400;font-style:normal;font-display:swap}
@font-face{font-family:CohereText;src:url("https://cohere.com/_next/static/immutable/media/CohereVariable.14rd3idw_4066.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/CohereVariable.30x2vo9-09iqm.woff")format("woff");font-weight:500 525;font-style:normal;font-display:swap}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Thin.0zauujyc9klux.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Thin.1vzfyjt31y07x.woff")format("woff");font-display:swap;font-weight:100}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-ThinItalic.2z2vm2w-sc7sa.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-ThinItalic.2xm5rmgbm-m-h.woff")format("woff");font-display:swap;font-weight:100;font-style:italic}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Light.2pvjt0p0kya26.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Light.3tdanau4bp9yg.woff")format("woff");font-display:swap;font-weight:300}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-LightItalic.2lcix7mv4jhvi.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-LightItalic.1pr3rabxdr3_9.woff")format("woff");font-display:swap;font-weight:300;font-style:italic}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Regular.08nli527722ku.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Regular.0s7p5tqg488vh.woff")format("woff");font-display:swap;font-weight:400}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Italic.05iyzcnc64eis.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Italic.23h51ctzlsrmj.woff")format("woff");font-display:swap;font-weight:400;font-style:italic}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Medium.2d_f6bxov-n_b.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Medium.0779qubp1wt-l.woff")format("woff");font-display:swap;font-weight:500}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-MediumItalic.2a9yhz7r1c3sp.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-MediumItalic.2m9xxzietnwvo.woff")format("woff");font-display:swap;font-weight:500;font-style:italic}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Bold.0ifnon1g78mmk.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-Bold.1j4rc78-gwmn-.woff")format("woff");font-display:swap;font-weight:700}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-BoldItalic.310xu8zec83lw.woff2")format("woff2"),url("https://cohere.com/_next/static/immutable/media/Unica77CohereWeb-BoldItalic.13aee300oqm1o.woff")format("woff");font-display:swap;font-weight:700;font-style:italic}
@font-face{font-family:CohereText;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Regular.2w5c73mttyaq7.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:CohereText;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Medium.1zxxsez8l1wma.otf")format("opentype");font-weight:500 525;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Thin.34jrckrwjosgr.otf")format("opentype");font-weight:100;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Light.3159m1qdpc1cs.otf")format("opentype");font-weight:300;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Regular.2w5c73mttyaq7.otf")format("opentype");font-weight:400;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Medium.1zxxsez8l1wma.otf")format("opentype");font-weight:500;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
@font-face{font-family:Unica77 Cohere Web;src:url("https://cohere.com/_next/static/immutable/media/Unica77CohereAra-Bold.0kweqe_824x4b.otf")format("opentype");font-weight:700;font-style:normal;font-display:swap;unicode-range:U+6??,U+750-77F,U+8A0-8FF,U+FB50-FDFF,U+FE70-FEFF}
```

The full fallback stacks are in the front matter.

## Layout

Center a broad homepage introduction above an expansive product demonstration and spacious feature sections. The Command route switches to a dark green introduction with a prominent media panel and modular feature blocks. Mobile stacks those sections while retaining large text and a generous reading measure.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 36px, section 80px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is fixed, 60px high, with 0px left and 0px right padding. The sampled nav is fixed, 60px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `437.328px 437.328px 437.344px` with gap `24px`; `437.328px 437.328px 437.344px` with gap `24px`; `437.328px 437.328px 437.344px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `617px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use restrained pill-shaped priority actions, quiet text links, rounded media panels, softly separated feature cards and small technical labels. Keep white-on-forest and dark-on-white treatments consistent within each section.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 42px, horizontal padding 12px / 12px, and gap 12px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses organic textures, product demonstrations and colorful model imagery. Create original textural compositions and generic enterprise workflow diagrams without copying screenshots, artwork, logos or customer marks.

**Motion.** Observed CSS transition declarations include `transform 0.3s`, `opacity 0.15s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.2s`, `all 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Measured, clear and enterprise-oriented, with precise capability and deployment descriptions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
