---
name: Aasha
colors:
  surface: '#f8f9ff'
  surface-dim: '#d0dbed'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e6eeff'
  surface-container-high: '#dee9fc'
  surface-container-highest: '#d9e3f6'
  on-surface: '#121c2a'
  on-surface-variant: '#42493e'
  inverse-surface: '#27313f'
  inverse-on-surface: '#eaf1ff'
  outline: '#72796e'
  outline-variant: '#c2c9bb'
  surface-tint: '#3b6934'
  primary: '#154212'
  on-primary: '#ffffff'
  primary-container: '#2d5a27'
  on-primary-container: '#9dd090'
  inverse-primary: '#a1d494'
  secondary: '#904d00'
  on-secondary: '#ffffff'
  secondary-container: '#fe932c'
  on-secondary-container: '#663500'
  tertiary: '#393a29'
  on-tertiary: '#ffffff'
  tertiary-container: '#50513f'
  on-tertiary-container: '#c3c4ac'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#bcf0ae'
  primary-fixed-dim: '#a1d494'
  on-primary-fixed: '#002201'
  on-primary-fixed-variant: '#23501e'
  secondary-fixed: '#ffdcc3'
  secondary-fixed-dim: '#ffb77d'
  on-secondary-fixed: '#2f1500'
  on-secondary-fixed-variant: '#6e3900'
  tertiary-fixed: '#e4e4cc'
  tertiary-fixed-dim: '#c8c8b0'
  on-tertiary-fixed: '#1b1d0e'
  on-tertiary-fixed-variant: '#474836'
  background: '#f8f9ff'
  on-background: '#121c2a'
  surface-variant: '#d9e3f6'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 20px
    fontWeight: '400'
    lineHeight: 30px
  body-md:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  label-lg:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: 0.01em
  button:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  touch-target-min: 56px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style
The design system is centered on the concept of "Digital Companionship." It targets elderly users in North East India, prioritizing a sense of safety, familiarity, and cultural warmth. The aesthetic rejects the cold, clinical feel of traditional medical apps in favor of a **Warm Modernism** that blends soft, organic shapes with structured clarity.

The emotional response should be one of "calm competence." Users should feel empowered, not overwhelmed. This is achieved through a minimalist interface that utilizes heavy whitespace to reduce cognitive load, paired with tactile-inspired elements that make digital interactions feel more physical and intuitive.

## Colors
The palette is derived from the natural landscapes of North East India—deep forest greens, earth-toned ambers, and soft river-stone creams. 

- **Primary (Sage Forest):** Used for primary actions and brand presence. It provides a grounding, stable foundation.
- **Secondary (Warm Amber):** Reserved for highlights, notifications, and interactive elements that require gentle attention without causing alarm.
- **Surface (Cream/Ivory):** The main background color to reduce the harsh glare of pure white screens, making it easier on aging eyes.
- **Contrast:** All text-to-background combinations must maintain a 7:1 ratio (WCAG AAA) to ensure maximum legibility for users with visual impairments.

## Typography
Legibility is the primary functional requirement of this design system. We use a dual-font approach:
1. **Plus Jakarta Sans** for headings: Its soft, rounded terminals feel approachable and modern.
2. **Atkinson Hyperlegible Next** for all body and UI text: This font is specifically designed to increase character recognition and reduce misreading for users with low vision.

**Key Rules:**
- Never use a font size smaller than 18px.
- Use generous line heights (minimum 1.5x) to prevent lines of text from "blurring" together.
- Maintain high weight contrast between headings and body text to clearly signal hierarchy.

## Layout & Spacing
The layout follows a **Fixed-Fluid Hybrid** model. On mobile, elements span the full width minus safe margins to maximize touch surface area. On larger screens, content is constrained to a central column to prevent long line lengths that are difficult for elderly users to track.

**Spacing Philosophy:**
- **The 56px Rule:** No interactive element (button, link, checkbox) should have a touch target smaller than 56x56px.
- **Isolation:** Use "stack-lg" (48px) spacing between unrelated functional groups to prevent accidental taps.
- **Margins:** Generous outer margins (20px+) ensure that the user's thumb does not accidentally trigger edge-swipes or interact with the bezel.

## Elevation & Depth
To aid cognitive processing, the design system uses **Tonal Layering** rather than complex shadows. 

- **Level 0 (Base):** The Cream background.
- **Level 1 (Cards):** Pure white surfaces with a very soft, 1px "Sage" border (10% opacity). This creates a clear container for information without the visual "noise" of heavy shadows.
- **Active State:** When a user interacts with an element, it should "depress" (scale down slightly) or change to a solid fill color, providing immediate tactile-like feedback.
- **Avoid:** Glassmorphism and complex blurs, as these can be confusing for users with cataracts or light sensitivity.

## Shapes
The shape language is organic and friendly. We avoid sharp corners, which can feel aggressive or "technical." 

- **Standard Elements:** Buttons and input fields use a 0.5rem (8px) radius.
- **Containers:** Large cards and informational blocks use a 1rem (16px) radius to create a soft, welcoming frame.
- **Selection Indicators:** Use pill-shapes for active states in navigation to clearly distinguish them from static content containers.

## Components

### Buttons
- **Primary:** Solid Sage Green with White text. Minimum height 56px.
- **Secondary:** Outlined Sage Green (2px stroke). 
- **Action Feedback:** Every button press must trigger a clear visual change (fill color shift) to confirm the intent.

### Input Fields
- Use large, 20px text labels placed *above* the field, never as placeholder text.
- Border stroke increases to 3px when focused, using the Warm Amber color to draw the eye.

### Cards
- Used to group related information (e.g., "Morning Medicine").
- Cards should be tappable as a whole unit if they lead to a detail page, avoiding small "chevron" icons as the sole interaction point.

### Lists
- Vertical lists only. Avoid horizontal scrolling, which can be physically difficult for some users.
- Each list item must be separated by a clear horizontal divider or generous whitespace.

### Large-Scale Navigation
- Use a bottom navigation bar with large icons and accompanying text labels. Icons alone are insufficient for this demographic; they must always be paired with a label in a 1:1 ratio of importance.