# UpdatePlan-Instructions -- ALREADY DONE

## 0. Global Renaming and Branding

### 0.1 Application Name

**Goal:** Replace all occurrences of the current app/site name with **"Let's Math!"** to maintain a single canonical brand identifier.

**Implementation details:**
- Perform a project-wide search-and-replace of the previous name with `Let's Math!` in:
  - `<title>` elements in HTML.
  - Visible headings (e.g., main site header, navbar brand text).
  - Metadata (Open Graph, Twitter cards, manifests) if present.
- Avoid replacing inside data file references (e.g., if any file paths still use the old name) unless those assets are also renamed and references updated accordingly.

**Runtime considerations:**
- Centralize the app name in a configuration constant (e.g., `APP_NAME = "Let's Math!"`) and reference it wherever possible instead of hardcoding strings to prevent future inconsistencies.


### 0.2 Site Icon

**Goal:** Replace the current icon with a calculator emoji that is unfiltered and rendered in a rounded container.

**Implementation details:**
- Use a single component or element for the icon, for example in the navbar:
  - Use the standard calculator emoji: `🧮` or `📟` (no additional color filters).
  - Wrap in a container with:
    - `border-radius: 50%` or a small radius (e.g., `8px`) for a rounded border.
    - Minimal shadow and padding to maintain clarity at small sizes.

Example CSS:
```css
.app-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 32px;
  height: 32px;
  border-radius: 50%;
  border: 1px solid #ccc;
  background-color: #fff;
  font-size: 20px;
}
```

**Runtime considerations:**
- Use a single, reusable icon component (e.g., `<AppIcon />`) to avoid duplicating DOM and styles.
- If used in a favicon or PWA manifest, generate a static PNG/SVG once and reference it via the manifest instead of dynamically rendering the emoji for those surfaces.


## 1. Layout Changes: Header, Tabs, and Hero Image

### 1.1 Remove Top Tabs Under Title

**Goal:** Simplify the top layout by removing tabs located under the site title.

**Implementation details:**
- Identify the tab container (e.g., `<ul class="nav nav-tabs">`, tab bar, or similar).
- Remove this block from the home layout and any shared layout that renders it sitewide.
- Ensure navigation routes are preserved through the new navigation bar (see homepage section) so there are no dead screens.

**Runtime considerations:**
- Avoid mounting unused tab components; ensure the tabs logic and event handlers are not instantiated to reduce unnecessary event listeners and DOM updates.


### 1.2 Insert Hero Image on Homepage

**Goal:** Insert `assets\brainCalc.jpg` above the main site content on the homepage only, and fade it out when the user navigates away from the homepage.

**Implementation details:**
- On the homepage route (e.g., `/`), render a hero image component above the main content:

```html
<div id="home-hero">
  <img src="assets/brainCalc.jpg" alt="Brain and calculator illustration" />
</div>
```

- Add a fade-out animation that triggers when:
  - The route changes away from the homepage, or
  - The user navigates to any other part of the site (review, directory, flashcards, quiz, etc.).

Example CSS:
```css
#home-hero {
  transition: opacity 300ms ease-out;
  opacity: 1;
}

#home-hero.is-hidden {
  opacity: 0;
  pointer-events: none;
}
```

**Routing / state logic:**
- Subscribe to route changes (or use a router hook).
- If `currentRoute !== "/"`, add `is-hidden` class to `#home-hero`.
- If `currentRoute === "/"`, ensure `is-hidden` is removed.

**Runtime considerations:**
- Load `brainCalc.jpg` lazily or ensure it is optimized (compressed and sized correctly) to avoid blocking initial paint.
- Avoid re-mounting the hero component on minor state changes; only toggle a CSS class for fade to minimize reflow/repaint overhead.


## 2. Content Synchronization with Organized Content Library

### 2.1 Authoritative Data Source

**Goal:** Use `Organized-Content-Library.md` as the single source of truth for all questions, answers, flashcards, explanations, and tags.

**Implementation details:**
- Parse `Organized-Content-Library.md` into a structured data format at build time or pre-processing step, producing a JSON (or similar) asset such as `contentIndex.json`.

Data model (derived from tags):
- Core fields:
  - `id`: unique string (e.g., `"FC-ALG-01"`).
  - `course`: `"precalc"` | `"calculus"`.
  - `area`: `"algebra"` | `"trig"` | `"calculus"` | `"precalc-general"`.
  - `type`: `"review-card"` | `"expansion-review"` | `"flashcard"` | `"quiz"`.
  - `subtopic`: string (e.g., `"unit-circle"`, `"limits"`).
- Optional (for expansion items):
  - `tier`: `"1-essential"` | `"2-important"` | `"3-advanced"`.
  - `code`: `"A1"–"A13"` or `"B1"–"B14"`.
  - `yugioh`: `"yes"` | `"no"`.
- Content fields:
  - `title`: human-readable title.
  - `body`: markdown or HTML content.
  - `qa`: list of question/answer pairs for flashcards and quizzes where applicable.

