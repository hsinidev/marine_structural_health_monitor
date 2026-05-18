---
name: Marine Structural Intelligence
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#383939'
  surface-container-lowest: '#0d0e0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#292a2a'
  surface-container-highest: '#343535'
  on-surface: '#e3e2e2'
  on-surface-variant: '#e4bfb1'
  inverse-surface: '#e3e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#ab8a7d'
  outline-variant: '#5b4137'
  surface-tint: '#ffb599'
  primary: '#ffb599'
  on-primary: '#5a1c00'
  primary-container: '#ff5f00'
  on-primary-container: '#531a00'
  inverse-primary: '#a63b00'
  secondary: '#c8c6c5'
  on-secondary: '#303030'
  secondary-container: '#474746'
  on-secondary-container: '#b6b5b4'
  tertiary: '#c6c6c6'
  on-tertiary: '#303030'
  tertiary-container: '#949494'
  on-tertiary-container: '#2d2d2d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbce'
  primary-fixed-dim: '#ffb599'
  on-primary-fixed: '#370e00'
  on-primary-fixed-variant: '#7f2b00'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#121414'
  on-background: '#e3e2e2'
  surface-variant: '#343535'
typography:
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  data-display:
    fontFamily: JetBrains Mono
    fontSize: 28px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: -0.05em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.2'
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
spacing:
  unit: 4px
  gutter: 16px
  margin: 24px
  panel-padding: 12px
  compact-gap: 4px
  standard-gap: 8px
---

## Brand & Style

This design system is engineered for the high-stakes environment of maritime structural monitoring. The visual language is rooted in **Industrial Precision**, prioritizing data density and immediate cognitive processing over decorative aesthetics. It draws from the functional beauty of naval engineering blueprints and bridge instrumentation.

The brand personality is authoritative, resilient, and technical. The UI must feel like a specialized tool—rugged enough for physical bridge consoles and precise enough for deep-dive engineering analysis. We utilize a **high-contrast, minimal-layering** approach to ensure legibility under harsh lighting conditions, from the midday sun on deck to the low-light environment of a night watch. 

The aesthetic avoids unnecessary depth or soft shadows, favoring thin, surgical lines and structural grids that mirror the very bulkheads and hull sections the system monitors.

## Colors

The palette is strictly functional, utilizing a deep black foundation to eliminate screen glare and maximize contrast.

- **Black & Background Deep:** Used for primary work surfaces to recede visually, allowing data to pop.
- **Graphite (Secondary):** Used for structural elements, containers, and inactive "off" states of instruments.
- **Safety Orange (Primary):** Reserved for primary actions, active highlights, and critical system statuses. It acts as the "laser pointer" of the interface.
- **Data Colors:** A specialized set of "Safety" greens and yellows are used exclusively for nominal and warning statuses, following maritime signaling standards.
- **Neutrals:** Cool-toned greys facilitate the hierarchy of non-critical data points and labels.

## Typography

Typography is treated as a telemetry stream. We utilize three distinct families to separate intent:

1.  **Hanken Grotesk:** Used for structural headings and major section titles. It provides a modern, engineered feel with high legibility.
2.  **Inter:** The workhorse for descriptive text, tooltips, and secondary UI controls where variable character widths improve reading flow.
3.  **JetBrains Mono:** The primary typeface for all numerical data, sensor readouts, and status labels. Its monospaced nature ensures that fluctuating data points do not cause layout "jitter" during high-frequency updates.

**Note:** All data-heavy labels should use the `label-caps` style to mimic stamped metal plates found in engine rooms.

## Layout & Spacing

This design system utilizes a **Rigid Modular Grid** based on 4px increments. The layout is designed for high-density information environments where vertical scrolling is minimized in favor of "single-pane-of-glass" monitoring.

- **Desktop/Console:** 12-column grid with fixed sidebars for primary vessel systems. Panels are locked into place to build muscle memory for operators.
- **Tablet/Remote:** 8-column grid. Redundant data is hidden in favor of primary structural alerts and high-level hull stress indicators.
- **Mobile:** 4-column fluid grid. Focused strictly on emergency alerts and critical status pings.

Spacing between components is kept tight (`standard-gap`) to maximize the amount of visible telemetry. Large gutters are only used to separate unrelated vessel systems (e.g., separating "Hull Stress" from "Engine Vibration").

## Elevation & Depth

Elevation is conveyed through **chromatic intensity and border weight** rather than shadows. In a marine environment, shadows create visual mud; instead, we use "Tonal Layering."

1.  **Level 0 (Base):** True Black (#000000). The void background.
2.  **Level 1 (Panels):** Graphite (#1A1A1A). Used for the containers of specific instrument clusters.
3.  **Level 2 (Active Elements):** Dark Grey (#2A2A2A). Used for buttons or inputs within a panel.

**Borders:** Use 1px solid lines for all containers. `Secondary` containers use #333333, while `Active/Alert` containers use #FF5F00. 
**Overlays:** Technical overlays (like schematics) use a 20% opacity Safety Orange fill to indicate "Active Scan" zones.

## Shapes

The shape language is **Sharp (0px)**. To maintain an industrial and rugged feel, every component—from buttons to panels—uses 90-degree corners. This maximizes screen real estate and reinforces the "machined" aesthetic. 

Small 45-degree "dog-ear" clips may be used on the corners of primary status headers to further the blueprint/technical drawing aesthetic, but standard UI containers must remain strictly rectangular.

## Components

### Buttons
- **Primary:** Solid Safety Orange background with Black monospaced text.
- **Secondary:** 1px Graphite border, no fill, Orange text on hover.
- **Ghost:** No border, Orange text, used for low-priority dashboard toggles.

### Status Indicators (Instruments)
- **Gauges:** Use thin 1px arcs or linear bars. Inactive segments are Graphite; active segments are Safety Orange or Status colors.
- **LED Indicators:** Small 8x8px squares. "Off" is a dark Graphite fill; "On" is a glowing (neon) version of the status color.

### Data Inputs
- Fields consist of a bottom-border only (1px Graphite) with a monospaced label floating above it in `label-caps`. 
- Focused state changes the bottom border to 1px Safety Orange.

### Cards & Panels
- Every panel must have a header bar containing the Title in `label-caps` and a technical ID number (e.g., `SEC_04 // HULL_VIBE`).
- Panels are separated by a 1px vertical or horizontal rule to maintain the "grid" feel.

### Lists
- High-density rows with 1px border-bottom separation. 
- Hovering a row should trigger a 10% opacity Safety Orange highlight across the entire width.