---
name: EstateFlow Design System
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#38393a'
  surface-container-lowest: '#0d0e0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#292a2a'
  surface-container-highest: '#343535'
  on-surface: '#e3e2e2'
  on-surface-variant: '#c7c4d7'
  inverse-surface: '#e3e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#908fa0'
  outline-variant: '#464554'
  surface-tint: '#c0c1ff'
  primary: '#c0c1ff'
  on-primary: '#1000a9'
  primary-container: '#8083ff'
  on-primary-container: '#0d0096'
  inverse-primary: '#494bd6'
  secondary: '#89ceff'
  on-secondary: '#00344d'
  secondary-container: '#00a2e6'
  on-secondary-container: '#00344e'
  tertiary: '#ffb783'
  on-tertiary: '#4f2500'
  tertiary-container: '#d97721'
  on-tertiary-container: '#452000'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#07006c'
  on-primary-fixed-variant: '#2f2ebe'
  secondary-fixed: '#c9e6ff'
  secondary-fixed-dim: '#89ceff'
  on-secondary-fixed: '#001e2f'
  on-secondary-fixed-variant: '#004c6e'
  tertiary-fixed: '#ffdcc5'
  tertiary-fixed-dim: '#ffb783'
  on-tertiary-fixed: '#301400'
  on-tertiary-fixed-variant: '#703700'
  background: '#121414'
  on-background: '#e3e2e2'
  surface-variant: '#343535'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Hanken Grotesk
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
  label-md:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  code-sm:
    fontFamily: Geist
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
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
  xl: 40px
  2xl: 64px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style
The design system is built for a high-performance property management environment, prioritizing clarity, efficiency, and a premium "Pro" feel. It draws inspiration from modern technical tools like Linear and Stripe, utilizing a **Minimalist-Corporate** hybrid style. 

The aesthetic is defined by a "Dark Mode First" philosophy, creating a focused environment that reduces eye strain for power users managing large datasets. The visual narrative relies on precision, utilizing high-contrast typography and subtle depth through glassmorphism to distinguish between management layers and actionable data. The goal is to evoke a sense of absolute control, reliability, and modern sophistication.

## Colors
This design system utilizes a monochromatic foundation with a singular, high-vibrancy Indigo accent to drive action. 

- **Primary (#6366f1):** Used exclusively for primary call-to-actions, active states, and critical paths.
- **Surface Strategy:** We use a tiered grayscale approach. The background (#0a0a0a) provides the deepest level, while surfaces (#171717) and borders (#262626) create structural separation without relying on heavy shadows.
- **Text Hierarchy:** Primary text (#fafafa) is reserved for headers and critical information. Secondary text (#a3a3a3) is used for descriptions, labels, and metadata to maintain a clean visual scan.
- **Accents:** Subtle use of secondary blue/cyan can be used for informational badges or "success" states to keep the palette dynamic.

## Typography
The typography system uses a tri-font approach to balance character with utility. 

**Hanken Grotesk** provides a sharp, contemporary feel for headlines, giving the platform a custom-branded appearance. **Inter** is the workhorse for all body copy and data entry, ensuring maximum legibility in dense tables. **Geist** is utilized for labels, badges, and technical data points, adding a subtle "developer-tool" precision to the management interface.

Maintain tight letter-spacing on headlines to emphasize the premium, high-contrast look. Use `label-md` in all-caps for section headers and table headers to create clear visual anchors.

## Layout & Spacing
This design system employs a **Fluid Grid** model with a 4px baseline rhythm. 

- **Desktop:** 12-column grid with 20px gutters. Content should be contained within a 1440px max-width for dashboards to prevent excessive eye travel.
- **Density:** While the aesthetic is minimal, property data requires high density. Use 12px padding for table cells and list items, but 24px-32px padding for container cards to provide "breathing room" around data groups.
- **Reflow:** On mobile, margins shrink to 16px. Multi-column tables must collapse into "Data Cards" to maintain readability without horizontal scrolling.

## Elevation & Depth
Elevation is communicated through **Tonal Layering** and **Glassmorphism** rather than traditional heavy shadows.

1.  **Level 0 (Base):** #0a0a0a. The foundation of the application.
2.  **Level 1 (Cards/Sidebar):** #171717 with a 1px border of #262626.
3.  **Level 2 (Modals/Popovers):** Semi-transparent #1c1c1c with a `backdrop-filter: blur(12px)`. This creates a sophisticated "glass" look that maintains context of the data underneath.
4.  **Shadows:** Use a single, ultra-diffused shadow for floating elements: `0 8px 30px rgba(0,0,0,0.5)`. Avoid shadows on flat card elements.

## Shapes
The shape language follows a "Modern Soft" approach. 

- **Standard Elements:** Buttons, inputs, and small cards use a **12px (rounded-lg)** radius.
- **Large Containers:** Main dashboard widgets and outer modal shells use a **16px (rounded-xl)** radius.
- **Interactive States:** Focus rings should have a 2px offset and use the primary indigo color with 50% opacity.

## Components
- **Buttons:** Primary buttons use a solid Indigo (#6366f1) with white text. Secondary buttons use a ghost style: a #262626 border and a subtle hover fill of #1c1c1c.
- **Cards:** Incorporate glassmorphism for top-level stats. Use a 1px border (#262626) and a very subtle linear gradient (top-left to bottom-right) from #1c1c1c to #171717.
- **Input Fields:** Background should be #0a0a0a (darker than the card surface) to create an "etched" look. Use #262626 for the border, changing to Indigo on focus.
- **Tables:** Remove vertical borders. Use horizontal dividers in #1c1c1c. The header row should use `label-md` typography with a subtle #171717 background tint.
- **Status Chips:** Use low-saturation background tints (e.g., dark emerald for "Leased", dark amber for "Pending") with high-vibrancy text to ensure accessibility without breaking the dark aesthetic.
- **Dashboards:** Use "Sparklines" (miniature charts) for property performance metrics, rendered in the primary indigo color with a subtle glow (drop-shadow) effect.