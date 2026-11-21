---
version: alpha
name: "Firebase"
description: "Firebase's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Firebase."
colors:
  primary: "rgb(255, 145, 0)"
  background: "rgb(30, 30, 30)"
  surface: "rgb(30, 30, 30)"
  foreground: "rgb(255, 255, 255)"
  muted: "rgb(255, 255, 255)"
  border: "rgb(50, 50, 50)"
  on-primary: "rgb(0, 0, 0)"
typography:
  display:
    fontFamily: '"Google Sans", sans-serif'
    fontSize: 75px
    fontWeight: 700
    lineHeight: 1.33
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Google Sans", sans-serif'
    fontSize: 45px
    fontWeight: 700
    lineHeight: 1.44
    letterSpacing: 0em
  heading:
    fontFamily: '"Google Sans", "Noto Sans", "Noto Sans JP", "Noto Sans KR", "Noto Naskh Arabic", "Noto Sans Thai", "Noto Sans Hebrew", "Noto Sans Bengali", sans-serif'
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Google Sans", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Google Sans", "Noto Sans", "Noto Sans JP", "Noto Sans KR", "Noto Naskh Arabic", "Noto Sans Thai", "Noto Sans Hebrew", "Noto Sans Bengali", sans-serif'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 4px
  card: 20px
spacing:
  xs: 5px
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

# Firebase DESIGN.md

## Overview

A developer platform pairs dark charcoal introductory chapters with warm orange action signals and bold Google Sans headlines. White detail sections and blue plan headers introduce a separate, practical comparison context.

