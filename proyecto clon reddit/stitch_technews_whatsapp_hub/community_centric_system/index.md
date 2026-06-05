---
name: Community-Centric System
colors:
  surface: '#f7f9fc'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#5d4038'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#926f66'
  outline-variant: '#e7bdb2'
  surface-tint: '#b12d00'
  primary: '#ad2c00'
  on-primary: '#ffffff'
  primary-container: '#d83900'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb5a0'
  secondary: '#0060a9'
  on-secondary: '#ffffff'
  secondary-container: '#4ba1fd'
  on-secondary-container: '#003663'
  tertiary: '#7c5400'
  on-tertiary: '#ffffff'
  tertiary-container: '#9d6b00'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbd1'
  primary-fixed-dim: '#ffb5a0'
  on-primary-fixed: '#3b0900'
  on-primary-fixed-variant: '#872000'
  secondary-fixed: '#d3e4ff'
  secondary-fixed-dim: '#a2c9ff'
  on-secondary-fixed: '#001c38'
  on-secondary-fixed-variant: '#004881'
  tertiary-fixed: '#ffddaf'
  tertiary-fixed-dim: '#ffba43'
  on-tertiary-fixed: '#281800'
  on-tertiary-fixed-variant: '#614000'
  background: '#f7f9fc'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: IBM Plex Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 26px
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 21px
  body-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
  label-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 16px
  label-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 12px
  margin-desktop: 24px
---

## Brand & Style

This design system is built to facilitate community, conversation, and information density. It balances a professional, systematic structure with a friendly, approachable personality. The visual identity draws inspiration from social aggregates, focusing on content-first layouts where the UI recedes to highlight user-generated media and discussions.

The style is **Modern / Corporate** with a focus on high legibility and functional clarity. It avoids excessive ornamentation in favor of clear information architecture, using white space to separate distinct "threads" of information while maintaining a high density of data. The emotional response is intended to be inviting, democratic, and reliable.

## Colors

The palette is anchored by a vibrant, energetic primary orange-red, used strictly for primary actions, branding, and highlighting active states. A deep "Action Blue" serves as the secondary color, traditionally used for links, interactive text, and secondary functional elements.

The background uses a pure white for content surfaces to maximize contrast, paired with a very light gray (`#F6F7F8`) for the application background to create a clear distinction between the "canvas" and the "content cards." Neutrals are carefully stepped to handle metadata, borders, and disabled states without cluttering the visual field.

## Typography

The design system utilizes a dual-font strategy. **Plus Jakarta Sans** is used for headlines and display text, providing a soft, modern, and friendly character to the structural headers. For the core experience—comments, post bodies, and metadata—**IBM Plex Sans** is employed for its exceptional legibility and systematic feel.

Information hierarchy is strictly enforced through weight and color rather than just size. Metadata (timestamps, usernames) should consistently use `body-sm` or `label-sm` in a neutral gray to ensure the primary content remains the focal point.

## Layout & Spacing

This design system uses a **Fluid Grid** model with a max-width container for desktop viewing to prevent line lengths from becoming unreadable. The spacing rhythm is based on a 4px baseline grid.

- **Desktop:** 12-column grid with 16px gutters. Content is typically centered in a container that caps at 1200px, though a "sidebar-main" layout (8 columns main, 4 columns sidebar) is the standard for feed views.
- **Mobile:** Single column with 12px side margins.
- **Density:** Elements like comment threads use a nested indentation logic (16px per level) to visually represent hierarchy without the need for excessive borders.

## Elevation & Depth

Hierarchy is primarily achieved through **Tonal Layers** and **Low-Contrast Outlines** rather than heavy shadows. 

- **Level 0 (Background):** Used for the app canvas (`#F6F7F8`).
- **Level 1 (Cards):** Pure white surfaces with a 1px solid border (`#EDEFF1`). On hover, these cards may lift slightly using a very soft, diffused shadow (0px 2px 4px rgba(0,0,0,0.05)).
- **Level 2 (Modals/Popovers):** Standard white surface with a more pronounced ambient shadow (0px 8px 24px rgba(0,0,0,0.12)) to separate them from the content layer.
- **Depth Cues:** Interactive elements use subtle background color shifts (e.g., a light gray hover state) instead of elevation changes to maintain a "flat" and efficient interface.

## Shapes

The shape language is defined as **Rounded**. This provides a friendly, modern feel that softens the high-density information layout.

- **Standard Elements:** Buttons, input fields, and small cards use a 0.5rem (8px) corner radius.
- **Large Containers:** Content blocks or large cards use 1rem (16px) for a more distinct, approachable look.
- **Contextual Shapes:** Search bars and specific action "pills" (like community tags) utilize a full pill-shape (circular ends) to differentiate them from square-ish content cards.

## Components

### Buttons
Primary buttons use the orange-red background with white text. Secondary buttons use a transparent background with a blue border and blue text. Tertiary buttons are "ghost" style, using blue or gray text that highlights with a light gray background on hover.

### Cards
Cards are the primary container for the design system. They feature a 1px border (`#EDEFF1`), 16px internal padding, and a white background. Top-level cards on mobile should span the full width to maximize space, while on desktop they sit within the grid.

### Chips & Tags
Used for categorization. These are small, pill-shaped elements with a light gray background (`#E3E6E8`) and bold `label-sm` text. They have a 4px horizontal gap between them.

### Input Fields
Inputs are outlined with a 1px gray border. On focus, the border transitions to the secondary blue color. Labels should be placed above the field in `label-sm` weight to maximize clarity.

### Voting Controls
A signature component. Vertically stacked icons (arrows) with a centered count. Upvote uses the primary orange-red for the active state; downvote uses a specific periwinkle blue (`#7193FF`). Counts should be bold and centered.

### Lists & Feeds
Items in a feed are separated by the background color (`#F6F7F8`) appearing as a "gutter" between Level 1 cards, rather than internal dividers, to create a clear "chunking" effect of content.