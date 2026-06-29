---
name: Unisphere Premium
colors:
  surface: '#0c1324'
  surface-dim: '#0c1324'
  surface-bright: '#33394c'
  surface-container-lowest: '#070d1f'
  surface-container-low: '#151b2d'
  surface-container: '#191f31'
  surface-container-high: '#23293c'
  surface-container-highest: '#2e3447'
  on-surface: '#dce1fb'
  on-surface-variant: '#cbc3d7'
  inverse-surface: '#dce1fb'
  inverse-on-surface: '#2a3043'
  outline: '#958ea0'
  outline-variant: '#494454'
  surface-tint: '#d0bcff'
  primary: '#d0bcff'
  on-primary: '#3c0091'
  primary-container: '#a078ff'
  on-primary-container: '#340080'
  inverse-primary: '#6d3bd7'
  secondary: '#c0c1ff'
  on-secondary: '#1000a9'
  secondary-container: '#3131c0'
  on-secondary-container: '#b0b2ff'
  tertiary: '#ffb0cd'
  on-tertiary: '#640039'
  tertiary-container: '#f751a1'
  on-tertiary-container: '#570032'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d0bcff'
  on-primary-fixed: '#23005c'
  on-primary-fixed-variant: '#5516be'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffd9e4'
  tertiary-fixed-dim: '#ffb0cd'
  on-tertiary-fixed: '#3e0022'
  on-tertiary-fixed-variant: '#8c0053'
  background: '#0c1324'
  on-background: '#dce1fb'
  surface-variant: '#2e3447'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  unit-base: 8px
---

## Brand & Style

The brand personality is sophisticated, academic, and technologically forward. It targets high-achieving students who balance academic rigor with lifestyle management, requiring an environment that feels both high-end and hyper-functional. 

The design system utilizes **Glassmorphism** as its primary visual driver. By layering translucent surfaces over deep, tonal backgrounds, the UI creates a sense of "digital depth" that feels premium and immersive. The aesthetic moves away from standard flat corporate interfaces toward a "liquid" and "luminous" experience. Expect heavy use of background blurs, subtle inner glows, and vibrant gradients that simulate light refracting through glass, perfect for a modern ecosystem spanning housing, marketplace, and finance.

## Colors

The palette is anchored in a deep **Slate 950** background, providing a canvas that allows the glass effects to pop. The primary engine is a duo of **Violet** and **Indigo**, often used as a linear gradient (from top-left to bottom-right) for primary actions and brand accents. 

- **Primary (Violet):** Used for main interactions and highlights.
- **Secondary (Indigo):** Used for supporting active states and secondary depth.
- **Tertiary (Pink/Magenta):** Used sparingly for status indicators, "hot" marketplace items, or high-urgency financial alerts.
- **Glass Effects:** Surfaces are defined by a semi-transparent slate-800/900 mix with a high backdrop-blur (minimum 12px) and a subtle 1px white border at 10% opacity to simulate the edge of a glass pane.

## Typography

This design system uses **Inter** for its legibility and neutral, systematic feel, ensuring that the complex glass visuals do not compromise readability. For technical and financial data (labels, prices, and monospaced values), **Geist** is used to provide a modern, developer-centric precision.

Headlines should utilize a tight letter-spacing to feel "locked" and authoritative. Large displays (headline-xl) should occasionally use a subtle text-shadow or a light violet-to-white gradient to maintain the luminous theme. Body text must remain high-contrast (Slate 100 or White) against the dark background for accessibility.

## Layout & Spacing

The layout follows a **Fluid Grid** philosophy with generous breathing room to support the glassmorphic aesthetic. Because glass surfaces "float," extra padding is required to prevent the UI from feeling cluttered.

- **Desktop:** 12-column grid with 24px gutters. Content is centered in a 1280px container.
- **Mobile:** 4-column grid with 16px margins. 
- **Rhythm:** All spacing (margins, padding, gaps) follows a strict 8px base unit. 
- **Layering:** Components should use a "stacked" logic where the most important interactive elements are visually "higher" (more transparent/brighter) than the background layers.

## Elevation & Depth

Hierarchy is established through **Backdrop Blurs** and **Tonal Translucency** rather than traditional black shadows.

1.  **Level 0 (Base):** Slate 950. No blur.
2.  **Level 1 (Cards/Sections):** 40% opacity Slate 900, 12px blur, 1px border (White 10%).
3.  **Level 2 (Modals/Popovers):** 60% opacity Slate 800, 24px blur, 1px border (White 20%).
4.  **Glows:** High-elevation elements (like active primary buttons) feature a diffuse "Bloom" shadow—a low-opacity violet glow (#8B5CF6 at 30% opacity) with a 20px blur radius to simulate a light source behind the glass.

## Shapes

The design system uses a **Rounded** (0.5rem base) corner language. This strikes a balance between the precision of financial tools and the approachability of a student marketplace. 

- **Standard Buttons & Inputs:** 0.5rem (8px).
- **Cards & Large Containers:** 1rem (16px).
- **Status Chips & Tags:** 3rem (Pill-shaped) to distinguish them from interactive buttons.
- **Marketplace Images:** Should always carry the `rounded-lg` (1rem) treatment to fit the container language.

## Components

- **Buttons:** 
    - **Primary:** Violet-to-Indigo gradient, white text, subtle inner-glow on hover.
    - **Secondary/Glass:** Translucent background (10% white), heavy blur, 1px border.
- **Glassmorphic Cards:** The core component. Must have `backdrop-filter: blur(12px)`, a subtle gradient stroke from top-left (White 20%) to bottom-right (White 5%), and a 40% Slate 900 fill.
- **Inputs:** Darker than the card surface (Slate 950), 1px Violet border on focus, with Geist font for numeric/financial input.
- **Chips:** Small, pill-shaped elements with semi-transparent backgrounds reflecting the category color (e.g., Green for "Available Housing," Violet for "Finance").
- **Financial Graphs:** Use glowing solid lines (Violet) with a soft gradient area fill underneath that fades into the glass surface.
- **Marketplace Listings:** Cards should use "Floating Price Tags"—small glass labels positioned in the top-right of the product image.