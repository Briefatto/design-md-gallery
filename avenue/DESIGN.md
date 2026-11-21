---
version: alpha
name: "Avenue"
description: "Avenue's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Avenue."
colors:
  primary: "rgb(255, 225, 83)"
  background: "rgb(247, 247, 249)"
  surface: "rgb(247, 247, 249)"
  foreground: "rgb(17, 18, 28)"
  muted: "rgb(110, 110, 110)"
  border: "rgb(110, 110, 110)"
  on-primary: "rgb(0, 0, 0)"
  accent: "rgb(39, 92, 227)"
typography:
  display:
    fontFamily: 'Inter, "Inter Placeholder", sans-serif'
    fontSize: 57px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0em
  display-mobile:
    fontFamily: 'Inter, "Inter Placeholder", sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0em
  heading:
    fontFamily: '"Sequel Sans Headline Light", "Sequel Sans Headline Light Placeholder", sans-serif'
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  body:
    fontFamily: 'Inter, "Inter Placeholder", sans-serif'
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0em
  action:
    fontFamily: 'Inter, "Inter Placeholder", sans-serif'
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: 0em
rounded:
  control: 16px
  card: 16px
spacing:
  xs: 6px
  sm: 6px
  md: 16px
  lg: 21px
  xl: 32px
  section: 60px
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

# Avenue DESIGN.md

## Overview

An operations platform uses a pale lavender-gray ground, blue display text, yellow priority actions and a compact rounded navigation bar. Product demonstrations and occasional dark sections carry the denser operational detail.

