---
name: Blueprint Developer Core
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#4c4546'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#7e7576'
  outline-variant: '#cfc4c5'
  surface-tint: '#5e5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1b1b1b'
  on-primary-container: '#848484'
  inverse-primary: '#c6c6c6'
  secondary: '#5e5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2e2e2'
  on-secondary-container: '#646464'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1b1b1b'
  on-tertiary-container: '#848484'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c6'
  on-secondary-fixed: '#1b1b1b'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '700'
    lineHeight: '1.2'
  tool-name:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '700'
    lineHeight: '1.4'
  category-label:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.6'
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  grid-unit: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  container-max: 1200px
---

## Brand & Style

The brand personality is **utilitarian, precise, and systematic**. This design system is built for high-velocity developer workflows where clarity is the highest priority. It targets software engineers and technical professionals who value efficiency over decorative flair.

The design style is a blend of **Minimalism** and **Technical Modernism**. It leverages a structural grid aesthetic—reminiscent of architectural blueprints or engineering paper—to provide a sense of mathematical order. The interface avoids "playful" elements like emojis or soft gradients, instead using high-contrast typography and intentional color-coding to guide the user's eye. The emotional response should be one of confidence, reliability, and focus.

## Colors

The palette is strictly functional. The base is a pure white background to maintain maximum readability. A **subtle grid overlay** (rendered at 8-10% opacity, though conceptually referred to as 40% density) provides the structural foundation.

- **Primary:** Black (#000000) is used for all core UI actions and primary text to ensure maximum contrast.
- **Accent Palette:** Specific professional hues are assigned to tool categories. These are not used for decoration but as functional wayfinding markers (e.g., a slim 4px border or a badge background). 
- **Grayscale:** Soft grays are reserved for borders and secondary metadata. No emojis are permitted; icons should be monochromatic or use the category's accent color.

## Typography

This system uses **Hanken Grotesk** for all primary interface elements to provide a sharp, contemporary feel that avoids the "commonplace" look of system fonts while maintaining high legibility. 

- **Hierarchy:** Tool names and category labels use high-contrast weights (700-800).
- **Secondary Monospace:** While the prompt avoids "byte-coded" primary styles, **JetBrains Mono** is used sparingly for labels and technical data to reinforce the developer context.
- **Scale:** Headlines scale aggressively. On mobile, the XL headline reduces to 28px to maintain layout integrity.

## Layout & Spacing

The layout follows a **8px square grid system** that aligns perfectly with the visual grid overlay. 

- **Model:** A fluid grid that transitions to a fixed max-width of 1200px on large displays.
- **Grid Layout:** Tools are organized in a responsive card grid. 
  - **Desktop:** 3 or 4 columns.
  - **Tablet:** 2 columns.
  - **Mobile:** 1 column.
- **Rhythm:** Vertical rhythm is strictly enforced in 8px increments. Gutters are fixed at 24px to provide ample "air" between functional zones, preventing the interface from feeling cluttered despite the dense information.

## Elevation & Depth

Depth is conveyed through **Low-contrast outlines** rather than shadows. This maintains the "blueprint" aesthetic.

- **Surface Levels:** All tool cards sit on the base white background. 
- **Borders:** Instead of shadows, cards use a 1px solid border (#E0E0E0).
- **Interaction:** On hover, a card does not lift; instead, its border color changes to the category's accent color, and the background may shift to a 2% opacity tint of that accent.
- **Overlay:** Only modal dialogs or search dropdowns use a subtle, crisp 4px shadow to indicate temporary placement above the grid.

## Shapes

The design uses **Soft (0.25rem)** roundedness. This provides a professional balance—sharp enough to feel technical and precise, but with a slight corner radius to feel modern and "finished."

- **Cards:** Use `rounded-lg` (0.5rem) to differentiate the container from the smaller internal elements.
- **Inputs/Buttons:** Use the base `rounded` (0.25rem) for a tighter, more tool-like appearance.
- **Pills:** Not used. All tags and category badges remain rectangular with minimal corner rounding.

## Components

- **Tool Cards:** The core component. Features a category accent bar at the top (4px height), followed by a monochromatic icon, the tool name in high-contrast weight, and a short description. A "pinned" or "favorite" indicator is a simple stroke star.
- **Category Headers:** Large, all-caps labels using the monospace font. They sit directly on the grid lines.
- **Input Fields:** Flat design. 1px gray border that turns black on focus. No inner shadows. Labels are placed above the field in the category-label style.
- **Buttons:** 
  - **Primary:** Solid black background with white text.
  - **Secondary:** Transparent with a 1px black border.
- **Grid Overlay:** A persistent background element. It should be implemented as a CSS pattern rather than an image to ensure it scales perfectly with the 8px spacing system.
- **Search Bar:** A wide, prominent field at the top of the layout, using a slightly larger font size for immediate accessibility.