---
version: alpha
name: "Dropbox"
description: "Dropbox's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Dropbox."
colors:
  primary: "rgb(0, 97, 254)"
  background: "rgb(247, 245, 242)"
  surface: "rgb(247, 245, 242)"
  foreground: "rgb(30, 25, 25)"
  muted: "rgba(82, 74, 62, 0.82)"
  border: "rgb(247, 245, 242)"
  on-primary: "rgb(247, 245, 242)"
typography:
  display:
    fontFamily: '"Sharp Grotesk", SharpGrotesk, "Sharp Grotesk KR", "Sharp Grotesk Thai", "Atlas Grotesk Web", "Atlas Grotesk", AtlasGrotesk, -apple-system, "system-ui", "Segoe UI", "Helvetica Neue", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Sharp Grotesk", SharpGrotesk, "Atlas Grotesk Web", "Atlas Grotesk", AtlasGrotesk, -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif'
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.015em
  heading:
    fontFamily: '"Sharp Grotesk", SharpGrotesk, "Sharp Grotesk KR", "Sharp Grotesk Thai", "Atlas Grotesk Web", "Atlas Grotesk", AtlasGrotesk, -apple-system, "system-ui", "Segoe UI", "Helvetica Neue", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Atlas Grotesk Web", "Atlas Grotesk", AtlasGrotesk, -apple-system, "system-ui", "Segoe UI", "Helvetica Neue", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
  action:
    fontFamily: '"Atlas Grotesk Web", "Atlas Grotesk", AtlasGrotesk, -apple-system, "system-ui", "Segoe UI", "Helvetica Neue", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"'
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 12px
  card: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 48px
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

# Dropbox DESIGN.md

## Overview

A file and collaboration platform combines warm neutral surfaces, strong grotesk headings, practical Atlas interface text and vivid blue actions. Product demonstrations and selective lime plan signals provide contrast to the restrained reading surfaces.

