```markdown
# Design System: High-End Editorial Manufacturing

## 1. Overview & Creative North Star: "The Precision Atelier"
The Creative North Star for this design system is **"The Precision Atelier."** This concept bridges the gap between heavy industrial manufacturing and the bespoke world of luxury high-performance mobility. We are moving away from the "industrial template" look. 

Instead of rigid grids and heavy containers, we treat the digital interface as a high-end editorial spread. We break the mold through **intentional asymmetry**, where text elements may overlap high-resolution imagery, and a **high-contrast typography scale** that creates a rhythmic flow across the page. This system values the "unsaid"—leveraging expansive whitespace to signal confidence, prestige, and engineering excellence.

## 2. Colors: Tonal Depth & Signature Accents
Our palette is rooted in the contrast between the mechanical (`Deep Charcoal`) and the organic (`Soft Bone White`), stitched together by the conductive warmth of `Champagne Gold`.

*   **Primary (`#775a19` / `#c5a059`):** Our Champagne Gold. Use this for moments of high intent. It represents the "spark" of innovation.
*   **Surface Hierarchy (`Soft Bone White` Base):** We use a monochromatic layering system to define structure.
    *   `surface`: `#faf9f5` (The canvas)
    *   `surface-container-low`: `#f4f4f0` (Subtle sectioning)
    *   `surface-container-high`: `#e8e8e4` (Interactive elements)
*   **The "No-Line" Rule:** We do not use 1px solid borders to separate sections. Boundaries are defined exclusively through background shifts (e.g., a `surface-container-low` section sitting against a `surface` background). This creates a seamless, "architectural" flow.
*   **The "Glass & Gold" Rule:** For floating navigation or modal overlays, use `surface-container-lowest` at 80% opacity with a `20px` backdrop-blur. This "frosted glass" effect allows the rich imagery of manufacturing to bleed through, softening the interface.
*   **Signature Texture:** Use a subtle linear gradient from `primary` (#775a19) to `primary-container` (#c5a059) at a 45-degree angle for primary CTAs. This provides a metallic "sheen" that flat colors cannot replicate.

## 3. Typography: The Editorial Contrast
We use a "High-Low" typographic approach. High-contrast Serifs evoke the heritage of luxury mastheads, while technical Sans-Serifs provide the clarity required for manufacturing specifications.

*   **Display & Headline (Newsreader):** This is our "Editorial" voice. It should be used with generous letter-spacing (tracking: -0.02em) and displayed in large scales. It speaks of legacy and authority.
*   **Title & Body (Manrope):** This is our "Functional" voice. Modern, geometric, and highly legible. Manrope provides a technical counterpoint to the Serif, ensuring the data looks as precise as the machinery.
*   **Hierarchy as Identity:** Use `display-lg` for hero statements, but pair it immediately with a `label-md` in all-caps (tracked out to +10%) for a "curated" look.

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are forbidden. We achieve depth through the **Layering Principle**.

*   **Stacking:** A `surface-container-lowest` card placed on a `surface-container-low` background creates a natural, soft lift.
*   **Ambient Shadows:** If an element must float (e.g., a "Magnetic" button), use a shadow with a `40px` blur, 0px offset, and 5% opacity using the `on-surface` color. It should feel like an atmospheric glow, not a shadow.
*   **The "Ghost Border":** For input fields or cards where containment is strictly required for accessibility, use the `outline-variant` token at **15% opacity**. It should be felt, not seen.
*   **Sharpened Form:** Note that the `Roundedness Scale` is set to `0px`. Every element—buttons, cards, images—must have razor-sharp corners. This communicates precision engineering and "brutalist luxury."

## 5. Components: Minimalist & Tactile

### Buttons
*   **Primary:** Sharp-edged, Champagne Gold gradient background. Text is `on-primary`. 
*   **Interaction:** Use a "Magnetic" hover state where the button follows the cursor slightly within a small radius, and the label shifts +2px in the opposite direction.
*   **Secondary:** Ghost style. No background, `Ghost Border` (15% opacity), Serif text.

### Masonry Grid Layouts
*   For imagery-heavy sections (e.g., the manufacturing floor or product showcases), avoid uniform grids. Use a masonry layout with varying aspect ratios. 
*   **The "Breath" Spacing:** Use a minimum of `48px` gap between items to ensure the "Luxury Whitespace" is maintained.

### Tabbed Interfaces
*   Horizontal tabs with no background or borders. 
*   Active state is indicated by a 1px `Champagne Gold` underline that animates its width from 0% to 100% on selection.

### Form Inputs
*   Minimalist underlines only. No boxes. 
*   Floating labels in `label-sm` (Manrope) that move into position with a subtle 200ms ease-in-out transition.

### Cards & Lists
*   **Constraint:** No divider lines.
*   **Separation:** Use `surface-container` shifts or `32px` of vertical white space. In lists, use the `headline-sm` Serif for titles to create a strong visual anchor for each row.

## 6. Do’s and Don’ts

### Do:
*   **Use Asymmetry:** Place a large `display-lg` heading off-center, overlapping a high-resolution image of a vehicle component.
*   **Prioritize Imagery:** Let the photography do the heavy lifting. The UI is merely the "gallery frame."
*   **Use "Thin" Weights:** Stick to Regular or Medium weights. Avoid "Bold" or "Black" weights as they diminish the refined, luxury feel.

### Don’t:
*   **No Rounded Corners:** Never use border-radius. The identity is sharp and uncompromising.
*   **No Standard Blue/Green:** Never use default system colors for success or info states. Use tonal shifts of the brand palette.
*   **No Crowding:** If you feel you need more content, you likely need more whitespace. Increase the padding before adding more elements.
*   **No Borders:** If you are reaching for a 1px solid line to separate content, stop and use a background color shift instead.```