**Runtime considerations:**
- Do **not** parse the markdown on every page load. Parse once at build time or as a pre-deploy step to generate static JSON.
- At runtime, load `contentIndex.json` once and reuse it across pages; cache in memory or via a global store.


### 2.2 Tag Consistency Across the HTML Site

**Goal:** Ensure that all rendered content on the HTML site corresponds exactly to the categories and tags defined in `Organized-Content-Library.md`.

**Implementation details:**
- Remove hardcoded question sets and flashcard definitions in HTML/JS.
- Replace them with a dynamic rendering layer that:
  - Loads items from the content index.
  - Filters by `course`, `area`, `type`, `subtopic`, and `tier` according to the current view.
- For each rendered item, keep a data attribute for its identifier and tags to enable future cross-references and analytics:

```html
<div
  class="content-item"
  data-id="FC-ALG-01"
  data-course="precalc"
  data-area="algebra"
  data-type="flashcard"
  data-subtopic="functions-notation"
>
  <!-- rendered question/answer -->
</div>
```

**Runtime considerations:**
- Use index structures in memory for efficient filtering:
  - Build maps keyed by `(course, area, type)` at initialization to avoid repeated linear scans.
  - For the directory filters (see below), precompute tag-based indexes to support O(1) or near O(1) lookups by tag, then intersect small result sets rather than full arrays.

Example:
- Maintain an object like:
```js
const indexByTag = {
  "course:precalc": [id1, id2, ...],
  "area:trig": [...],
  "type:flashcard": [...],
  "subtopic:unit-circle": [...],
  "tier:1-essential": [...]
};
```
- When filtering, intersect arrays associated with selected tags instead of scanning the entire dataset.


## 3. New Homepage Design

### 3.1 Homepage Layout

**Goal:** Create a new homepage that focuses on the four main areas and avoids overwhelming users with all review cards at once.

**Visible sections:**
- Site header (with new name and icon).
- Navigation bar (used sitewide).
- Four clickable **area cards**:
  - Algebra
  - Trigonometry
  - Calculus
  - Precalc-General

No other review content should be shown directly on the homepage.

**Implementation details:**
- Construct four cards, each representing an `area` value:
  - `area:algebra`
  - `area:trig`
  - `area:calculus`
  - `area:precalc-general`
- Each card should have:
  - Title (e.g., “Algebra”).
  - Short description (optional).
  - On click: expansion behavior (see below).

**Runtime considerations:**
- Render area cards from a configuration array to avoid duplication:
```js
const AREA_CARDS = [
  { id: "algebra", label: "Algebra", area: "algebra" },
  { id: "trig", label: "Trigonometry", area: "trig" },
  { id: "calculus", label: "Calculus", area: "calculus" },
  { id: "precalc-general", label: "Precalc General", area: "precalc-general" }
];
```


### 3.2 Area Card Expansion and Navigation Behavior

**Goal:** When an area card is selected, it should expand to focus that area and hide the others, while providing navigation to its associated resources.

**Behavioral requirements:**
- Clicking an area card:
  - Expands the selected card (visually).
  - Hides the three non-selected cards (remove from DOM or hide with CSS).
  - Shows a **Back** button in the top-left of the content area that:
    - Returns to the previous view (the four-card layout).
    - Restores all four cards.

**Implementation details:**
- State model:
  - `selectedArea: null | "algebra" | "trig" | "calculus" | "precalc-general"`.
- Render logic:
  - If `selectedArea === null` → show all four cards.
  - If `selectedArea !== null` → show only the expanded card and the Back button.

**Back button:**
- Place above the expanded card content.
- On click:
  - Set `selectedArea = null`.

**Runtime considerations:**
- Keep the homepage in a single component with local state for `selectedArea` to avoid full route transitions when expanding/collapsing.
- When hiding non-selected cards, prefer conditional rendering over merely adding `display:none` to reduce DOM size and event overhead.


### 3.3 Directory Links Inside Expanded Area Cards

**Goal:** Each expanded area card should expose navigation into the appropriate resources for that area.

**Required links per area card:**
- Review Cards (for that area)
- Expansion Review Cards (A/B-coded items relevant to that area)
- Flashcards
- Quiz

**Implementation details:**
- Under the expanded area card, render a small directory (list or grid of links):

```html
<nav class="area-directory">
  <a href="/directory?course=precalc&area=algebra&type=review-card">
    Review Cards
  </a>
  <a href="/directory?course=precalc&area=algebra&type=expansion-review">
    Expansion Review Cards
  </a>
  <a href="/directory?course=precalc&area=algebra&type=flashcard">
    Flashcards
  </a>
  <a href="/directory?course=precalc&area=algebra&type=quiz">
    Quiz
  </a>
</nav>
```

- When clicked, each link should navigate to the **Directory** page (see Section 5) with the appropriate query parameters set so the Directory view loads with the correct filters pre-selected.

