---
name: Operational Precision
colors:
  surface: '#fcf8ff'
  surface-dim: '#dcd9e0'
  surface-bright: '#fcf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f2fa'
  surface-container: '#f0ecf4'
  surface-container-high: '#eae7ef'
  surface-container-highest: '#e5e1e9'
  on-surface: '#1b1b21'
  on-surface-variant: '#474651'
  inverse-surface: '#303036'
  inverse-on-surface: '#f3eff7'
  outline: '#777682'
  outline-variant: '#c8c5d3'
  surface-tint: '#5654a8'
  primary: '#1a146b'
  on-primary: '#ffffff'
  primary-container: '#312e81'
  on-primary-container: '#9c9af4'
  inverse-primary: '#c3c0ff'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#3e1a00'
  on-tertiary: '#ffffff'
  tertiary-container: '#5f2b00'
  on-tertiary-container: '#de915e'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#100563'
  on-primary-fixed-variant: '#3e3c8f'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdbc7'
  tertiary-fixed-dim: '#ffb688'
  on-tertiary-fixed: '#311300'
  on-tertiary-fixed-variant: '#70380b'
  background: '#fcf8ff'
  on-background: '#1b1b21'
  surface-variant: '#e5e1e9'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
  mono-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding-sm: 12px
  container-padding-md: 16px
  gutter: 16px
  stack-xs: 4px
  stack-sm: 8px
  stack-md: 16px
  max-width-desktop: 1440px
---

## Brand & Style
The design system is engineered for high-stakes operational environments where clarity and speed of information processing are paramount. It follows a **Corporate Modern** aesthetic with a heavy emphasis on **Functional Minimalism**. 

The visual language prioritizes utility over ornamentation, utilizing a "data-first" approach. The interface should feel like a precision instrument: reliable, calm under pressure, and inherently structured. By reducing visual noise and focusing on rhythmic alignment, the system ensures that users can manage high-density ticket queues without cognitive fatigue. The emotional response is one of professional confidence and systematic control.

## Colors
The color palette is anchored by a deep Indigo primary, signaling authority and stability. The neutral palette is extensive, utilizing a Slate-based grayscale to provide subtle differentiation between UI layers without introducing unnecessary hue shifts.

- **Primary:** Deep Indigo (#312E81) used for primary actions, active navigation states, and brand touchpoints.
- **Secondary:** Slate (#64748B) for supportive icons and secondary text.
- **Accents:** Semantic colors are reserved strictly for status communication:
    - **Emerald:** Resolved / Success.
    - **Amber:** Pending / Warning.
    - **Rose:** Urgent / Breach / Error.
- **Neutral:** A range of Slate grays from 50 to 900. Backgrounds primarily use #F8FAFC (Slate-50) for the canvas and #FFFFFF for containers.

## Typography
This design system employs **Inter** for all UI elements to ensure maximum legibility at small sizes. The typographic scale is optimized for high-density data viewing, with tighter line-heights for body text to allow more information to fit above the fold.

For technical data points like Ticket IDs or log entries, use a monospaced font (JetBrains Mono) at 12px. Labels should be used sparingly for metadata headers, often in uppercase with slight letter-spacing to distinguish them from interactive body text.

## Layout & Spacing
The layout follows a **Fixed Grid** model for the main dashboard view, ensuring that data columns remain predictable and scannable. 

- **Base Unit:** A 4px incremental scale (4, 8, 12, 16, 24, 32).
- **Grid:** A 12-column system for desktop with 16px gutters.
- **Density:** High. Margins between ticket rows are kept to 8px or 12px to maximize visibility of the queue. 
- **Reflow:** On tablet, the sidebar collapses into an icon-only rail. On mobile, the grid collapses into a single-column stack, prioritizing the Ticket Subject and Status Badge.

## Elevation & Depth
Depth is conveyed primarily through **Tonal Layers** and **Low-contrast Outlines** rather than heavy shadows. This maintains a flat, professional profile.

- **Level 0 (Canvas):** #F8FAFC (Slate-50).
- **Level 1 (Card/Container):** White background with a 1px border (#E2E8F0).
- **Level 2 (Dropdowns/Modals):** White background, 1px border, and a subtle "Ambient Shadow" (0px 4px 6px -1px rgba(0, 0, 0, 0.05)).
- **Interactivity:** Hover states on rows or buttons should use a subtle background tint (#F1F5F9) rather than a shadow increase.

## Shapes
The shape language is **Soft** (4px / 0.25rem). This small radius provides a hint of modern approachability while maintaining the structured, architectural feel of a professional tool. 

- **Buttons & Inputs:** 4px radius.
- **Status Badges:** 4px radius (not pill-shaped) to keep them aligned with the block-based grid.
- **Cards:** 8px (rounded-lg) for outer containers to provide clear containment.

## Components
- **Buttons:** Primary buttons use the Indigo background with white text. Secondary buttons use a Slate-100 background with Slate-900 text. Use "compact" sizing (32px height) for toolbar actions.
- **Chips (Status):** Use a "Soft Tint" approach: a 10% opacity background of the semantic color with 100% opacity text of the same color (e.g., Light Emerald background with Dark Emerald text).
- **Lists (Data Tables):** Rows must have a 1px bottom border. Highlight the "Active" ticket with a 4px primary-colored left border strip.
- **Input Fields:** Use a 1px border (#CBD5E1). On focus, the border changes to Primary Indigo with a subtle 2px outer glow of the same color at 10% opacity.
- **Checkboxes:** Square with a 2px radius. When checked, use the Primary Indigo fill.
- **Cards:** Use for individual ticket details. They should be flat with a 1px border, no shadow, and consistent 16px internal padding.
- **Additional Components:** "SLA Timers" (compact countdown text with semantic color indicators) and "Activity Feed" (a vertical timeline using 1px slate lines and 8px dot indicators).