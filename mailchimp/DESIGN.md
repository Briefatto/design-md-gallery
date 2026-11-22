---
version: alpha
name: "Mailchimp"
description: "Mailchimp's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Mailchimp."
colors:
  primary: "rgb(255, 224, 27)"
  background: "rgb(255, 255, 255)"
  surface: "rgb(239, 238, 234)"
  foreground: "rgb(35, 30, 21)"
  muted: "rgba(35, 30, 21, 0.65)"
  border: "rgb(222, 222, 222)"
  on-primary: "rgb(35, 30, 21)"
typography:
  display:
    fontFamily: '"Means Web", Georgia, Times, "Times New Roman", serif'
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.019em
  display-mobile:
    fontFamily: '"Means Web", Georgia, Times, "Times New Roman", serif'
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0em
  heading:
    fontFamily: '"Means Web", Georgia, Times, "Times New Roman", serif'
    fontSize: 29.25px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.017em
  body:
    fontFamily: 'Tally, "Graphik Web", "Helvetica Neue", Helvetica, Arial, Verdana, sans-serif'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  action:
    fontFamily: 'Tally, "Graphik Web", "Helvetica Neue", Helvetica, Arial, Verdana, sans-serif'
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0em
rounded:
  control: 26px
  card: 10px
spacing:
  xs: 2px
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

# Mailchimp DESIGN.md

## Overview

A lively editorial system pairs expressive Means Web serif headings with compact Tally interface text, warm near-black and saturated yellow.

Built from [/](https://mailchimp.com/) and [/pricing](https://mailchimp.com/pricing), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(255, 224, 27)` | Priority actions and selected emphasis |
| background | `rgb(255, 255, 255)` | Page canvas |
| surface | `rgb(239, 238, 234)` | Panels and cards |
| foreground | `rgb(35, 30, 21)` | Primary text |
| muted | `rgba(35, 30, 21, 0.65)` | Supporting text |
| border | `rgb(222, 222, 222)` | Quiet separators and outlines |
| on-primary | `rgb(35, 30, 21)` | Text on the primary action |



Keep the page ground and text pairing stable. Give the primary color a clear job in actions, selection, or links; use surface changes and thin rules to organize secondary content. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Means Web" | 64px | 400 | 1.2 | -0.019em |
| display-mobile | "Means Web" | 36px | 400 | 1.3 | 0em |
| heading | "Means Web" | 29.25px | 400 | 1 | -0.017em |
| body | Tally | 16px | 400 | 1.25 | 0em |
| action | Tally | 13px | 700 | 1.1 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Light-Web.woff2") format("woff2"); font-weight: 300; font-style: normal; font-display: fallback; }
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-LightItalic-Web.woff2") format("woff2"); font-weight: 300; font-style: italic; font-display: fallback; }
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Regular-Web.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: fallback; }
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-RegularItalic-Web.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: fallback; }
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Medium-Web.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: fallback; }
@font-face { font-family: "Means Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-MediumItalic-Web.woff2") format("woff2"); font-weight: 500; font-style: italic; font-display: fallback; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Light-Web.woff2") format("woff2"); font-weight: 300; font-style: normal; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-LightItalic-Web.woff2") format("woff2"); font-weight: 300; font-style: italic; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Regular-Web.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-RegularItalic-Web.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Medium-Web.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-MediumItalic-Web.woff2") format("woff2"); font-weight: 500; font-style: italic; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Semibold-Web.woff2") format("woff2"); font-weight: 600; font-style: normal; font-display: optional; }
@font-face { font-family: "Graphik Web"; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-SemiboldItalic-Web.woff2") format("woff2"); font-weight: 600; font-style: italic; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Regular.woff2") format("woff2"); font-weight: 400; font-style: normal; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-RegularItalic.woff2") format("woff2"); font-weight: 400; font-style: italic; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Medium.woff2") format("woff2"); font-weight: 500; font-style: normal; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-MediumItalic.woff2") format("woff2"); font-weight: 500; font-style: italic; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Bold.woff2") format("woff2"); font-weight: 700; font-style: normal; font-display: optional; }
@font-face { font-family: Tally; src: url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-BoldItalic.woff2") format("woff2"); font-weight: 700; font-style: italic; font-display: optional; }
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Light-Web.woff2")format("woff2");font-weight:300;font-style:normal;font-display:fallback}
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-LightItalic-Web.woff2")format("woff2");font-weight:300;font-style:italic;font-display:fallback}
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Regular-Web.woff2")format("woff2");font-weight:400;font-style:normal;font-display:fallback}
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-RegularItalic-Web.woff2")format("woff2");font-weight:400;font-style:italic;font-display:fallback}
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-Medium-Web.woff2")format("woff2");font-weight:500;font-style:normal;font-display:fallback}
@font-face{font-family:Means Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/means/Means-MediumItalic-Web.woff2")format("woff2");font-weight:500;font-style:italic;font-display:fallback}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Light-Web.woff2")format("woff2");font-weight:300;font-style:normal;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-LightItalic-Web.woff2")format("woff2");font-weight:300;font-style:italic;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Regular-Web.woff2")format("woff2");font-weight:400;font-style:normal;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-RegularItalic-Web.woff2")format("woff2");font-weight:400;font-style:italic;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Medium-Web.woff2")format("woff2");font-weight:500;font-style:normal;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-MediumItalic-Web.woff2")format("woff2");font-weight:500;font-style:italic;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-Semibold-Web.woff2")format("woff2");font-weight:600;font-style:normal;font-display:optional}
@font-face{font-family:Graphik Web;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/graphik/Graphik-SemiboldItalic-Web.woff2")format("woff2");font-weight:600;font-style:italic;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Regular.woff2")format("woff2");font-weight:400;font-style:normal;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-RegularItalic.woff2")format("woff2");font-weight:400;font-style:italic;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Medium.woff2")format("woff2");font-weight:500;font-style:normal;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-MediumItalic.woff2")format("woff2");font-weight:500;font-style:italic;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-Bold.woff2")format("woff2");font-weight:700;font-style:normal;font-display:optional}
@font-face{font-family:Tally;src:url("https://mailchimp.com/cdn/product/fonts/mailchimp/tally/1.0.2/Tally-BoldItalic.woff2")format("woff2");font-weight:700;font-style:italic;font-display:optional}
```

The full fallback stacks are in the front matter.

## Layout

Alternate wide photographic statements with pale neutral product sections. Pricing combines a split introductory offer with a compact white plan card, then a detailed ruled comparison grid; mobile stacks the offer and plan.

Spacing scale: xs 2px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 68px high, with 0px left and 0px right padding. The sampled nav is relative, 68px high, with 16px left and 16px right padding.

 Sampled container maximum widths: `960px`, `100%`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `26px`; the reusable card treatment uses `10px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Yellow pill actions, outlined secondary pills, small circular arrow controls and fine dark rules establish the visual rhythm. Use subtle card shadows only where a plan floats above the background.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 43.5px, horizontal padding 24px / 24px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 20px, radius 50%, background rgba(0, 0, 0, 0), and border 0px rgb(0, 0, 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Warm photography, colorful product screenshots, small hand-drawn accents and simple circular benefit icons carry the brand personality.

**Motion.** Observed CSS transition declarations include `background-color 0.2s`, `background-color 0.15s`, `transform, opacity 0.2s, 0.2s`, `transform, box-shadow 0.3s, 0.3s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Conversational, optimistic and concrete; expressive headlines lead to short action labels.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't replace the defining spacing and type proportions with unrelated decorative effects.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
