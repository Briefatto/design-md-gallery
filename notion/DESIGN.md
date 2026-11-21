---
version: alpha
name: "Notion"
description: "Notion's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Notion."
colors:
  primary: "rgb(0, 117, 222)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(249, 249, 248)"
  foreground: "rgb(0, 0, 0)"
  muted: "rgba(0, 0, 0, 0.59)"
  border: "rgba(0, 0, 0, 0.1)"
  on-primary: "rgb(255, 255, 255)"
  accent: "rgb(255, 177, 16)"
typography:
  display:
    fontFamily: 'NotionInter, Inter, -apple-system, "system-ui", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 96px
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: -0.048em
  display-mobile:
    fontFamily: 'NotionInter, Inter, -apple-system, "system-ui", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1.14
    letterSpacing: -0.036em
  heading:
    fontFamily: 'NotionInter, Inter, -apple-system, "system-ui", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.27
    letterSpacing: -0.011em
  body:
    fontFamily: 'NotionInter, Inter, -apple-system, "system-ui", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
  action:
    fontFamily: 'NotionInter, Inter, -apple-system, "system-ui", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 8px
  card: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
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

# Notion DESIGN.md

## Overview

A workspace platform combines very large, heavy sans-serif headlines, bright blue priority actions, pale neutral product surfaces and playful line illustrations. Selective colored word highlights and small icon signals add warmth to a disciplined interface.

