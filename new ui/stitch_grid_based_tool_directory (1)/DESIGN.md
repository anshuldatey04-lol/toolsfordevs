---
name: Deep Space Technical
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bdc8d1'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#87929a'
  outline-variant: '#3e484f'
  surface-tint: '#7bd0ff'
  primary: '#8ed5ff'
  on-primary: '#00354a'
  primary-container: '#38bdf8'
  on-primary-container: '#004965'
  inverse-primary: '#00668a'
  secondary: '#4fdbc8'
  on-secondary: '#003731'
  secondary-container: '#04b4a2'
  on-secondary-container: '#003f38'
  tertiary: '#ffc176'
  on-tertiary: '#472a00'
  tertiary-container: '#f1a02b'
  on-tertiary-container: '#613b00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c4e7ff'
  primary-fixed-dim: '#7bd0ff'
  on-primary-fixed: '#001e2c'
  on-primary-fixed-variant: '#004c69'
  secondary-fixed: '#71f8e4'
  secondary-fixed-dim: '#4fdbc8'
  on-secondary-fixed: '#00201c'
  on-secondary-fixed-variant: '#005048'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb960'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 20px
    fontWeight: '500'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin: 32px
  container-max: 1280px
---

## Brand & Style
The design system is engineered for developer tools, technical dashboards, and high-performance SaaS environments. It evokes a sense of "precision in the dark"—a calm, focused atmosphere that reduces eye strain during long working sessions.

The style is **Geist-inspired Minimalism** with a **Technical** edge. It prioritizes information density, crisp geometry, and logical hierarchy. By utilizing deep charcoal surfaces and subtle grid-based layouts, the design system creates a professional environment that feels robust and dependable. The emotional response is one of clarity, efficiency, and quiet power.

## Colors
The palette is rooted in a "Near-Black" foundation to provide maximum contrast for technical data.

- **Primary (#38bdf8):** A vibrant sky blue used for primary actions, focus states, and active indicators.
- **Secondary (#14b8a6):** A professional teal for success states and secondary data visualizations.
- **Neutral/Background (#0a0a0a):** The base surface of the application.
- **Surface Containers:** Hierarchy is established through incremental lightness (#171717 and #262626) rather than shadows.
- **Grid Lines:** Defined at 5-8% opacity white to remain visible but non-distracting.

## Typography
The typography utilizes **Geist** for its exceptional legibility in dark environments and its technical, neutral character. For metadata, code snippets, and small labels, **JetBrains Mono** is used to reinforce the developer-centric aesthetic.

Headings should always be high-contrast white (#FFFFFF). Body text utilizes a softer gray (#A3A3A3) to maintain readability without overwhelming the user's vision. Letter spacing is slightly tightened on headings for a premium, "locked-in" look.

## Layout & Spacing
The layout follows a **Fixed Grid** model for desktop and a **Fluid** model for mobile.

- **Grid:** A 12-column system with 24px gutters.
- **Background Grid:** A persistent 20px CSS grid pattern is rendered in the background at low opacity to provide a "blueprint" feel.
- **Mobile:** Breakpoints at 640px (Mobile) and 1024px (Tablet). On mobile, side margins reduce to 16px and the grid collapses to a single column.
- **Rhythm:** All vertical spacing must be a multiple of 4px.

## Elevation & Depth
This design system avoids traditional drop shadows in favor of **Tonal Layering** and **Low-Contrast Outlines**.

- **Level 0 (Base):** #0a0a0a (The Canvas).
- **Level 1 (Cards/Panels):** #171717 with a 1px solid border of #2e2e2e.
- **Level 2 (Popovers/Modals):** #262626 with a subtle 1px border of #404040.
- **Interaction:** Hover states are indicated by increasing the border brightness or adding a primary-colored glow (0px 0px 8px) rather than increasing shadow depth.

## Shapes
Shapes are **Soft (0.25rem)**. This provides just enough curvature to feel modern and "designed" while maintaining the rigid, structural integrity required for a technical tool. 

Larger containers (Cards) use `rounded-lg` (0.5rem), while internal elements like inputs and buttons use the base `rounded` (0.25rem).

## Components
- **Buttons:** Primary buttons use a solid primary blue fill with black text for maximum punch. Secondary buttons use a transparent fill with a #2e2e2e border.
- **Inputs:** Darker than the surface (#0a0a0a) to create an "inset" feel. Borders turn primary blue on focus.
- **Chips/Tags:** Use a subtle primary-tinted background (e.g., primary at 10% opacity) with primary-colored text in JetBrains Mono.
- **Cards:** Defined by a 1px border (#2e2e2e). Header areas within cards should have a subtle bottom border to separate titles from content.
- **Lists:** Clean rows separated by 1px dividers. Hover states should highlight the entire row with a #171717 background.
- **Status Indicators:** Use small, high-saturation pips (Teal for online, Amber for warning, Red for error).