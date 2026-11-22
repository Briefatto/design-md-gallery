---
version: alpha
name: "OpenClaw"
description: "OpenClaw's colours, type, radii, spacing and components as DESIGN.md tokens. Not affiliated with OpenClaw."
colors:
  primary: "rgb(245, 101, 74)"
  background: "oklch(0.135 0 0)"
  surface: "oklch(0.178 0 0)"
  foreground: "oklch(0.985 0 0)"
  muted: "oklch(0.716 0 0)"
  border: "oklch(0.269 0 0)"
  on-primary: "oklch(0.135 0 0)"
typography:
  display:
    fontFamily: 'Switzer, system-ui, sans-serif'
    fontSize: 60.8px
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: -0.03em
  display-mobile:
    fontFamily: 'Switzer, system-ui, sans-serif'
    fontSize: 38.4px
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: -0.03em
  heading:
    fontFamily: 'Switzer, system-ui, sans-serif'
    fontSize: 21.6px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.015em
  body:
    fontFamily: 'Switzer, system-ui, sans-serif'
    fontSize: 14.4px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: 0em
  action:
    fontFamily: 'Switzer, system-ui, sans-serif'
    fontSize: 16.32px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0em
  display-emphasis:
    fontFamily: 'Sentient, Georgia, serif'
    fontSize: 60.8px
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: -0.015em
rounded:
  control: 8px
  card: 0px
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

# OpenClaw DESIGN.md

## Overview

A developer-oriented assistant site uses a near-black neutral canvas, Switzer headings, coral actions, fine charcoal rules, and a terminal-like supporting layer. A single Sentient italic phrase softens the main headline, while an original ASCII-style atmosphere can provide depth without image-heavy framing.