Built from [/](https://avenue.app/) and [/pricing](https://avenue.app/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 225, 83)` | Priority actions and selected emphasis |
| background | `rgb(247, 247, 249)` | Page canvas |
| surface | `rgb(247, 247, 249)` | Panels and cards |
| foreground | `rgb(17, 18, 28)` | Primary text |
| muted | `rgb(110, 110, 110)` | Supporting text |
| border | `rgb(110, 110, 110)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |
| accent | `rgb(39, 92, 227)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Inter | 57px | 500 | 1.1 | 0em |
| display-mobile | Inter | 40px | 500 | 1.1 | 0em |
| heading | "Sequel Sans Headline Light" | 40px | 400 | 1.3 | 0em |
| body | Inter | 15px | 400 | 1.6 | 0em |
| action | Inter | 14px | 400 | 1.71 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Sequel Sans Headline Light"; src: url("https://framerusercontent.com/assets/Kqn4QGDQDbXMtme4X7tc9WfrGiM.woff2"); font-display: swap; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.cyrillic-ext-CFTLRB35.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.cyrillic-KKLZBALH.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.greek-ext-ULEBLIFV.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.greek-IRHSNFQB.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.latin-ext-VZDUGU3Q.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.latin-JLQMKCHE.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-Regular.vietnamese-QK7VSWXK.woff2"); font-display: swap; font-style: normal; font-weight: 400; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.cyrillic-ext-C7KWUKA7.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.cyrillic-JWV7SOZ6.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.greek-ext-FBKSFTSU.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.greek-EQ3PSENU.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.latin-ext-ULRSO3ZR.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.latin-RDYY2AG2.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://app.framerstatic.com/Inter-SemiBold.vietnamese-ESQNSEQ3.woff2"); font-display: swap; font-style: normal; font-weight: 600; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/NXxvFRoY5LDh3yCm7MEP2jqYk.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/5CcgcVyoWSqO1THBiISd6oCog.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/MF544SVCvk3yNpLIz3pwDXFZPKM.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/TNtxudDBkAm2RXdtU3rvTBwoM.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/fIabp4VN5z7iJ3lNOz9qfNeQHc.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/YSOgKh50dqzzsXffetgcarlLHcI.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/9iRSYClnXA0RMygyIn6yjjWXJw.woff2"); font-display: block; font-style: normal; font-weight: 100; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/MVhJhYeDWxeyqT939zMNyw9p8.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/WXQXYfAQJIi2pCJACAfWWXfIDqI.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/RJeJJARdrtNUtic58kOz7hIgBuE.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/4hBRAuM02i3fsxYDzyNvt5Az2so.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/fz1JbBffNGgK7BNUI1mmbFBlgA8.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/hgmI3sEShaw5UU738TAjDBQPH0.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/eIZyQwIlHYR0mnMSneEDMtqBPgw.woff2"); font-display: block; font-style: normal; font-weight: 200; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/BkDpl4ghaqvMi1btKFyG2tdbec.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/zAMK70AQRFSShJgUiaR5IiIhgzk.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/IETjvc5qzUaRoaruDpPSwCUM8.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/oLCoaT3ioA0fHdJnWR9W6k7NY.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/Sj0PCHQSBjFmEp6NBWg6FNaKc.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/v2q8JTTTs7McDMSEhnxAIBqd0.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/H4TfENUY1rh8R9UaSD6vngjJP3M.woff2"); font-display: swap; font-style: normal; font-weight: 300; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/5A3Ce6C9YYmCjpQx9M4inSaKU.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/Qx95Xyt0Ka3SGhinnbXIGpEIyP4.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/6mJuEAguuIuMog10gGvH5d3cl8.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/xYYWaj7wCU5zSQH0eXvSaS19wo.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/otTaNuNpVK4RbdlT7zDDdKvQBA.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/d3tHnaQIAeqiE5hGcRw4mmgWYU.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/DolVirEGb34pEXEp8t8FQBSK4.woff2"); font-display: swap; font-style: normal; font-weight: 500; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/DpPBYI0sL4fYLgAkX8KXOPVt7c.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/4RAEQdEOrcnDkhHiiCbJOw92Lk.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/1K3W8DizY3v4emK8Mb08YHxTbs.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/tUSCtfYVM1I1IchuyCwz9gDdQ.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/VgYFWiwsAC5OYxAycRXXvhze58.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/DXD0Q7LSl7HEvDzucnyLnGBHM.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/GIryZETIX4IFypco5pYZONKhJIo.woff2"); font-display: swap; font-style: normal; font-weight: 700; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/PONfPc6h4EPYwJliXQBmjVx7QxI.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/zsnJN7Z1wdzUvepJniD3rbvJIyU.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/UrzZBOy7RyJEWAZGduzOeHiHuY.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/996sR9SfSDuYELz8oHhDOcErkY.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/ftN1HpyPVJEoEb4q36SOrNdLXU.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/jN39PDxZWEwjG7Csryx3JN2r2Y.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/JAur4lGGSGRGyrFi59JSIKqVgU.woff2"); font-display: swap; font-style: normal; font-weight: 800; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/mkY5Sgyq51ik0AMrSBwhm9DJg.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/X5hj6qzcHUYv7h1390c8Rhm6550.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/gQhNpS3tN86g8RcVKYUUaKt2oMQ.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/cugnVhSraaRyANCaUtI5FV17wk.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/5HcVoGak8k5agFJSaKa4floXVu0.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/jn4BtSPLlS0NDp1KiFAtFKiiY0o.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/P2Bw01CtL0b9wqygO0sSVogWbo.woff2"); font-display: block; font-style: normal; font-weight: 900; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/YJsHMqeEm0oDHuxRTVCwg5eZuo.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/oJJMyJlDykMObEyb5VexHSxd24.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/IpeaX0WzLaonj68howNZg4SJJaY.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/KCj1bV3vDXY5OLHttTeRYcu9J8.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/biaVHhOprxbHaR3dIP7Z8cYurHg.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/BpOIEy4nYtcp1RwqOtwAgi2EiDE.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/gNa011yWpVpNFgUhhSlDX8nUiPQ.woff2"); font-display: block; font-style: italic; font-weight: 100; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/vpq17U0WM26sBGHgq9jnrUmUf8.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/bNYh7lNMEpOegeRYAtyGel1WqBE.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/FBzcXZYmdulcZC0z278U6o0cw.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/ua60IRqWK94xCrq0SC639Hbsdjg.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/Pd8gNPn2dSCh4FyjWFw9PJysoQ.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/zpiI5DA3vCb3G2sqEyq9xqogo.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/DtVQjTG8OGGKnwKYrMHRZVCyo.woff2"); font-display: block; font-style: italic; font-weight: 200; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/YYB6GZmCWnZq3RWZOghuZIOxQY.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/miJTzODdiyIr3tRo9KEoqXXk2PM.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/6ZMhcggRFfEfbf7lncCpaUbA.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/8sCN6PGUr4I8q5hC5twAXfcwqV0.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/aUYDUTztS7anQw5JuwCncXeLOBY.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/5mDAOkC5Wpzo7NkuE9oYfqlY2u4.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/yDiPvYxioBHsicnYxpPW35WQmx8.woff2"); font-display: swap; font-style: italic; font-weight: 300; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/CfMzU8w2e7tHgF4T4rATMPuWosA.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/867QObYax8ANsfX4TGEVU9YiCM.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/Oyn2ZbENFdnW7mt2Lzjk1h9Zb9k.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/cdAe8hgZ1cMyLu9g005pAW3xMo.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/DOfvtmE1UplCq161m6Hj8CSQYg.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/vFzuJY0c65av44uhEKB6vyjFMg.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/tKtBcDnBMevsEEJKdNGhhkLzYo.woff2"); font-display: swap; font-style: italic; font-weight: 400; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/khkJkwSL66WFg8SX6Wa726c.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/0E7IMbDzcGABpBwwqNEt60wU0w.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/NTJ0nQgIF0gcDelS14zQ9NR9Q.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/QrcNhgEPfRl0LS8qz5Ln8olanl8.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/JEXmejW8mXOYMtt0hyRg811kHac.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/ksvR4VsLksjpSwnC2fPgHRNMw.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/uy9s0iWuxiNnVt8EpTI3gzohpwo.woff2"); font-display: swap; font-style: italic; font-weight: 500; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/vxBnBhH8768IFAXAb4Qf6wQHKs.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/zSsEuoJdh8mcFVk976C05ZfQr8.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/b8ezwLrN7h2AUoPEENcsTMVJ0.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/mvNEIBLyHbscgHtwfsByjXUz3XY.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/6FI2EneKzM3qBy5foOZXey7coCA.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/qrVgiXNd6RuQjETYQiVQ9nqCk.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/NHHeAKJVP0ZWHk5YZnQQChIsBM.woff2"); font-display: swap; font-style: italic; font-weight: 600; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/H89BbHkbHDzlxZzxi8uPzTsp90.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/u6gJwDuwB143kpNK1T1MDKDWkMc.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/43sJ6MfOPh1LCJt46OvyDuSbA6o.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/wccHG0r4gBDAIRhfHiOlq6oEkqw.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/WZ367JPwf9bRW6LdTHN8rXgSjw.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/QxmhnWTzLtyjIiZcfaLIJ8EFBXU.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/2A4Xx7CngadFGlVV4xrO06OBHY.woff2"); font-display: swap; font-style: italic; font-weight: 700; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/if4nAQEfO1l3iBiurvlUSTaMA.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/GdJ7SQjcmkU1sz7lk5lMpKUlKY.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/sOA6LVskcCqlqggyjIZe0Zh39UQ.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/zUCSsMbWBcHOQoATrhsPVigkc.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/6eYp9yIAUvPZY7o0yfI4e2OP6g.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/aKoimhPBfs6C7Am2HTTVjGcpE.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/L9nHaKi7ULzGWchEehsfwttxOwM.woff2"); font-display: swap; font-style: italic; font-weight: 800; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/05KsVHGDmqXSBXM4yRZ65P8i0s.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+460-52F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/ky8ovPukK4dJ1Pxq74qGhOqCYI.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+301, U+400-45F, U+490-491, U+4B0-4B1, U+2116; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/vvNSqIj42qeQ2bvCRBIWKHscrc.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+1F00-1FFF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/3ZmXbBKToJifDV9gwcifVd1tEY.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+370-3FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/FNfhX3dt4ChuLJq2PwdlxHO7PU.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+100-24F, U+259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/g0c8vEViiXNlKAgI4Ymmk3Ig.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+0-FF, U+131, U+152-153, U+2BB-2BC, U+2C6, U+2DA, U+2DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD; }
@font-face { font-family: Inter; src: url("https://framerusercontent.com/assets/efTfQcBJ53kM2pB1hezSZ3RDUFs.woff2"); font-display: block; font-style: italic; font-weight: 900; unicode-range: U+102-103, U+110-111, U+128-129, U+168-169, U+1A0-1A1, U+1AF-1B0, U+1EA0-1EF9, U+20AB; }
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction and main action above an airy product demonstration and customer-proof band. Pricing uses two simple white offer panels followed by a soft gradient conversion panel; preserve clear reading order when adapting the mobile layout.

Spacing scale: xs 6px, sm 6px, md 16px, lg 21px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 256px high, with 60px left and 60px right padding.

 Sampled container maximum widths: `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.08) 0px 0.720139px 0.720139px 0.720139px, rgba(255, 255, 255, 0.2) 0px 0px 0.720139px 0.720139px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `16px`; the reusable card treatment uses `16px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use yellow pill-shaped homepage actions, quiet rounded cards, compact badges, pale grids and generous whitespace. The pricing route introduces violet contact actions, so treat those as route-specific accents rather than replacing every action color.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 62px, radius 98px, background rgb(255, 255, 255), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses dashboard demonstrations, workflow diagrams and softly colored technical panels. Use original generic operations interfaces and simple diagrams, excluding source screenshots and customer marks.

**Motion.** No non-zero transition was exposed in the sampled component styles. Static screenshots do not establish entrance choreography, hover behavior, or video timing. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, practical and operational, with concise benefit and next-step labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
