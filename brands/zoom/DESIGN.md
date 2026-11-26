---
version: alpha
name: "Zoom"
description: "Zoom's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Zoom."
colors:
  primary: "rgb(11, 92, 255)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(243, 248, 255)"
  foreground: "rgb(0, 5, 61)"
  muted: "rgb(105, 105, 105)"
  border: "rgb(209, 222, 242)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: 'Newsreader, Helvetica, Arial, "Noto Sans JP", "Noto Sans KR", "Noto Sans SC", "Noto Sans TC", "Noto Sans", sans-serif'
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Newsreader, Helvetica, Arial, "Noto Sans JP", "Noto Sans KR", "Noto Sans SC", "Noto Sans TC", "Noto Sans", sans-serif'
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0em
  heading:
    fontFamily: 'Newsreader, Helvetica, Arial, "Noto Sans JP", "Noto Sans KR", "Noto Sans SC", "Noto Sans TC", "Noto Sans", sans-serif'
    fontSize: 46px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: -0.03em
  body:
    fontFamily: 'Inter, Helvetica, "Noto Sans JP", "Noto Sans KR", "Noto Sans SC", "Noto Sans TC", "Noto Sans", Arial, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, Helvetica, "Noto Sans JP", "Noto Sans KR", "Noto Sans SC", "Noto Sans TC", "Noto Sans", Arial, sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: 0em
rounded:
  control: 12px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 30px
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

# Zoom DESIGN.md

## Overview

Newsreader serif statements and Inter interface text give the homepage a conversational editorial feel, framed by navy-to-lilac gradients and vivid blue actions.

Built from [/](https://zoom.com/) and [/pricing](https://zoom.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(11, 92, 255)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(243, 248, 255)` | Panels and cards |
| foreground | `rgb(0, 5, 61)` | Primary text |
| muted | `rgb(105, 105, 105)` | Supporting text |
| border | `rgb(209, 222, 242)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Newsreader | 54px | 500 | 1.12 | 0em |
| display-mobile | Newsreader | 34px | 500 | 1.1 | 0em |
| heading | Newsreader | 46px | 400 | 1.14 | -0.03em |
| body | Inter | 16px | 400 | 1.3 | 0em |
| action | Inter | 14px | 500 | 1.15 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face{font-display:swap;font-family:Noto Sans;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSans-Regular.4c8d6700.ttf") format("ttf")}
@font-face{font-display:swap;font-family:Noto Sans JP;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansJP-Regular.34b41de3.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans KR;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansKR-Regular.29445948.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans SC;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansSC-Regular.a2b93e6c.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans JP;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansTC-Regular.8d9cd5f2.otf") format("otf")}
@font-face{font-display:swap;font-family:Newsreader;font-style:normal;font-weight:200 800;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/newsreader/newsreader-vietnamese.68ef9a14.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-display:swap;font-family:Newsreader;font-style:normal;font-weight:200 800;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/newsreader/newsreader-latin-ext.cbca0011.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-display:swap;font-family:Newsreader;font-style:normal;font-weight:200 800;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/newsreader/newsreader-latin.01817351.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-cyrillic-ext.942b7145.woff2") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-cyrillic.a7f3e736.woff2") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-greek-ext.009e52d8.woff2") format("woff2");unicode-range:u+1f??}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-greek.b6a22966.woff2") format("woff2");unicode-range:u+0370-0377,u+037a-037f,u+0384-038a,u+038c,u+038e-03a1,u+03a3-03ff}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-vietnamese.07df696d.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-latin-ext.8bc9dee3.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-latin.dd8a4575.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-cyrillic-ext.974fe69b.woff2") format("woff2");unicode-range:u+0460-052f,u+1c80-1c8a,u+20b4,u+2de0-2dff,u+a640-a69f,u+fe2e-fe2f}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-cyrillic.925b918f.woff2") format("woff2");unicode-range:u+0301,u+0400-045f,u+0490-0491,u+04b0-04b1,u+2116}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-greek-ext.dbc57e88.woff2") format("woff2");unicode-range:u+1f??}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-greek.380e26a8.woff2") format("woff2");unicode-range:u+0370-0377,u+037a-037f,u+0384-038a,u+038c,u+038e-03a1,u+03a3-03ff}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-vietnamese.3199b2e5.woff2") format("woff2");unicode-range:u+0102-0103,u+0110-0111,u+0128-0129,u+0168-0169,u+01a0-01a1,u+01af-01b0,u+0300-0301,u+0303-0304,u+0308-0309,u+0323,u+0329,u+1ea0-1ef9,u+20ab}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-latin-ext.7d263a25.woff2") format("woff2");unicode-range:u+0100-02ba,u+02bd-02c5,u+02c7-02cc,u+02ce-02d7,u+02dd-02ff,u+0304,u+0308,u+0329,u+1d00-1dbf,u+1e00-1e9f,u+1ef2-1eff,u+2020,u+20a0-20ab,u+20ad-20c0,u+2113,u+2c60-2c7f,u+a720-a7ff}
@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100 900;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/inter/inter-italic-latin.124b693f.woff2") format("woff2");unicode-range:u+00??,u+0131,u+0152-0153,u+02bb-02bc,u+02c6,u+02da,u+02dc,u+0304,u+0308,u+0329,u+2000-206f,u+20ac,u+2122,u+2191,u+2193,u+2212,u+2215,u+feff,u+fffd}
@font-face{font-display:swap;font-family:Noto Sans;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSans-Regular.ttf") format("ttf")}
@font-face{font-display:swap;font-family:Noto Sans JP;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansJP-Regular.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans KR;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansKR-Regular.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans SC;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansSC-Regular.otf") format("otf")}
@font-face{font-display:swap;font-family:Noto Sans JP;font-style:normal;font-weight:400;src:url("https://st1.zoom.us/homepage/20261118-1151/primary/dist/assets/fonts/noto-sans/NotoSansTC-Regular.otf") format("otf")}
```

The full fallback stacks are in the front matter.

## Layout

Use a compact navigation, centered statement and horizontal product-media carousel, followed by broad alternating feature sections. Pricing shifts to a persistent product sidebar and a dense plan comparison; the mobile capture retains horizontally arranged plan cards.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 30px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is fixed, 78px high, with 0px left and 0px right padding. The sampled nav is static, 36.0938px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `519.422px 173.141px 173.141px 173.141px 173.156px` with gap `37px`. Build them as a fluid grid. Sampled container maximum widths: `100%`, `830px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Blue priority actions, pale blue alternatives, modest rounded corners and inset product tiles establish the system. Pricing uses a blue featured-plan banner, billing toggle and compact feature rows, with Almaden Sans rather than homepage Inter.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 46px, horizontal padding 20px / 20px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 24px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(35, 35, 51). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Video-call portraits, meeting and productivity interfaces and illustrated product cards explain the suite. Keep people and product imagery grouped into clear rectangular frames.

**Motion.** Observed CSS transition declarations include `all 0.3s`, `background 0.15s`, `all 0.5s`, `all 0.25s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Welcoming and practical, centered on connection and clear product choices.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
