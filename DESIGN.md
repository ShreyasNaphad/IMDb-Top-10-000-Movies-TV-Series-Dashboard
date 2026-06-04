---
name: Cinematic Insights
colors:
  surface: '#0f131b'
  surface-dim: '#0f131b'
  surface-bright: '#353942'
  surface-container-lowest: '#0a0e16'
  surface-container-low: '#181c24'
  surface-container: '#1c2028'
  surface-container-high: '#262a32'
  surface-container-highest: '#31353e'
  on-surface: '#dfe2ee'
  on-surface-variant: '#d1c5ac'
  inverse-surface: '#dfe2ee'
  inverse-on-surface: '#2c3039'
  outline: '#9a9078'
  outline-variant: '#4e4633'
  surface-tint: '#f0c110'
  primary: '#ffe5a0'
  on-primary: '#3d2f00'
  primary-container: '#f5c518'
  on-primary-container: '#695200'
  inverse-primary: '#745b00'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#7dffc4'
  on-tertiary: '#003824'
  tertiary-container: '#54e3a7'
  on-tertiary-container: '#006242'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe08b'
  primary-fixed-dim: '#f0c110'
  on-primary-fixed: '#241a00'
  on-primary-fixed-variant: '#584400'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#0f131b'
  on-background: '#dfe2ee'
  surface-variant: '#31353e'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
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
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin: 24px
---

## Brand & Style

The design system is engineered for deep cinematic data analysis, catering to industry professionals, researchers, and data enthusiasts. The brand personality is **authoritative, analytical, and cinematic**, bridging the gap between high-end entertainment and rigorous data science.

The visual style is **Corporate Modern with a "Dark Mode" focus**, utilizing a layered surface architecture to manage information density. It prioritizes clarity and precision, ensuring that complex IMDb datasets are navigable and insights are immediate. The emotional response should be one of "command and control"—providing the user with a powerful, sophisticated cockpit for global film and television intelligence.

## Colors

This design system utilizes a tiered dark palette to create depth without relying on heavy shadows. 

- **Primary (IMDb Yellow):** Reserved for high-priority actions, branding, and highlighting "Winner" or "Top-Rated" status.
- **Secondary & Tertiary (Data Blue/Teal):** Used primarily for data visualization, progress indicators, and interactive states to differentiate from the core brand yellow.
- **Neutrals:** The background scale follows a strict "Deep to Light" elevation model:
  - **Deep Dark (#0B0E14):** The canvas background.
  - **Surface (#151921):** Navigation bars and sidebars.
  - **Card (#1C212B):** The primary container for data widgets.
- **Data Visualization Palette:** Beyond the accent colors, implement a Viridis-inspired scale (Deep Purple to Bright Yellow) for heatmaps and complex charts to ensure accessibility and high contrast against the dark background.

## Typography

The typography system uses **Inter** for its exceptional legibility in high-density environments. 

- **Hierarchy:** Use `headline-xl` sparingly for title-level views. `headline-md` is the standard for card titles.
- **Data Labels:** `label-md` uses uppercase with slight letter spacing to clearly delineate category headers from the data they contain.
- **Tabular Data:** For numerical values in tables, use a monospaced alternative like **JetBrains Mono** or Inter’s tabular lining features to ensure columns align perfectly for easy scanning.
- **Color Contrast:** Use `text_primary` (#FFFFFF) for headlines and critical data points. Use `text_secondary` (#94A3B8) for labels and supporting text to reduce visual noise.

## Layout & Spacing

This design system employs a **Fixed 12-Column Grid** for desktop to ensure data visualizations remain consistent and readable. 

- **Rhythm:** A 4px baseline grid governs all spacing. 
- **Density:** The layout is intentionally "tight." Gutters are fixed at 16px to maximize the horizontal space available for multi-column data tables and charts.
- **Responsive Behavior:**
  - **Desktop (1440px+):** 12 columns, 24px outer margins.
  - **Tablet (768px - 1439px):** 6 columns, 16px outer margins, cards stack vertically where necessary.
  - **Mobile (<767px):** 2 columns, 12px outer margins. Most complex charts should be replaced with simplified summary cards or horizontal scroll views.

## Elevation & Depth

In this dark-themed environment, depth is communicated through **Tonal Layering** supplemented by **Low-Contrast Outlines**.

- **Shadows:** Use extremely subtle, large-radius shadows for the top-level cards (e.g., `0 10px 15px -3px rgba(0, 0, 0, 0.5)`). Shadows should feel ambient rather than directional.
- **Borders:** Every card and input field must have a 1px border. The border color is `rgba(255, 255, 255, 0.08)`. This creates a crisp definition between surfaces that have similar hex values.
- **Interaction:** Upon hover, interactive cards should increase their border opacity to `rgba(255, 255, 255, 0.15)` and shift their background color 2% lighter.

## Shapes

The shape language is **Soft (0.25rem)**, reflecting a professional and technical aesthetic.

- **Buttons & Inputs:** Use the standard `rounded` (4px) for a precise, architectural feel.
- **Cards & Modals:** Use `rounded-lg` (8px) to provide a clear container boundary that feels modern but not overly playful.
- **Status Pills:** Use `rounded-xl` (12px) or a full pill shape for status indicators (e.g., "Trending," "Released") to distinguish them from functional buttons.

## Components

- **Cards:** The workhorse of the system. Cards use `surface_card` background, 8px corner radius, and a subtle 1px border. Padding should be 16px or 24px depending on content density.
- **Buttons:** 
  - *Primary:* IMDb Yellow with black text for maximum prominence.
  - *Secondary:* Ghost style with a `text_secondary` border and white text.
- **Inputs:** Darker than the card background (#0B0E14), 1px border, with Inter `body-md` text. The active state uses a Data Blue (#3B82F6) border glow.
- **Data Tables:** No vertical borders. Use thin horizontal dividers (`rgba(255, 255, 255, 0.05)`). Alternating row stripes (zebra striping) are encouraged for tables exceeding 10 rows.
- **Charts:** Use the Viridis scale. Axes and gridlines should be muted (`rgba(255, 255, 255, 0.1)`). Tooltips should use the `background_deep` color with a `primary_color` border.
- **Chips/Badges:** Small, high-contrast indicators for genres (e.g., "Sci-Fi", "Drama"). Use a semi-transparent fill of the primary or secondary color with 100% opacity text.