Built from [/](https://dropbox.com/) and [/pricing](https://dropbox.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(0, 97, 254)` | Priority actions and selected emphasis |
| background | `rgb(247, 245, 242)` | Page canvas |
| surface | `rgb(247, 245, 242)` | Panels and cards |
| foreground | `rgb(30, 25, 25)` | Primary text |
| muted | `rgba(82, 74, 62, 0.82)` | Supporting text |
| border | `rgb(247, 245, 242)` | Quiet separators and outlines |
| on-primary | `rgb(247, 245, 242)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Sharp Grotesk" | 40px | 500 | 1.2 | 0em |
| display-mobile | "Sharp Grotesk" | 40px | 500 | 1.1 | -0.015em |
| heading | "Sharp Grotesk" | 32px | 400 | 1.2 | 0em |
| body | "Atlas Grotesk Web" | 16px | 400 | 1.5 | 0em |
| action | "Atlas Grotesk Web" | 14px | 500 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Atlas Grotesk Web"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflk7bxjs.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflyEJFZg.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflJ3txfq.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: "Atlas Grotesk Web"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vflOIRvCj.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vflDo8Kta.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vfllxpplt.ttf") format("truetype"); font-weight: 400; font-style: italic; }
@font-face { font-family: "Atlas Grotesk Web"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vfl38XiTL.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vflyja8tN.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vflbI0jjP.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: "Atlas Grotesk Web"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vfliTEIPs.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vflSOoqcm.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vflp44bwY.ttf") format("truetype"); font-weight: 500; font-style: italic; }
@font-face { font-family: "Sharp Grotesk"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vfl6-4ZSp.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vflay0Vof.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vflBru9m9.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: "Sharp Grotesk"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflwCQ830.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflYS2fRH.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflAAS2f2.ttf") format("truetype"); font-weight: 400; font-style: italic; }
@font-face { font-family: "Sharp Grotesk"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vflI3qtaE.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vflXS-0WC.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vfls8l7-a.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: "Sharp Grotesk"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vfltFffZa.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vflYvafQB.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vflbICI7o.ttf") format("truetype"); font-weight: 500; font-style: italic; }
@font-face { font-family: "Sharp Grotesk KR"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vfl9wW8_g.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vfltMRUQR.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vflobyC-1.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: "Sharp Grotesk KR"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vflHQZNTE.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vflVZ2WV-.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vfliXzeWX.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: "Sharp Grotesk Thai"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vflP_GuC6.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vflvm5YIY.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vfluZAIYj.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: "Sharp Grotesk Thai"; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vflFc-HqT.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vfl21-x5L.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vflGNZ9CT.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflugmAly.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflWr14lv.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflYSEsbG.ttf") format("truetype"); font-weight: 100; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflP-manv.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflmKWqdQ.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflHYkDrv.ttf") format("truetype"); font-weight: 100; font-style: italic; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vflvAXMid.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vfl9_ktQy.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vflc5lLwp.ttf") format("truetype"); font-weight: 300; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vflq-t642.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vfl1PZNwi.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vflvfjS6x.ttf") format("truetype"); font-weight: 300; font-style: italic; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflk7bxjs.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflyEJFZg.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflJ3txfq.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vflOIRvCj.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vflDo8Kta.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vfllxpplt.ttf") format("truetype"); font-weight: 400; font-style: italic; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vfl38XiTL.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vflyja8tN.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vflbI0jjP.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vfliTEIPs.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vflSOoqcm.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vflp44bwY.ttf") format("truetype"); font-weight: 500; font-style: italic; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vfl39K48X.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vflaLofNp.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vflD33tdn.ttf") format("truetype"); font-weight: 700; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflk44sx_.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflIKY_FY.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflntJR9Z.ttf") format("truetype"); font-weight: 700; font-style: italic; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflp3rI0W.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflY3PiPg.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflNBqfnS.ttf") format("truetype"); font-weight: 900; font-style: normal; }
@font-face { font-family: AtlasGrotesk; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflCRgLG7.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflLHCpzg.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflazUzhM.ttf") format("truetype"); font-weight: 900; font-style: italic; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vfl6-4ZSp.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflay0Vof.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflBru9m9.ttf") format("truetype"); font-weight: 400; font-style: normal; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflwCQ830.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflYS2fRH.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflAAS2f2.ttf") format("truetype"); font-weight: 400; font-style: italic; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflI3qtaE.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflXS-0WC.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vfls8l7-a.ttf") format("truetype"); font-weight: 500; font-style: normal; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vfltFffZa.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vflYvafQB.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vflbICI7o.ttf") format("truetype"); font-weight: 500; font-style: italic; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflsuA9PK.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflbRns0b.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflTu1-s0.ttf") format("truetype"); font-weight: 600; font-style: normal; }
@font-face { font-family: SharpGrotesk; font-display: swap; src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflgGzNpl.woff2") format("woff2"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vfl9WOTTB.woff") format("woff"), url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflBaHh8U.ttf") format("truetype"); font-weight: 600; font-style: italic; }
@font-face {
  font-family: 'Atlas Grotesk Web';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflk7bxjs.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflyEJFZg.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Web-vflJ3txfq.ttf")
      format('truetype');
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'Atlas Grotesk Web';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vflOIRvCj.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vflDo8Kta.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Regular-Italic-Web-vfllxpplt.ttf")
      format('truetype');
  font-weight: 400;
  font-style: italic;
}
@font-face {
  font-family: 'Atlas Grotesk Web';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vfl38XiTL.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vflyja8tN.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Web-vflbI0jjP.ttf")
      format('truetype');
  font-weight: 500;
  font-style: normal;
}
@font-face {
  font-family: 'Atlas Grotesk Web';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vfliTEIPs.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vflSOoqcm.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/atlas_grotesk/AtlasGrotesk-Medium-Italic-Web-vflp44bwY.ttf")
      format('truetype');
  font-weight: 500;
  font-style: italic;
}
@font-face {
  font-family: 'Sharp Grotesk';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vfl6-4ZSp.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vflay0Vof.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBook20-vflBru9m9.ttf")
      format('truetype');
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'Sharp Grotesk';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflwCQ830.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflYS2fRH.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrBookItalic20-vflAAS2f2.ttf")
      format('truetype');
  font-weight: 400;
  font-style: italic;
}
@font-face {
  font-family: 'Sharp Grotesk';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vflI3qtaE.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vflXS-0WC.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMedium20-vfls8l7-a.ttf")
      format('truetype');
  font-weight: 500;
  font-style: normal;
}
@font-face {
  font-family: 'Sharp Grotesk';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vfltFffZa.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vflYvafQB.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/SharpGroteskDBCyrMediumItalic20-vflbICI7o.ttf")
      format('truetype');
  font-weight: 500;
  font-style: italic;
}
@font-face {
  font-family: 'Sharp Grotesk KR';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vfl9wW8_g.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vfltMRUQR.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Book20-vflobyC-1.ttf")
      format('truetype');
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'Sharp Grotesk KR';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vflHQZNTE.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vflVZ2WV-.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/korean/SharpGroteskDBKO-Medium20-vfliXzeWX.ttf")
      format('truetype');
  font-weight: 500;
  font-style: normal;
}
@font-face {
  font-family: 'Sharp Grotesk Thai';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vflP_GuC6.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vflvm5YIY.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiBook-20-vfluZAIYj.ttf")
      format('truetype');
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'Sharp Grotesk Thai';
  src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vflFc-HqT.woff2")
      format('woff2'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vfl21-x5L.woff")
      format('woff'),
    url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/dig-fonts/sharp_grotesk/thai/SharpGroteskDBThaiMedium-20-vflGNZ9CT.ttf")
      format('truetype');
  font-weight: 500;
  font-style: normal;
}
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20.ttf")
                format('truetype');
        font-weight: $font_weight_book;
        font-style: normal;
    }
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20.ttf")
                format('truetype');
        font-weight: $font_weight_book;
        font-style: italic;
    }
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20.ttf")
                format('truetype');
        font-weight: $font_weight_medium;
        font-style: normal;
    }
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20.ttf")
                format('truetype');
        font-weight: $font_weight_medium;
        font-style: italic;
    }
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20.ttf")
                format('truetype');
        font-weight: $font_weight_semibold;
        font-style: normal;
    }
@font-face {
        font-family: 'SharpGrotesk';
        font-display: swap;
        src: url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20.eot");
        src:
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20.eot")
                format('embedded-opentype'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20.woff2")
                format('woff2'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20.woff")
                format('woff'),
            url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20.ttf")
                format('truetype');
        font-weight: $font_weight_semibold;
        font-style: italic;
    }
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflugmAly.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflWr14lv.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Thin-Web-vflYSEsbG.ttf") format("truetype");font-weight:100;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflP-manv.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflmKWqdQ.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-ThinItalic-Web-vflHYkDrv.ttf") format("truetype");font-weight:100;font-style:italic}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vflvAXMid.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vfl9_ktQy.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Light-Web-vflc5lLwp.ttf") format("truetype");font-weight:300;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vflq-t642.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vfl1PZNwi.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-LightItalic-Web-vflvfjS6x.ttf") format("truetype");font-weight:300;font-style:italic}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflk7bxjs.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflyEJFZg.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Regular-Web-vflJ3txfq.ttf") format("truetype");font-weight:400;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vflOIRvCj.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vflDo8Kta.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-RegularItalic-Web-vfllxpplt.ttf") format("truetype");font-weight:400;font-style:italic}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vfl38XiTL.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vflyja8tN.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Medium-Web-vflbI0jjP.ttf") format("truetype");font-weight:500;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vfliTEIPs.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vflSOoqcm.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-MediumItalic-Web-vflp44bwY.ttf") format("truetype");font-weight:500;font-style:italic}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vfl39K48X.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vflaLofNp.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Bold-Web-vflD33tdn.ttf") format("truetype");font-weight:700;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflk44sx_.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflIKY_FY.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BoldItalic-Web-vflntJR9Z.ttf") format("truetype");font-weight:700;font-style:italic}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflp3rI0W.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflY3PiPg.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-Black-Web-vflNBqfnS.ttf") format("truetype");font-weight:900;font-style:normal}
@font-face{font-family:'AtlasGrotesk';src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflCRgLG7.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflLHCpzg.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/paper-atlasgrotesk/AtlasGrotesk-BlackItalic-Web-vflazUzhM.ttf") format("truetype");font-weight:900;font-style:italic}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflyTZCFu.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflyTZCFu.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vfl6-4ZSp.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflay0Vof.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBook20-vflBru9m9.ttf") format("truetype");font-weight:400;font-style:normal}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vfltXscaV.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vfltXscaV.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflwCQ830.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflYS2fRH.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBBookItalic20-vflAAS2f2.ttf") format("truetype");font-weight:400;font-style:italic}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflxc0xOG.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflxc0xOG.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflI3qtaE.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vflXS-0WC.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMedium20-vfls8l7-a.ttf") format("truetype");font-weight:500;font-style:normal}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vfl7NEbfO.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vfl7NEbfO.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vfltFffZa.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vflYvafQB.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBMediumItalic20-vflbICI7o.ttf") format("truetype");font-weight:500;font-style:italic}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vfl49YBmP.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vfl49YBmP.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflsuA9PK.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflbRns0b.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBold20-vflTu1-s0.ttf") format("truetype");font-weight:600;font-style:normal}
@font-face{font-family:'SharpGrotesk';font-display:swap;src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflouajOT.eot");src:url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflouajOT.eot") format("embedded-opentype"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflgGzNpl.woff2") format("woff2"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vfl9WOTTB.woff") format("woff"),url("https://cfl.dropboxstatic.com/static/metaserver/static/fonts/sharpgrotesk/SharpGroteskDBSmBoldItalic20-vflBaHh8U.ttf") format("truetype");font-weight:600;font-style:italic}
```

The full fallback stacks are in the front matter.

## Layout

Use a two-column desktop introduction with a product demonstration beside concise copy and actions. The captured mobile homepage instead uses a blue media-led introduction. Pricing organizes rounded neutral plan cards in a repeated desktop row and a vertical mobile sequence.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 48px. Use smaller steps within a control and larger steps between content groups.

The sampled nav is sticky, 72px high, with 24px left and 24px right padding. The sampled nav is sticky, 72px high, with 24px left and 24px right padding.

Measured desktop grid tracks: `513.219px` with gap `16px normal`; `31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px` with gap `24px`; `31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px 31px` with gap `24px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `12px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use bright blue priority actions, quiet text companions, softly rounded plan cards, compact billing radio controls and clear feature lists. Featured-plan ribbons may use a lime accent while the core action and reading hierarchy remains blue and neutral.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 40px, horizontal padding 12px / 12px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 32px, radius 0px, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source uses file-interface demonstrations, abstract media and customer imagery. Create original generic file and collaboration specimens without copying files, screenshots, portraits, logos or source artwork.

**Motion.** Observed CSS transition declarations include `color 0.125s`, `background-color, border-color 0.1s, 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Clear, reassuring and practical, with concise storage, sharing and collaboration labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
