---
name: Cyber-Scientific Simulation Environment
colors:
  surface: '#10141a'
  surface-dim: '#10141a'
  surface-bright: '#353940'
  surface-container-lowest: '#0a0e14'
  surface-container-low: '#181c22'
  surface-container: '#1c2026'
  surface-container-high: '#262a31'
  surface-container-highest: '#31353c'
  on-surface: '#dfe2eb'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#dfe2eb'
  inverse-on-surface: '#2d3137'
  outline: '#849495'
  outline-variant: '#3a494b'
  surface-tint: '#00dbe7'
  primary: '#e1fdff'
  on-primary: '#00363a'
  primary-container: '#00f2ff'
  on-primary-container: '#006a71'
  inverse-primary: '#00696f'
  secondary: '#f5fff3'
  on-secondary: '#00391d'
  secondary-container: '#27ff97'
  on-secondary-container: '#00723f'
  tertiary: '#fff5f1'
  on-tertiary: '#4e2600'
  tertiary-container: '#ffd2b2'
  on-tertiary-container: '#934d00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#5bffa1'
  secondary-fixed-dim: '#00e383'
  on-secondary-fixed: '#00210e'
  on-secondary-fixed-variant: '#00522c'
  tertiary-fixed: '#ffdcc4'
  tertiary-fixed-dim: '#ffb77f'
  on-tertiary-fixed: '#2f1500'
  on-tertiary-fixed-variant: '#6f3900'
  background: '#10141a'
  on-background: '#dfe2eb'
  surface-variant: '#31353c'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  data-lg:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
    letterSpacing: 0.05em
  data-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.1em
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
  margin: 40px
  container-max: 1440px
---

## Brand & Style

The design system is engineered to evoke the feeling of a high-fidelity laboratory interface. It targets researchers, students, and enthusiasts who require an immersive, "ultra-realistic" environment for complex data visualization and scientific simulation. 

The aesthetic is **Cyber-Scientific**: a synthesis of high-performance computing and tactile laboratory instrumentation. It leverages **Glassmorphism** to simulate advanced lens-based displays and **High-Contrast** elements to ensure critical data remains legible against deep-space backdrops. The emotional response is one of precision, curiosity, and technological empowerment. The UI should feel like a physical "heads-up display" (HUD) layered over a digital void.

## Colors

The palette is anchored in a **Deep Space Blue** (#0A0E14) base to maximize contrast and minimize eye strain during long simulation sessions. 

- **Neon Cyan (#00F2FF)**: The primary interactive and data-stream color. It represents active energy and system "on" states.
- **Bio-Green (#00FF94)**: Reserved for biological data, health metrics, and successful operation confirmations.
- **Warning Orange (#FF8A00)**: Used exclusively for critical alerts, heat signatures, or hazardous experimental conditions.
- **Glass Surfaces**: Use semi-transparent layers of the primary surface color with a 60% opacity and a heavy backdrop blur (20px+) to create the "mesmerizing" depth required for the simulation.

## Typography

This design system utilizes a three-tier typographic hierarchy to balance readability with a technical aesthetic:

1.  **Headings (Plus Jakarta Sans)**: Used for module titles and primary navigation. The geometric clarity provides a modern, approachable entry point into complex data sets.
2.  **Body Content (Inter)**: The workhorse for descriptions, tooltips, and general interface text. It provides maximum legibility and a neutral, systematic feel.
3.  **Data & Metrics (JetBrains Mono)**: Essential for the "scientific" feel. All numerical data, code snippets, and readout labels must use this monospaced font to ensure alignment and a "machine-processed" look.

Apply subtle 1px text-shadows to Cyan headings to simulate a phosphor glow.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy suitable for a PC application, maximizing the screen real estate of 16:9 or 21:9 monitors.

- **Grid**: A 12-column grid with a 24px gutter.
- **Modules**: Information is organized into "Glass Modules." These modules should feel like physical hardware slides.
- **Safe Zones**: Maintain a 40px margin from the screen edges for HUD-style elements.
- **Rhythm**: Use a 4px base unit. All padding and margins should be multiples of 4 (8, 16, 24, 32). 
- **Density**: The simulation requires high information density. Use tighter vertical spacing for JetBrains Mono data tables compared to Inter-based descriptive text.

## Elevation & Depth

Depth is the defining characteristic of this design system. It uses a combination of **Glassmorphism** and **Realistic 3D-Shadows**.

- **Level 1 (Base)**: The Deep Space Blue background.
- **Level 2 (Panels)**: Glass panels with a 1px inner stroke (#FFFFFF at 10% opacity) and a 40px backdrop blur.
- **Level 3 (Interactive)**: Buttons and active cards feature a dual shadow: a soft, 15% opacity black drop shadow and a tight, colored glow matching the element's primary color (e.g., a 4px Cyan glow).
- **Masking**: Use subtle vignette gradients on the edges of the screen to focus the user's attention on the central simulation area.

## Shapes

The shape language is **Soft (0.25rem / 4px)**. While the overall feel is sharp and technical, pure 0px corners feel overly aggressive and "retro." A minimal radius provides a contemporary, manufactured feel, reminiscent of CNC-machined laboratory equipment.

- **Standard Elements**: 4px radius.
- **Large Container Modules**: 8px radius.
- **Data Tags/Chips**: 2px radius or chamfered (clipped) corners for a more "military-spec" look.

## Components

### Buttons
- **Primary**: Solid Cyan fill with black text. On hover, apply a high-intensity cyan outer glow.
- **Ghost**: Cyan 1px border with transparent background. Fills with 10% Cyan opacity on hover.

### Glass Cards
Every container must have a subtle top-down gradient (10% white to 0% white) to simulate light hitting the top edge of a glass pane. 

### Input Fields
Dark backgrounds (#000000 at 30% opacity) with a bottom-only 2px border in Cyan. The cursor should be a blinking block character from the JetBrains Mono set.

### Chips & Status Tags
Small, all-caps labels using JetBrains Mono. Use "Bio-Green" for "STABLE" and "Warning Orange" for "CRITICAL."

### Data Visualization (The "Mesmerizer")
Graphs and charts should use thin 1px lines. Avoid solid fills; use 5% opacity gradients for the area under curves to maintain the glass transparency across the entire UI.

### Scanners & Gauges
Include circular "loading" or "scanning" animations using segmented strokes. These act as secondary visual feedback for simulation processing.