Built from [/](https://openclaw.ai/) and [/integrations](https://openclaw.ai/integrations), captured on 2026-11-21 UTC at 1440×900 and 390×844. The front matter holds the computed values as portable tokens.

## Colors

| Token | Computed value | Role |
| --- | --- | --- |
| primary | `rgb(245, 101, 74)` | Priority actions and selected emphasis |
| background | `oklch(0.135 0 0)` | Page canvas |
| surface | `oklch(0.178 0 0)` | Panels and cards |
| foreground | `oklch(0.985 0 0)` | Primary text |
| muted | `oklch(0.716 0 0)` | Supporting text |
| border | `oklch(0.269 0 0)` | Quiet separators and outlines |
| on-primary | `oklch(0.135 0 0)` | Text on the primary action |



Keep the canvas and reading text neutral. Use coral for the priority action, selected technical labels, and sparing editorial emphasis. Sentient emphasis was measured at 60.8px, weight 400, italic, line-height 1.08, and tracking -0.015em; the base display remains Switzer. Alpha colors retain the captured opacity and must be composited over the intended background.

## Typography

| Role | First family | Size | Weight | Leading | Tracking |
| --- | --- | --- | --- | --- | --- |
| display | Switzer | 60.8px | 600 | 1.08 | -0.03em |
| display-mobile | Switzer | 38.4px | 600 | 1.08 | -0.03em |
| heading | Switzer | 21.6px | 600 | 1.2 | -0.015em |
| body | Switzer | 14.4px | 400 | 1.65 | 0em |
| action | Switzer | 16.32px | 600 | 1.2 | 0em |
| display-emphasis | Sentient | 60.8px | 400 | 1.08 | -0.015em |

Keep display, reading, and action roles distinct. The heading sample is the recurring section role, while display records the first prominent headline. Use the mobile display value at narrow widths; allow natural line wrapping and preserve the reading measure. The display transformation is `none` and its font style is `normal`; preserve these in CSS.

Font loading:

```css
@font-face {
  font-family: 'Switzer';
  src: url("https://cdn.fontshare.com/wf/BLNB4FAQFNK56DWWNF7PMGTCOTZHOEII/ST3WKSSDMBK2MIQQO3MAVYWLF4FTOLFV/6IN5WOLRCYP4G4MOCOHOMXNON6Q7MDAR.woff2") format('woff2'),
       url("https://cdn.fontshare.com/wf/BLNB4FAQFNK56DWWNF7PMGTCOTZHOEII/ST3WKSSDMBK2MIQQO3MAVYWLF4FTOLFV/6IN5WOLRCYP4G4MOCOHOMXNON6Q7MDAR.woff") format('woff'),
       url("https://cdn.fontshare.com/wf/BLNB4FAQFNK56DWWNF7PMGTCOTZHOEII/ST3WKSSDMBK2MIQQO3MAVYWLF4FTOLFV/6IN5WOLRCYP4G4MOCOHOMXNON6Q7MDAR.ttf") format('truetype');
  font-weight: 400;
  font-display: swap;
  font-style: normal;
}
@font-face {
  font-family: 'Switzer';
  src: url("https://cdn.fontshare.com/wf/OYB4CXKJQXKTNSLJMTDQOIVUL2V5EL7S/WYO2P7DQVV5RNXGMCUO2HL4RJP4VFUAS/6XPIMU23OJVRY676OG5YVJMWEHWICATX.woff2") format('woff2'),
       url("https://cdn.fontshare.com/wf/OYB4CXKJQXKTNSLJMTDQOIVUL2V5EL7S/WYO2P7DQVV5RNXGMCUO2HL4RJP4VFUAS/6XPIMU23OJVRY676OG5YVJMWEHWICATX.woff") format('woff'),
       url("https://cdn.fontshare.com/wf/OYB4CXKJQXKTNSLJMTDQOIVUL2V5EL7S/WYO2P7DQVV5RNXGMCUO2HL4RJP4VFUAS/6XPIMU23OJVRY676OG5YVJMWEHWICATX.ttf") format('truetype');
  font-weight: 500;
  font-display: swap;
  font-style: normal;
}
@font-face {
  font-family: 'Switzer';
  src: url("https://cdn.fontshare.com/wf/5SZVFDB7V52TI6ULVC6J3WQZQCIZVDV5/ODYPSTCUDMKSTYIPTV4CLQ7URIK7XYBJ/YS3VPNVO4B3TOJMEXDGFZQ4TLZGGSRZC.woff2") format('woff2'),
       url("https://cdn.fontshare.com/wf/5SZVFDB7V52TI6ULVC6J3WQZQCIZVDV5/ODYPSTCUDMKSTYIPTV4CLQ7URIK7XYBJ/YS3VPNVO4B3TOJMEXDGFZQ4TLZGGSRZC.woff") format('woff'),
       url("https://cdn.fontshare.com/wf/5SZVFDB7V52TI6ULVC6J3WQZQCIZVDV5/ODYPSTCUDMKSTYIPTV4CLQ7URIK7XYBJ/YS3VPNVO4B3TOJMEXDGFZQ4TLZGGSRZC.ttf") format('truetype');
  font-weight: 600;
  font-display: swap;
  font-style: normal;
}
@font-face {
  font-family: 'Switzer';
  src: url("https://cdn.fontshare.com/wf/HBNTRIISA5MEXGL5WPYI7CV2HIWTDV3Q/YDPDINVT673XLXNSTMLG4JNCZZMVVNPN/Y7SCNZJOT2MW5ADSGOFLDGH4TNL4JCQY.woff2") format('woff2'),
       url("https://cdn.fontshare.com/wf/HBNTRIISA5MEXGL5WPYI7CV2HIWTDV3Q/YDPDINVT673XLXNSTMLG4JNCZZMVVNPN/Y7SCNZJOT2MW5ADSGOFLDGH4TNL4JCQY.woff") format('woff'),
       url("https://cdn.fontshare.com/wf/HBNTRIISA5MEXGL5WPYI7CV2HIWTDV3Q/YDPDINVT673XLXNSTMLG4JNCZZMVVNPN/Y7SCNZJOT2MW5ADSGOFLDGH4TNL4JCQY.ttf") format('truetype');
  font-weight: 700;
  font-display: swap;
  font-style: normal;
}
```

The full fallback stacks are in the front matter.

## Layout

Use a slim navigation, centered opening statement, and compact starting actions above a tabbed installation panel. Keep subsequent technical sections on a consistent reading grid. The integrations page uses a concise introduction, divided summary metrics, and a ruled multi-column directory that stacks on mobile.

Spacing scale: xs 2px, sm 8px, md 16px, lg 24px, xl 32px, section 64px. Use smaller steps within a control and larger steps between content groups.

The sampled header is sticky, 64px high, with 32px left and 32px right padding. The sampled header is relative, 684.547px high, with 0px left and 0px right padding.

Measured desktop grid tracks: `192.391px 192.406px 192.391px 192.406px 192.391px` with gap `normal`; `252px 252px 252px` with gap `1px`; `319.328px 319.328px 319.344px` with gap `1px`. Build them as a fluid grid. Sampled container maximum widths: `760px`, `620px`.

At narrow widths, keep the content order, let columns stack, wrap action groups, and give navigation a compact treatment. Recreate the observed desktop and mobile differences, with breakpoints chosen for your layout.

## Elevation & Depth

The sampled card shadow is `rgba(245, 101, 74, 0.4) 0px 0px 0px 1px inset`. Keep most reading surfaces quiet. Use borders and surface contrast for grouping; reserve stronger depth for floating controls or intentional feature panels.

## Shapes

Controls use `8px`; the reusable card treatment uses `0px`. Keep corner geometry consistent within each component family. Do not automatically apply the card radius to every image, badge, or full-width section.

## Components

Use small coral filled actions, thin outlined companions, monochrome code panels, tab strips, tiny tracked monospace labels, and directory cells separated by rules. Keep rounding modest and let alignment do most grouping.

- **Primary and secondary actions:** use primary/on-primary for the priority action and a surface/foreground or outlined treatment for the supporting action. The sampled action has height 44px, horizontal padding 24px / 24px, and gap 8px. Keep labels short and allow enough hit area for touch.
- **Cards:** group one heading, supporting text, and a clear next step. Preserve the hierarchy and spacing; avoid making every element a nested card.
- **Navigation:** retain the captured information hierarchy and distinguish navigation links from the main call to action. Provide a visible keyboard focus treatment.
- **Forms:** the sampled field uses height 62px, radius 0px, background oklch(0.178 0 0), and border 1px oklch(0.269 0 0). Add persistent labels, useful errors, and clear disabled/focus states.

**Imagery and iconography.** Use original ASCII fields, abstract point geometry, workflow diagrams, and neutral code examples.

**Motion.** Observed CSS transition declarations include `background-color, color 0.25s, 0.25s`, `color, border-color 0.15s, 0.15s`, `flex-basis, width, background 0.28s, 0.28s, 0.15s`, `background, border-color 0.15s, 0.15s`. Use restrained feedback and respect reduced-motion preferences.

**Voice.** Direct, practical, and comfortable with technical terminology.

## Do's and Don'ts

- Do preserve the palette roles, type hierarchy, and relationship between dense controls and larger section spacing.
- Do keep content readable at both captured widths and provide focus, error, loading, and reduced-motion behavior for any new interface.
- Do use simple geometric placeholders for imagery.
- Don't reproduce the logo, brand illustrations, product screenshots, or marketing text.
- Don't let added decoration compete with the site's defining typography, content rhythm, and action hierarchy.

---

Made with [Briefatto Board](https://github.com/Briefatto/briefatto-board). Run `npx briefatto-board install` and every agent reads this file before visual work and checks every piece it renders.