Built from [/](https://notion.com/) and [/pricing](https://notion.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 117, 222)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(249, 249, 248)` | Panels and cards |
| foreground | `rgb(0, 0, 0)` | Primary text |
| muted | `rgba(0, 0, 0, 0.59)` | Supporting text |
| border | `rgba(0, 0, 0, 0.1)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |
| accent | `rgb(255, 177, 16)` | Selective emphasis in headings, graphics, and small signals |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | NotionInter | 96px | 600 | 1.04 | -0.048em |
| display-mobile | NotionInter | 42px | 600 | 1.14 | -0.036em |
| heading | NotionInter | 22px | 700 | 1.27 | -0.011em |
| body | NotionInter | 14px | 500 | 1.43 | 0em |
| action | NotionInter | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: NotionInter; src: url("https://www.notion.com/front-static/fonts/NotionInter-Regular.woff2") format("woff2"), url("https://www.notion.com/front-static/fonts/NotionInter-Regular.woff") format("woff"); font-style: normal; font-weight: 400; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/front-static/fonts/NotionInter-Medium.woff2") format("woff2"), url("https://www.notion.com/front-static/fonts/NotionInter-Medium.woff") format("woff"); font-style: normal; font-weight: 500; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/front-static/fonts/NotionInter-SemiBold.woff2") format("woff2"), url("https://www.notion.com/front-static/fonts/NotionInter-SemiBold.woff") format("woff"); font-style: normal; font-weight: 600; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/front-static/fonts/NotionInter-Bold.woff2") format("woff2"), url("https://www.notion.com/front-static/fonts/NotionInter-Bold.woff") format("woff"); font-style: normal; font-weight: 700; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Italic.2vb9zej_iju_y.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Italic.12i6afi9b9hxe.woff") format("woff"); font-style: italic; font-weight: 400; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic.2g12c_dh0rad3.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic.2rynykzgn0xv8.woff") format("woff"); font-style: italic; font-weight: 500; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic.275kiy_6teqt3.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic.3i3ekylt2dzo6.woff") format("woff"); font-style: italic; font-weight: 600; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic.3u147tw2czjpe.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic.08sixp5xcn5t3.woff") format("woff"); font-style: italic; font-weight: 700; font-display: swap; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Regular-i18n.00ioyd906d58c.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Regular-i18n.41t_njf6omqug.woff") format("woff"); font-style: normal; font-weight: 400; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Italic-i18n.13ttwp5t-mbd7.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Italic-i18n.0-k84asq6g8u0.woff") format("woff"); font-style: italic; font-weight: 400; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Medium-i18n.2323dzohbvk8n.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Medium-i18n.2tkojwvm96-0f.woff") format("woff"); font-style: normal; font-weight: 500; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-i18n.3c5zkal8qq863.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-i18n.3jlqi1wpho-1p.woff") format("woff"); font-style: italic; font-weight: 500; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-i18n.0v6npia89qig-.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-i18n.1pdr821pyw3m5.woff") format("woff"); font-style: normal; font-weight: 600; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-i18n.19mbftanf92cw.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-i18n.2c9ecteqq2dz6.woff") format("woff"); font-style: italic; font-weight: 600; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Bold-i18n.007-piztngqyv.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Bold-i18n.1kf1-bcapvitl.woff") format("woff"); font-style: normal; font-weight: 700; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-i18n.428p1llnba081.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-i18n.2tgc92j7lw1ya.woff") format("woff"); font-style: italic; font-weight: 700; font-display: swap; unicode-range: U+300-36F, U+C0-FF, U+100-17F, U+1EA0-1EF9; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Regular-math.1a6t35xyuxi20.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Regular-math.1hzylpes2g_bm.woff") format("woff"); font-style: normal; font-weight: 400; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Italic-math.22b8zyjp-fmrg.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Italic-math.0boesj398nbmg.woff") format("woff"); font-style: italic; font-weight: 400; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Medium-math.3h5a0h0lxvtg-.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Medium-math.1dgmj_gsijb1f.woff") format("woff"); font-style: normal; font-weight: 500; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-math.0q1zkx9qhcer0.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-math.2le-vmg0w-w1c.woff") format("woff"); font-style: italic; font-weight: 500; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-math.0a6v2_nx97nws.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-math.0m755201v_cvt.woff") format("woff"); font-style: normal; font-weight: 600; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-math.0-zip_tvxb4gj.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-math.22oeklwa0ha-y.woff") format("woff"); font-style: italic; font-weight: 600; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-Bold-math.14rbjwnmavhus.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-Bold-math.2z3rh5kxmzpvv.woff") format("woff"); font-style: normal; font-weight: 700; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face { font-family: NotionInter; src: url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-math.2k5m59rf5np05.woff2") format("woff2"), url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-math.2qjvrl3b8y4s2.woff") format("woff"); font-style: italic; font-weight: 700; font-display: swap; unicode-range: U+370-3FF, U+2070-2073, U+2075-209F, U+2200-2211, U+2213-22FF; }
@font-face{font-family:NotionInter;src:url("https://www.notion.com/front-static/fonts/NotionInter-Regular.woff2")format("woff2"),url("https://www.notion.com/front-static/fonts/NotionInter-Regular.woff")format("woff");font-style:normal;font-weight:400;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/front-static/fonts/NotionInter-Medium.woff2")format("woff2"),url("https://www.notion.com/front-static/fonts/NotionInter-Medium.woff")format("woff");font-style:normal;font-weight:500;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/front-static/fonts/NotionInter-SemiBold.woff2")format("woff2"),url("https://www.notion.com/front-static/fonts/NotionInter-SemiBold.woff")format("woff");font-style:normal;font-weight:600;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/front-static/fonts/NotionInter-Bold.woff2")format("woff2"),url("https://www.notion.com/front-static/fonts/NotionInter-Bold.woff")format("woff");font-style:normal;font-weight:700;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Italic.2vb9zej_iju_y.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Italic.12i6afi9b9hxe.woff")format("woff");font-style:italic;font-weight:400;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic.2g12c_dh0rad3.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic.2rynykzgn0xv8.woff")format("woff");font-style:italic;font-weight:500;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic.275kiy_6teqt3.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic.3i3ekylt2dzo6.woff")format("woff");font-style:italic;font-weight:600;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic.3u147tw2czjpe.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic.08sixp5xcn5t3.woff")format("woff");font-style:italic;font-weight:700;font-display:swap}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Regular-i18n.00ioyd906d58c.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Regular-i18n.41t_njf6omqug.woff")format("woff");font-style:normal;font-weight:400;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Italic-i18n.13ttwp5t-mbd7.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Italic-i18n.0-k84asq6g8u0.woff")format("woff");font-style:italic;font-weight:400;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Medium-i18n.2323dzohbvk8n.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Medium-i18n.2tkojwvm96-0f.woff")format("woff");font-style:normal;font-weight:500;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-i18n.3c5zkal8qq863.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-i18n.3jlqi1wpho-1p.woff")format("woff");font-style:italic;font-weight:500;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-i18n.0v6npia89qig-.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-i18n.1pdr821pyw3m5.woff")format("woff");font-style:normal;font-weight:600;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-i18n.19mbftanf92cw.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-i18n.2c9ecteqq2dz6.woff")format("woff");font-style:italic;font-weight:600;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Bold-i18n.007-piztngqyv.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Bold-i18n.1kf1-bcapvitl.woff")format("woff");font-style:normal;font-weight:700;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-i18n.428p1llnba081.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-i18n.2tgc92j7lw1ya.woff")format("woff");font-style:italic;font-weight:700;font-display:swap;unicode-range:U+300-36F,U+C0-FF,U+100-17F,U+1EA0-1EF9}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Regular-math.1a6t35xyuxi20.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Regular-math.1hzylpes2g_bm.woff")format("woff");font-style:normal;font-weight:400;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Italic-math.22b8zyjp-fmrg.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Italic-math.0boesj398nbmg.woff")format("woff");font-style:italic;font-weight:400;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Medium-math.3h5a0h0lxvtg-.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Medium-math.1dgmj_gsijb1f.woff")format("woff");font-style:normal;font-weight:500;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-math.0q1zkx9qhcer0.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-MediumItalic-math.2le-vmg0w-w1c.woff")format("woff");font-style:italic;font-weight:500;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-math.0a6v2_nx97nws.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-SemiBold-math.0m755201v_cvt.woff")format("woff");font-style:normal;font-weight:600;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-math.0-zip_tvxb4gj.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-SemiBoldItalic-math.22oeklwa0ha-y.woff")format("woff");font-style:italic;font-weight:600;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-Bold-math.14rbjwnmavhus.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-Bold-math.2z3rh5kxmzpvv.woff")format("woff");font-style:normal;font-weight:700;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
@font-face{font-family:NotionInter;src:url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-math.2k5m59rf5np05.woff2")format("woff2"),url("https://www.notion.com/_next/static/media/NotionInter-BoldItalic-math.2qjvrl3b8y4s2.woff")format("woff");font-style:italic;font-weight:700;font-display:swap;unicode-range:U+370-3FF,U+2070-2073,U+2075-209F,U+2200-2211,U+2213-22FF}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction above a large workspace demonstration, then use spacious feature groups and editorial proof sections. Pricing groups four plans into two broader offer families, with the AI-oriented group on a pale blue surface. Mobile stacks those groups and their plans into a clear vertical flow.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 60px. Use smaller steps within a control and larger steps between content groups.

The sampled header is static, 308.109px high, with 0px left and 0px right padding. The sampled header is static, 108px high, with 24px left and 24px right padding.

Measured desktop grid tracks: `1440px` with gap `normal`; `188.656px 188.672px 188.672px 188.672px` with gap `80px 24px`; `476.891px 406.203px 476.906px` with gap `16px`. Build them as a fluid grid. Sampled container maximum widths: `500px`, `891.92px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `12px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact blue filled actions, pale blue companions, lightly rounded outlined panels, quiet billing switches and small feature checks. Keep product demonstrations dense while surrounding marketing copy has generous space and strong hierarchy.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 36px, horizontal padding 14px / 14px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 1px, radius 50%, background rgba(0, 0, 0, 0), and border 0px rgba(0, 0, 0, 0.5). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses hand-drawn characters, playful icons and detailed workspace demonstrations. Create original line illustrations and generic document or workflow diagrams without copying characters, screenshots, logos or customer marks.

**Motion.** Observed CSS transition declarations include `box-shadow 0.2s`, `background-color, border-color 0.2s`, `background-color 0.15s`, `all 0.2s`. These prove declared timing, not that a particular animation was watched end to end. The inline highlighted word changes between captures. Treat this as a dynamic content motif rather than a responsive copy rule; validate timing and reduced-motion behavior separately.

**Voice.** Clear, welcoming and practical, with concise benefit statements and simple actions.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
