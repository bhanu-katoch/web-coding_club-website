# Design System Strategy: The Kinetic Pulse

## 1. Overview & Creative North Star
**Creative North Star: "The Kinetic Pulse"**
This design system moves away from the static, rigid structures of traditional administration portals. For a modern community club, the UI must feel like a living organism—energetic, fluid, and student-centric. We achieve this through **Organic Layering**: a philosophy where elements aren't just placed on a grid, but float and interact within a cohesive ecosystem. 

By breaking the "template" look with intentional asymmetry, oversized display type, and a focus on tonal depth over structural lines, we create an editorial experience that feels premium yet accessible. The goal is to make every interaction feel like an invitation to participate, not a task to complete.

---

## 2. Colors: Vibrancy Through Tonal Depth
We utilize a sophisticated Material 3 palette to balance "Student Energy" with "Professional Credibility."

*   **The "No-Line" Rule:** Direct 1px solid borders are strictly prohibited for sectioning. To separate content, use background shifts. A `surface-container-low` section should sit against a `surface` background to create a "natural" boundary.
*   **Surface Hierarchy & Nesting:** Treat the UI as physical layers.
    *   **Base:** `surface` (#f9f5ff)
    *   **Sectioning:** `surface-container-low` (#f3eeff)
    *   **Primary Cards:** `surface-container-lowest` (#ffffff) for maximum "lift."
*   **The "Glass & Gradient" Rule:** For floating navigation or hero highlights, use Glassmorphism. Apply `surface` at 70% opacity with a `24px` backdrop-blur. 
*   **Signature Textures:** Do not use flat `primary` colors for large CTAs. Use a linear gradient from `primary` (#2444eb) to `primary_container` (#8999ff) at a 135-degree angle to add "soul" and dimension.

---

## 3. Typography: Editorial Authority
We pair **Plus Jakarta Sans** (Display/Headlines) with **Manrope** (Body/Labels) to balance high-energy personality with technical legibility.

*   **The Power Scale:** Use `display-lg` (3.5rem) for hero statements, utilizing tight letter-spacing (-0.02em) to create a high-end editorial feel.
*   **The Informational Core:** `body-lg` (Manrope, 1rem) is the workhorse. Ensure line-height is set to 1.6 for readability in long-form community updates.
*   **Functional Labeling:** `label-md` should be used sparingly for "overlines" above headlines, set in all-caps with increased letter-spacing (+0.05em) using the `secondary` (#af2700) token to provide a "pop" of energy.

---

## 4. Elevation & Depth: Tonal Layering
Traditional shadows and borders create "visual noise." We replace them with **Ambient Elevation**.

*   **The Layering Principle:** Place `surface-container-highest` (#ddd9ff) elements behind `surface-container-lowest` (#ffffff) cards to create depth. The contrast in "warmth" and "coolness" defines the edge.
*   **Ambient Shadows:** For interactive floating elements (e.g., Modals), use a "Soft-Focus" shadow: `0 20px 40px rgba(45, 42, 81, 0.06)`. Note that the shadow color is a tinted version of `on-surface` (#2d2a51), not black.
*   **The "Ghost Border" Fallback:** If a border is required for accessibility in forms, use `outline-variant` (#aca8d7) at 20% opacity. This creates a "suggestion" of a boundary without closing off the design.

---

## 5. Components: Fluidity in Form
All components must adhere to the **Roundedness Scale**, specifically utilizing `xl` (1.5rem) for major containers to maintain the "Student-Friendly" softness.

*   **Buttons:**
    *   *Primary:* Gradient fill (Primary to Primary-Container), `full` rounding, `label-md` typography.
    *   *Tertiary:* Ghost style. No background, no border. Use `primary` text with a subtle background shift to `surface-container-high` on hover.
*   **Input Fields:** Professionalism is key here. Use `surface-container-lowest` as the field background with a `Ghost Border`. When focused, transition the border to `primary` (#2444eb) and add a 4px soft outer "glow" using the primary color at 10% opacity.
*   **Cards:** Forbid divider lines. Separate header and body content using a change in surface tone (e.g., `surface-container-low` header against a `surface-container-lowest` body) or simply through 32px of vertical whitespace.
*   **Community Chips:** Use `secondary_container` (#ffc4b6) with `on_secondary_container` (#8b1d00) text for high-visibility tags (e.g., "New Event"). Rounding must be `full`.
*   **The "Glass" Bottom Bar:** For mobile views, use a floating navigation bar with a backdrop-blur and a `surface-variant` tinted glass effect to keep the "student-modern" aesthetic.

---

## 6. Do's and Don'ts

### Do:
*   **Do** use asymmetrical layouts. Let an image overlap the boundary of a `surface-container` to break the "box" feel.
*   **Do** use `secondary` (#af2700) as an accent for "Call to Action" sparks, but keep `primary` as the dominant brand voice.
*   **Do** lean into white space. If you think it needs more space, add 16px more.

### Don't:
*   **Don't** use 100% black (#000000) for text. Use `on-surface` (#2d2a51) to keep the palette sophisticated and integrated.
*   **Don't** use `none` or `sm` rounding unless it's for tiny utilitarian icons. Everything should feel approachable (minimum `md`).
*   **Don't** use standard "Drop Shadows." If the element doesn't feel "raised" enough through tonal shifts, rethink the background hierarchy before adding a shadow.