**Runtime considerations:**
- Use URL query parameters or hash-based parameters for filter preselection (e.g., `?course=precalc&area=trig&type=flashcard`).
- On the Directory page, parse these parameters once on load and initialize filter state accordingly.


## 4. Yu-Gi-Oh! Global Toggle

**Goal:** Provide a global toggle to enable/disable Yu-Gi-Oh!-related examples wherever they are available.

**Placement:**
- At the bottom of the main navigation bar (consistent across all pages).

**Behavioral requirements:**
- When toggle is **ON**:
  - All content items with `yugioh:yes` are allowed to render and appear in lists / cards / quizzes where applicable.
- When toggle is **OFF**:
  - Content tagged with `yugioh:yes` is either hidden or shown as collapsed/disabled according to UX preference, but not included in main study flows by default.
- When the toggle is hovered:
  - Display a tooltip explaining that Yu-Gi-Oh! crossovers will appear where available when this toggle is enabled.

**Implementation details:**
- Store toggle state:
  - In a global store (e.g., `uiState.yugiohEnabled`).
  - Persist to `localStorage` to survive reloads.
- Filtering logic:
  - All content queries should respect this flag:
    - If `yugiohEnabled === false`, filter out items with `yugioh === "yes"`.
- Tooltip:
  - Use `title` attribute or a custom tooltip component:
    - Text: e.g., “Show Yu-Gi-Oh! crossover examples wherever available.”

**Runtime considerations:**
- Keep the toggle purely UI-level; do not re-fetch data from the server on every change. Instead, filter items client-side based on the `yugioh` tag.
- Batch re-renders: when toggling, update the global state and let only relevant content containers re-render, avoiding unnecessary updates on unrelated components.


## 5. Directory Page (Replacement for Review Cards Page)

### 5.1 Replace “Review Cards” Page with “Directory”

**Goal:** Retire the old Review Cards page and replace it with a general Directory page that uses tag-based filtering for navigation.

**Implementation details:**
- Update routing so that:
  - `/review` (or the old Review Cards route) now renders the new Directory page.
  - If legacy routes exist, redirect them to the Directory to avoid broken links.
- Update navigation bar to label this page as “Directory”.

**Runtime considerations:**
- Do not render all content eagerly. Use initial filters or lazy loading with virtualization where necessary to maintain performance if many items are displayed.


### 5.2 Directory Filtering Functionality

**Goal:** Allow users to filter the content library by tag dimensions and navigate directly to the material they want.

**Available filters:**
- `course` (precalc, calculus)
- `area` (algebra, trig, calculus, precalc-general)
- `type` (review-card, expansion-review, flashcard, quiz)
- `subtopic` (e.g., unit-circle, domain-range, derivatives)
- `tier` (1-essential, 2-important, 3-advanced) — only for expansion content

**Implementation details:**
- UI structure:
  - A filter panel with dropdowns or multi-select controls:
    - Course: single-select.
    - Area: single-select or multi-select.
    - Type: single-select.
    - Subtopic: searchable dropdown derived from the content index.
    - Tier: single-select (`All`, 1, 2, 3).
  - A results list that shows all matching items from the content index.

- Filter logic:
  - Start from the full set of items.
  - For each selected filter dimension, narrow down the set by intersecting the precomputed index arrays (see Section 2.2).
  - Example:
    - User selects `course=precalc`, `area=trig`, `type=flashcard`:
      - Intersection of:
        - all items with `"course:precalc"`
        - all items with `"area:trig"`
        - all items with `"type:flashcard"`.

- Result entries:
  - Display:
    - Title (e.g., “E-TRIG-13 · B13. Applications of Sinusoids / Harmonic Motion”).
    - Small tag summary (course, area, type, subtopic, tier).
  - Clicking an entry:
    - Either scrolls to a dedicated detail section on the same page, or
    - Navigates to an appropriate “reader” view (e.g., `/item/{id}`) depending on your architecture.

**Runtime considerations:**
- To keep filtering efficient:
  - Prebuild tag indexes at initialization.
  - Use array intersection algorithms optimized for sorted arrays or hash sets where appropriate.
- Consider debouncing subtopic search input to avoid re-filtering on every keystroke.


## 6. Efficiency and Data Flow Summary

- **Single data source:** `Organized-Content-Library.md` → preprocessed into `contentIndex.json`.
- **Single loading point:** Load and parse `contentIndex.json` once at app startup, then pass through context or a global store.
- **Tag-driven filtering:** All views (Homepage area cards, Directory, quizzes, flashcards, Yu-Gi-Oh! toggle) operate by filtering the same in-memory index by tags.
- **Minimal DOM work:** Prefer conditional rendering and CSS transitions over dynamic DOM construction for purely visual changes (hero fade, card expansion).
- **State centralization:** Navigation-related filters (course, area, type, tier, yugioh toggle) should be controlled from a small number of well-defined state variables to simplify reasoning and prevent inconsistent views.
