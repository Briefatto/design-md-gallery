---
version: alpha
name: "Gemini CLI"
description: "Gemini CLI's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with Gemini CLI."
colors:
  primary: "rgb(54, 75, 255)"
  background: "rgb(6, 6, 6)"
  surface: "rgb(255, 255, 255)"
  foreground: "rgb(255, 255, 255)"
  muted: "oklab(0.999994 0.0000455677 0.0000200868 / 0.7)"
  border: "rgb(236, 238, 242)"
  on-primary: "rgb(255, 255, 255)"
typography:
  display:
    fontFamily: '"Google Sans", Arial, sans-serif'
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  display-mobile:
    fontFamily: '"Google Sans", Arial, sans-serif'
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0em
  heading:
    fontFamily: '"Google Sans", Arial, sans-serif'
    fontSize: 35px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0em
  body:
    fontFamily: '"Google Sans Text", Arial, sans-serif, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
    letterSpacing: 0em
  action:
    fontFamily: '"Google Sans Text", Arial, sans-serif, ui-sans-serif, system-ui, -apple-system, "system-ui", "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"'
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.43
    letterSpacing: 0em
rounded:
  control: 4px
  card: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  section: 40px
components:
  primary-button:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.control}"
---

# Gemini CLI DESIGN.md

## Overview

The landing page uses a near-black terminal atmosphere, light Google Sans display type, and small blue/purple accents. The documentation route switches to white reading surfaces while retaining the type family and technical hierarchy.

Built from [/](https://geminicli.com/) and [/docs/](https://geminicli.com/docs/), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(54, 75, 255)` | Priority actions and selected emphasis |
| background | `rgb(6, 6, 6)` | Page canvas |
| surface | `rgb(255, 255, 255)` | Panels and cards |
| foreground | `rgb(255, 255, 255)` | Primary text |
| muted | `oklab(0.999994 0.0000455677 0.0000200868 / 0.7)` | Supporting text |
| border | `rgb(236, 238, 242)` | Quiet separators and outlines |
| on-primary | `rgb(255, 255, 255)` | Text on the primary action |

Use the dark palette for the landing-page interpretation. Documentation uses a separate light canvas; do not combine its dark reading text with the dark landing background. The green announcement strip is transient page chrome, not the core action color. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | "Google Sans" | 52px | 400 | 1.25 | 0em |
| display-mobile | "Google Sans" | 32px | 400 | 1.25 | 0em |
| heading | "Google Sans" | 35px | 500 | 1.2 | 0em |
| body | "Google Sans Text" | 16px | 400 | 1.75 | 0em |
| action | "Google Sans Text" | 14px | 700 | 1.43 | 0em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure.

Font loading:

```css
@font-face {
  font-family: 'Google Sans Text';
  font-style: normal;
  font-weight: 400;
  font-display: block;
  src: url("https://fonts.gstatic.com/s/googlesanstext/v29/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2i0VBuxM.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans Text';
  font-style: normal;
  font-weight: 500;
  font-display: block;
  src: url("https://fonts.gstatic.com/s/googlesanstext/v29/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtjm4DZw.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 400;
  font-display: block;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 500;
  font-display: block;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
@font-face {
  font-family: 'Google Sans';
  font-style: normal;
  font-weight: 700;
  font-display: block;
  src: url("https://fonts.gstatic.com/s/googlesans/v76/4UasrENHsxJlGDuGo1OIlJfC6l_24rlCK1Yo_Iqcsih3SAyH6cAwhX9RPjIUvbQoi-E.woff2") format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

The full fallback stacks are in the front matter.

## Layout

Keep the installation or starting point prominent, then move into documentation sections with a readable text measure.

Spacing scale: xs 4px, sm 8px, md 16px, lg 24px, xl 32px, section 40px. Use smaller steps within a control and larger steps between content groups.

The sampled header is relative, 76px high, with 0px left and 0px right padding. The sampled header is relative, 76px high, with 0px left and 24px right padding.

 Sampled container maximum widths: `600px`, `1080px`, `720px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled surface shadow is `none`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `4px`; the reusable card treatment uses `8px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use compact actions, monospace command examples, quiet containers, and straightforward navigation.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 30px, horizontal padding 8px / 8px, and gap normal. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** build fields from the action typography, control radius, and separator color. Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original terminal examples and simple geometric motifs; do not reproduce the brand mark.

**Motion.** Observed CSS transition declarations include `color 0.2s`, `all 0.2s`, `opacity, background, border-color 0.2s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Practical, explanatory, and approachable to developers.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

