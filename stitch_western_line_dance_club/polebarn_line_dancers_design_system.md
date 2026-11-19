---
name: "Rustic Timber & Saddle"
description: "A warm, authentic western design system tailored for community line dancing, featuring saddle leather tones, barnwood neutrals, and honest Americana typography."
---

## Overview

The Polebarn Line Dancers design system evokes the spirit of an authentic country dance hall: weathered cedar timber, glowing incandescent string lights, polished maple dance floors, and hand-tooled saddle leather. It is welcoming to absolute beginners stepping onto the hardwood for the first time, while honoring the rich tradition, step-sheet precision, and camaraderie of seasoned country dancers.

The design language balances tactile warmth with high legibility—pairing hearty transitional serif display typography with clean humanist sans body copy for effortless reading under event lighting or on mobile devices.

## Colors

The palette draws directly from the dance barn: rich saddle leather brown, warm whiskey amber accents, deep cedar timber framing, toasted cream surfaces, and clear high-contrast text.

- **Primary:** Deep saddle leather (`#5C2E0B`) anchoring headers and primary actions with rugged authority.
- **Secondary:** Warm cedar rust (`#8C3B14`) for secondary navigation, step difficulty badges, and active highlights.
- **Accent:** Warm whiskey gold (`#C87D20`) for calls-to-action, dance floor stars, and spotlighted events.
- **Surface:** Sunlit buttermilk cream (`#FDFBF7`) and soft barnwood parchment (`#F5EFEB`) delivering an inviting, organic glow.

```yaml
colors:
  accent: "#C87D20"
  secondary: "#8C3B14"
  border: "#E2D7C8"
  light:
    primary: "#5C2E0B"
    on-primary: "#FFFFFF"
    surface: "#FDFBF7"
    on-surface: "#2A1810"
    surface-container: "#F5EFEB"
    surface-container-high: "#EAE0D2"
    on-surface-variant: "#6B584D"
  dark:
    primary: "#F5C28E"
    on-primary: "#3D1A04"
    surface: "#1C140F"
    on-surface: "#F5ECE5"
    surface-container: "#2B1E17"
    surface-container-high: "#3A2B21"
    on-surface-variant: "#C4B2A5"
```

## Typography

This system uses **Castoro** as an expressive, authentic western headline serif with traditional American broadside heritage, paired with **Merriweather Sans** for clear, open humanist body text and step-by-step dance instructions. **Spline Sans Mono** handles dance counts (32-count, 4-wall), BPMs, and event start times.

```yaml
typography:
  display-lg:
    fontFamily: "Castoro"
    fontSize: 48px
    fontWeight: 700
    lineHeight: 56px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Castoro"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 40px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: "Castoro"
    fontSize: 36px
    fontWeight: 700
    lineHeight: 44px
    letterSpacing: -0.25px
  headline-lg-mobile:
    fontFamily: "Castoro"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 34px
  headline-md:
    fontFamily: "Castoro"
    fontSize: 24px
    fontWeight: 600
    lineHeight: 32px
  headline-sm:
    fontFamily: "Castoro"
    fontSize: 20px
    fontWeight: 600
    lineHeight: 28px
  title-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 18px
    fontWeight: 700
    lineHeight: 26px
  body-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
  body-md:
    fontFamily: "Merriweather Sans"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
  label-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 14px
    fontWeight: 700
    lineHeight: 20px
  label-md:
    fontFamily: "Merriweather Sans"
    fontSize: 12px
    fontWeight: 600
    lineHeight: 16px
  mono-sm:
    fontFamily: "Spline Sans Mono"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
```

## Layout & Spacing

Layouts follow a fluid, responsive container system with a max width of 1280px on desktop and cozy touch-friendly gutters on mobile. Rhythms are spaced on an 8px scale.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 64px
  page-margin: 24px
```

## Elevation & Depth

Surfaces emphasize tactile natural layering rather than heavy artificial drop shadows. Borders feature warm subtle outlines (`#E2D7C8`) paired with soft ambient diffusion (`0 4px 20px -2px rgba(42, 24, 16, 0.08)`). Badges, cards, and banners feel like embossed leather patches and framed wooden placards.

## Shapes

Corners feature grounded, gently rounded corners (8px default, 16px on hero cards) reminiscent of sanded cedar planks, saddle stitch corners, and vintage event tickets.

```yaml
rounded:
  sm: 4px
  DEFAULT: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Micro-interactions feel smooth, physical, and friendly—reminiscent of tactile tavern doors and responsive stepping. Transitions avoid snappy digital flashes.

```yaml
motion:
  state-change:
    duration: 150ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 250ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

- **Tone:** Warm, communal, encouraging, and genuine. We speak with down-home hospitality without caricature. Absolute beginners are met with reassurance ("No partner needed, two left feet welcome!").
- **Terminology:** "Floor Call", "Step Sheet", "Wall Count", "BPM", "Social Stomp", "Open Floor", "Walkthrough", "Barn Night".
- **Action Labels:** Action-driven and descriptive: "View Step Sheet", "RSVP for Saturday Stomp", "Filter by Beginner Level", "Download Practice Track".

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Table** → `@components/table.html`: `table-standard`, `table-interactive`, `table-selectable`
- **Tabs** → `@components/tabs.html`: `tabs-horizontal`, `tabs-with-icon`
