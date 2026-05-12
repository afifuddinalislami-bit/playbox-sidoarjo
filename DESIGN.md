---
name: The Design System
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
  on-surface-variant: '#d0c2d5'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#998d9e'
  outline-variant: '#4d4353'
  surface-tint: '#e0b6ff'
  primary: '#e0b6ff'
  on-primary: '#4c007d'
  primary-container: '#9d4edd'
  on-primary-container: '#fffdff'
  inverse-primary: '#8433c4'
  secondary: '#5bd5fc'
  on-secondary: '#003543'
  secondary-container: '#00a3c8'
  on-secondary-container: '#003341'
  tertiary: '#dbb8ff'
  on-tertiary: '#441573'
  tertiary-container: '#8c61be'
  on-tertiary-container: '#fffdff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f2daff'
  primary-fixed-dim: '#e0b6ff'
  on-primary-fixed: '#2e004e'
  on-primary-fixed-variant: '#6a0baa'
  secondary-fixed: '#b7eaff'
  secondary-fixed-dim: '#5bd5fc'
  on-secondary-fixed: '#001f28'
  on-secondary-fixed-variant: '#004e61'
  tertiary-fixed: '#efdbff'
  tertiary-fixed-dim: '#dbb8ff'
  on-tertiary-fixed: '#2b0053'
  on-tertiary-fixed-variant: '#5b308c'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Montserrat
    fontSize: 72px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.1em
  code-snippet:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  container-max: 1440px
  gutter: 24px
---

## Brand & Style

The design system is engineered to evoke the high-octane, immersive atmosphere of next-generation gaming. It targets a tech-savvy audience that values performance, speed, and cutting-edge aesthetics. The brand personality is unapologetically futuristic, blending a "Neon-Noir" cyberpunk vibe with the sleek functionalism of a high-end digital cockpit.

The visual style utilizes a mix of **Cyberpunk High-Tech** and **Glassmorphism**. Surfaces are treated as digital overlays—translucent, glowing, and sharp. By leveraging high-contrast luminosity against a void-black background, the system creates a sense of infinite depth and digital precision, mirroring the experience of high-fidelity PlayStation gaming.

## Colors

The palette is anchored by a deep, "absolute zero" dark background (#0a0a0a) to ensure maximum contrast for emissive elements. The primary accent is a vibrant **Neon Purple**, used for critical actions and brand presence. **Electric Blue** serves as the secondary accent, often used for interactive states, data visualization, and secondary highlights.

Gradients should be used sparingly but effectively, transitioning between the tertiary deep purple and the vibrant primary purple to add dimension. Transparency is a functional requirement; surfaces use low-opacity white or purple tints with heavy backdrop blurs to simulate frosted glass interfaces.

## Typography

This design system utilizes a dual-font strategy to balance character with legibility. **Montserrat** is the display typeface, chosen for its geometric, urban strength. It is used exclusively for headlines and impactful hero sections, often set in heavy weights (Bold to Black) to command attention.

**Inter** serves as the functional workhorse for body copy, descriptions, and UI labels. Its neutral, systematic construction ensures high readability even at small sizes against dark backgrounds. For a "HUD" (Heads-Up Display) effect, labels should frequently use uppercase styling with increased letter spacing.

## Layout & Spacing

The layout philosophy follows a **12-column fluid grid** for desktop, collapsing to 8 columns for tablet and 4 columns for mobile. Content is housed within a maximum container width of 1440px to maintain focus.

Spacing is governed by an 8px base unit, creating a rhythmic, geometric structure. While the overall feel is spacious, interactive elements like game cards and filters use tighter "sm" and "xs" spacing to mimic the dense information architecture found in gaming dashboards. Margins and gutters remain consistent to ensure a structured, high-tech alignment across all viewports.

## Elevation & Depth

Hierarchy in the design system is achieved through **Glassmorphism** and **Luminosity** rather than traditional shadows. 

1.  **Base Layer:** The absolute dark background (#0a0a0a).
2.  **Surface Layer:** Glassmorphic cards with a 20px–40px backdrop blur and a 3% white fill.
3.  **Active Layer:** Elements on this level feature a 1px solid border using the Primary or Secondary accent colors, accompanied by a subtle outer glow (box-shadow: 0 0 15px [color]).
4.  **Floating Elements:** Interactive components like tooltips or floating action buttons utilize a higher degree of transparency and more intense glow effects to appear "projected" toward the user.

## Shapes

The shape language is strictly **Sharp-edged (0px)**. This reinforces the "hard surface" industrial feel of a high-tech console interface. No corner rounding is permitted for buttons, cards, or input fields. To add visual interest without rounding, use diagonal "clipped" corners (45-degree chamfers) on prominent buttons and header sections to enhance the cyberpunk aesthetic.

## Components

### Buttons
Buttons are sharp-edged with a 2px solid border. 
- **Primary:** Neon Purple border and text. On hover, the background fills with a subtle purple gradient, and a 20px purple outer glow is applied.
- **Secondary:** Electric Blue border and text. On hover, the border pulses with an increased glow intensity.

### Cards
Cards use a glassmorphic background. Each card is framed with a thin, 1px Neon Purple or Electric Blue border. For "Featured Games," the border should have a linear gradient stroke.

### Input Fields
Inputs are minimal, featuring only a bottom border (2px) in a muted gray. Upon focus, the border transitions to Electric Blue and emits a soft glow, with the label floating above in a condensed uppercase font.

### Interactive Elements
- **Selection Chips:** Sharp rectangles with a Ghost-style border that fills solid when selected.
- **Progress Bars:** Thin tracks with a glowing, neon-filled "loading" state.
- **HUD Badges:** Small, floating labels used for "New" or "4K Ultra HD" tags, featuring high-contrast neon text on a semi-transparent black background.