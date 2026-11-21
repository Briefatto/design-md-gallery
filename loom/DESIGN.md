---
version: alpha
name: "Loom"
description: "Loom's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Loom."
colors:
  primary: "rgb(24, 104, 219)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(233, 242, 254)"
  foreground: "rgb(16, 18, 20)"
  muted: "rgb(41, 42, 46)"
  border: "rgba(0, 0, 0, 0.2)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Charlie Display", sans-serif'
    fontSize: 63.2692px
    fontWeight: 700
    lineHeight: 1.03
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Charlie Display", sans-serif'
    fontSize: 35px
    fontWeight: 700
    lineHeight: 1.03
    letterSpacing: 0em
  heading:
    fontFamily: '"Charlie Display", sans-serif'
    fontSize: 35px
    fontWeight: 700
    lineHeight: 1.03
    letterSpacing: 0em
  body:
    fontFamily: '"Charlie Text", sans-serif'
    fontSize: 18.6231px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: 0em
  action:
    fontFamily: '"Charlie Text", sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0em
rounded:
  control: 9999px
  card: 8px
spacing:
  xs: 6.30769px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 70.72px
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

# Loom DESIGN.md

## Overview

A video-communication site uses a bright blue and pale blue palette, strong Charlie Display headings, practical Charlie Text interface copy and large rounded media panels. The captured interface carries the current Atlassian-branded Loom treatment.

Built from [/](https://loom.com/) and [/pricing](https://loom.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(24, 104, 219)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(233, 242, 254)` | Panels and cards |
| foreground | `rgb(16, 18, 20)` | Primary text |
| muted | `rgb(41, 42, 46)` | Supporting text |
| border | `rgba(0, 0, 0, 0.2)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Charlie Display" | 63.2692px | 700 | 1.03 | 0em |
| display-mobile | "Charlie Display" | 35px | 700 | 1.03 | 0em |
| heading | "Charlie Display" | 35px | 700 | 1.03 | 0em |
| body | "Charlie Text" | 18.6231px | 400 | 1.65 | 0em |
| action | "Charlie Text" | 16px | 400 | 1.5 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 100; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 100; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 200; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 200; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 400; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Regular.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Regular.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 400; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 500; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 500; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 700; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 700; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: normal; font-weight: 800; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 800; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Display"; font-style: italic; font-weight: 900; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Ultra.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Ultra.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 100; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: italic; font-weight: 100; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 200; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: italic; font-weight: 200; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 400; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Regular.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Regular.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 500; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: italic; font-weight: 500; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 700; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: italic; font-weight: 700; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold_Italic.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: normal; font-weight: 800; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black.woff") format("woff"); }
@font-face { font-display: swap; font-family: "Charlie Text"; font-style: italic; font-weight: 800; src: url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black_Italic.woff2") format("woff2"), url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black_Italic.woff") format("woff"); }
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:100;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:100;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Thin_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:200;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:200;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Light.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:400;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Regular.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Regular.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:400;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:500;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:500;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Semibold_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:700;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:700;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Bold_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:normal;font-weight:800;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:800;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Black_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Display;font-style:italic;font-weight:900;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Ultra.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Display-Ultra.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:100;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:italic;font-weight:100;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Thin_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:200;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:italic;font-weight:200;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Light_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:400;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Regular.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Regular.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:500;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:italic;font-weight:500;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Semibold_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:700;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:italic;font-weight:700;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Bold_Italic.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:normal;font-weight:800;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black.woff") format("woff")}
@font-face{font-display:swap;font-family:Charlie Text;font-style:italic;font-weight:800;src:url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black_Italic.woff2") format("woff2"),url("https://cdn.loom.com/assets/marketing/fonts/Charlie_Text-Black_Italic.woff") format("woff")}
```

The full fallback stacks are in the front matter.

## Layout

Center the homepage introduction and paired actions above a prominent video panel, followed by proof and feature sections. Pricing places team-size and billing controls above four tall plan cards, with a pale blue featured plan. Mobile stacks the cards and keeps the controls compact.

Spacing scale: xs 6.30769px, sm 8px, md 16px, lg 24px, xl 32px, section 70.72px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 150px high, with 0px left and 0px right padding. The sampled header is static, 162.312px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `131px 132px 132px 134px 131px 37.5px 165px 108px 82px 132px 133px 113px 122px` with gap `111.04px`; `131px 132px 132px 134px 131px 37.5px 165px 108px 82px 132px 133px 113px 122px` with gap `111.04px`; `103px 144px 165px 165px 85px 149px` with gap `111.04px`. Build them as a fluid grid. Sampled container maximum widths: `1440px`, `640px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `rgba(0, 0, 0, 0.03) 0px 4px 6.4px 0px, rgba(0, 0, 0, 0.05) 0px 3px 9.6px 0px, rgba(0, 0, 0, 0.07) 0px 8px 32px 0px, rgba(0, 0, 0, 0.1) 0px 32px 96px 0px`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `9999px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use blue pill actions, pale blue companions, generously rounded media frames, soft shadows, clear featured-plan badges and precise feature lists. Keep display headlines strong while comparison text remains economical.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 48px, horizontal padding 15.6154px / 15.6154px, and gap 15.6154px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 36px, radius 14px, background rgb(255, 255, 255), and border 0px rgb(41, 42, 46). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** The source relies on video previews, product demonstrations and customer imagery. Use original licensed media and generic video-workflow diagrams without copying people, recordings, screenshots or organization marks.

**Motion.** Observed CSS transition declarations include `box-shadow 0.5s`, `background-color 0.6s`, `color, background-color, border-color, text-decoration-color, fill, stroke 0.15s`, `transform, background-color 0.1s, 0.1s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Friendly, clear and practical, with concise recording, sharing and collaboration labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and your coding agent reads this file before visual work and checks every piece it renders.
