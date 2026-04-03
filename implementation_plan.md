# Implementation Plan

Overview
The goal is to implement a fully functional and visually consistent "Light Theme" as an optional alternative to the existing Dark Mode, controllable via a toggle on the navigation sidebar, ensuring all core study modes (Review Topics, Flashcards, Quiz Mode) adapt correctly.

The implementation requires defining new CSS variables for light mode colors, updating the theme toggle JavaScript logic to handle the transition smoothly, and applying these new styles across all major components defined in `LetsMath_App_v1.html`. The plan assumes that the core structure (SPA nature, data embedding) remains untouched.

[Types]
No changes to core data structures or types are required; the implementation is purely cosmetic/styling-based. However, a new set of CSS variables must be defined within the `:root` selector specifically for `.light-theme` to override dark mode defaults. These variables will define primary colors, background surfaces, and text colors suitable for high contrast in daylight conditions.

[Files]
*   **Existing file to be modified:** `LetsMath_App_v1.html`. This file must receive the new CSS definitions within the `<style>` block (specifically targeting `:root.light-theme`) and updates to the theme toggle JavaScript logic within the `<script>` section. No new files are required for this implementation phase, as all content is self-contained in the HTML/CSS/JS structure.

[Functions]
*   **Modified function:** `initThemeToggle()` (in `LetsMath_App_v1.html` script block). This function must be updated to: 1) Check for a saved 'light' theme preference and apply `.light-theme`. 2) Update the toggle button text/icon correctly when switching between dark and light modes.
*   **New logic:** A mechanism must be added or verified within the JS to ensure that all components (e.g., `.concept-card`, `.flashcard`) receive necessary CSS class toggles or variable overrides when the theme switches, beyond just updating the root variables.

[Classes]
No new classes are required; existing component classes (`.concept-card`, `.flashcard`, etc.) will be styled using the newly defined light theme CSS variables. The primary change is ensuring that the `.light-theme` class correctly overrides or complements the default dark mode styling for these components.

[Dependencies]
No external package dependencies are required; all changes are confined to modifying existing inline HTML/CSS/JS within `LetsMath_App_v1.html`.

[Testing]
The testing approach involves verifying theme consistency across all major views: 1) **Home Page**: Check that the background, card colors, and text contrast look correct in light mode. 2) **Review Topics**: Verify that `.concept-card` styling (borders, shadows, backgrounds) correctly adapts to light mode variables. 3) **Flashcards/Quiz Mode**: Confirm that the primary action elements (buttons, question boxes) maintain high readability and visual appeal when the theme is set to light. The test must confirm that toggling between dark and light modes does not break any core functionality like quiz scoring or card flipping.

[Implementation Order]
1.  Update `LetsMath_App_v1.html` CSS: Define all necessary color variables for `.light-theme` within the `:root` selector, ensuring they provide high contrast against a light background surface (e.g., `--color-bg`, `--color-surface`).
2.  Update `LetsMath_App_v1.html` CSS: Apply these new theme variables to all major components (`.concept-card`, `.flashcard`, etc.) using the appropriate selectors, ensuring they override dark mode styles when `.light-theme` is present.
3.  Update `LetsMath_App_v1.html` JS: Refactor or extend `initThemeToggle()` to manage the theme state and ensure that any component-specific initialization (like setting initial card states) respects the newly applied light theme variables immediately upon loading.