Built from [/](https://firebase.google.com/) and [/pricing](https://firebase.google.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 145, 0)` | Priority actions and selected emphasis |
| background | `rgb(30, 30, 30)` | Page canvas |
| surface | `rgb(30, 30, 30)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `rgb(255, 255, 255)` | Supporting text |
| border | `rgb(50, 50, 50)` | Quiet separators and outlines |
| on-primary | `rgb(0, 0, 0)` | Text on the primary action |

Use white text on the charcoal introduction and orange for its key action or outline. Pricing switches to white reading surfaces with dark text and blue/charcoal plan bands; keep those pairings separate from the dark sample. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Google Sans" | 75px | 700 | 1.33 | 0em |
| display-mobile | "Google Sans" | 45px | 700 | 1.44 | 0em |
| heading | "Google Sans" | 20px | 500 | 1.2 | 0em |
| body | "Google Sans" | 16px | 400 | 1.5 | 0em |
| action | "Google Sans" | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCdG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCYW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCY20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCXm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCdW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCYG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCam0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCUm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCc20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCa20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCem0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCeG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCaW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCaG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCH20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCZ20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCZW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCf20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcW0AsJd9XQ&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCdG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCYW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCY20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCXm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCdW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCYG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCam0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCUm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCc20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCa20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCem0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCeG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCaW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCaG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbG0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCH20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCZ20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCbW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCZW0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCfm0AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCf20AsJd9XV1F&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/l/font?kit=4UbKrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RFD48TE63OOYKtrwEIMtpj9g6jpk_QovMyISCcW0AsJd9XQ&skey=c30756b8cf584a60&v=v76") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 600;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjcUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0600-06FF, U+0750-077F, U+0870-0891, U+0897-08E1, U+08E3-08FF, U+200C-200E, U+2010-2011, U+204F, U+2E41, U+FB50-FDFF, U+FE70-FE74, U+FE76-FEFC, U+102E0-102FB, U+10E60-10E7E, U+10EC2-10EC7, U+10EC9-10EEE, U+10EF0-10EFF, U+1EE00-1EE03, U+1EE05-1EE1F, U+1EE21-1EE22, U+1EE24, U+1EE27, U+1EE29-1EE32, U+1EE34-1EE37, U+1EE39, U+1EE3B, U+1EE42, U+1EE47, U+1EE49, U+1EE4B, U+1EE4D-1EE4F, U+1EE51-1EE52, U+1EE54, U+1EE57, U+1EE59, U+1EE5B, U+1EE5D, U+1EE5F, U+1EE61-1EE62, U+1EE64, U+1EE67-1EE6A, U+1EE6C-1EE72, U+1EE74-1EE77, U+1EE79-1EE7C, U+1EE7E, U+1EE80-1EE89, U+1EE8B-1EE9B, U+1EEA1-1EEA3, U+1EEA5-1EEA9, U+1EEAB-1EEBB, U+1EEF0-1EEF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiIUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0308, U+0530-058F, U+2010, U+2024, U+25CC, U+FB13-FB17;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0980-09FE, U+1CD0, U+1CD2, U+1CD5-1CD6, U+1CD8, U+1CE1, U+1CEA, U+1CED, U+1CF2, U+1CF5-1CF7, U+200C-200D, U+20B9, U+25CC, U+A8F1, U+11DF0-11DF1;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPh0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02C7, U+02D8-02D9, U+02DB, U+0307, U+1400-167F, U+18B0-18F5, U+25CC, U+11AB0-11ABF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C8A, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0900-097F, U+1CD0-1CF4, U+1CF7-1CF9, U+200C-200D, U+20A8, U+20B9, U+20F0, U+25CC, U+A830-A839, U+A8E0-A8FF, U+11B00-11B0A;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiMUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+030E, U+1200-1399, U+2D80-2DDE, U+AB01-AB2E, U+1E7E0-1E7E6, U+1E7E8-1E7EB, U+1E7ED-1E7EE, U+1E7F0-1E7FE;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0589, U+10A0-10FF, U+1C90-1CBA, U+1CBD-1CBF, U+205A, U+2D00-2D2F, U+2E31;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1F00-1FFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPikUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A80-0AFF, U+200C-200D, U+20B9, U+25CC, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPhEUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0A01-0A76, U+200C-200D, U+20B9, U+25CC, U+262C, U+A830-A839;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjAUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307-0308, U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPigUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C80-0CF3, U+1CD0, U+1CD2-1CD3, U+1CDA, U+1CF2, U+1CF4, U+200C-200D, U+20B9, U+25CC, U+A830-A835;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjkUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+1780-17FF, U+19E0-19FF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjsUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0E81-0EDF, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPioUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0307, U+0323, U+0951-0952, U+0964-0965, U+0B83, U+0D00-0D7F, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC, U+A830-A832;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPisUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B01-0B77, U+1CDA, U+1CF2, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi8UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0D81-0DF4, U+1CF2, U+200C-200D, U+25CC, U+111E1-111F4;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPlwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0001-000C, U+000E-001F, U+007F-009F, U+20DD-20E0, U+20E2-20E4, U+2150-218F, U+2190, U+2192, U+2194-2199, U+21AF, U+21E6-21F0, U+21F3, U+2218-2219, U+2299, U+22C4-22C6, U+2300-243F, U+2440-244A, U+2460-24FF, U+25A0-27BF, U+2800-28FF, U+2921-2922, U+2981, U+29BF, U+29EB, U+2B00-2BFF, U+4DC0-4DFF, U+FFF9-FFFB, U+10140-1018E, U+10190-1019C, U+101A0, U+101D0-101FD, U+102E0-102FB, U+10E60-10E7E, U+1D2C0-1D2D3, U+1D2E0-1D37F, U+1F000-1F0FF, U+1F100-1F1AE, U+1F1E6-1F1FF, U+1F30D-1F30F, U+1F315, U+1F31C, U+1F31E, U+1F320-1F32C, U+1F336, U+1F378, U+1F37D, U+1F382, U+1F393-1F39F, U+1F3A7-1F3A8, U+1F3AC-1F3AF, U+1F3C2, U+1F3C4-1F3C6, U+1F3CA-1F3CE, U+1F3D4-1F3E0, U+1F3ED, U+1F3F1-1F3F3, U+1F3F5-1F3F7, U+1F408, U+1F415, U+1F41F, U+1F426, U+1F43F, U+1F441-1F442, U+1F444, U+1F446-1F449, U+1F44C-1F44E, U+1F453, U+1F46A, U+1F47D, U+1F4A3, U+1F4B0, U+1F4B3, U+1F4B9, U+1F4BB, U+1F4BF, U+1F4C8-1F4CB, U+1F4D6, U+1F4DA, U+1F4DF, U+1F4E3-1F4E6, U+1F4EA-1F4ED, U+1F4F7, U+1F4F9-1F4FB, U+1F4FD-1F4FE, U+1F503, U+1F507-1F50B, U+1F50D, U+1F512-1F513, U+1F53E-1F54A, U+1F54F-1F5FA, U+1F610, U+1F650-1F67F, U+1F687, U+1F68D, U+1F691, U+1F694, U+1F698, U+1F6AD, U+1F6B2, U+1F6B9-1F6BA, U+1F6BC, U+1F6C6-1F6CF, U+1F6D3-1F6D7, U+1F6E0-1F6EA, U+1F6F0-1F6F3, U+1F6F7-1F6FC, U+1F700-1F80B, U+1F810-1F847, U+1F850-1F859, U+1F860-1F887, U+1F890-1F8AD, U+1F8B0-1F8BB, U+1F8C0-1F8C1, U+1F8D0-1F8D8, U+1F900-1F90B, U+1F93B, U+1F946, U+1F984, U+1F996, U+1F9E9, U+1FA00-1FA6F, U+1FA70-1FA7C, U+1FA80-1FAC6, U+1FAC8, U+1FACC-1FADD, U+1FADF-1FAEB, U+1FAEF-1FAFA, U+1FB00-1FBFF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiQUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0964-0965, U+0B82-0BFA, U+200C-200D, U+20B9, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPi4UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0951-0952, U+0964-0965, U+0B83, U+0C00-0C7F, U+1CD5-1CD6, U+1CD8, U+1CDA, U+1CF2, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPiYUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+02D7, U+0303, U+0331, U+0E01-0E5B, U+200C-200D, U+25CC;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPj0UvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjwUvbQoi-Entw.woff2") format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C4, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: swap;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Use a compact developer navigation above a centered, oversized introductory message. The pricing route begins with a dark title band, then opens into a wide comparison table on desktop and stacked plan groupings on mobile.

Spacing scale: xs 5px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is absolute, 48px high, with 0px left and 0px right padding. The sampled nav is static, 272px high, with 0px left and 0px right padding.

 Sampled container maximum widths: `100%`, `1000px`, `1280px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(0, 0, 0, 0.15) 0px 4px 12px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `20px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use clear action controls, modest-radius information cards, readable tabular comparisons, and practical navigation.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 36px, radius 0px, background rgb(241, 243, 244), and border 0px rgba(0, 0, 0, 0.6). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original technical diagrams, code snippets, and simple functional icons without copying product marks or illustrations.

**Motion.** Observed CSS transition declarations include `background-color, border, box-shadow 0.2s, 0.2s, 0.2s`, `color 0.2s`, `background, box-shadow, color 0.2s, 0.2s, 0.2s`, `background, color 0.2s, 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Helpful and specific; explain capabilities and pricing clearly.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

