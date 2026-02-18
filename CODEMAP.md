# Let's Math! Study Buddy - Code Map & Developer Guide

**Last Updated:** 2026-02-18  
**File Version:** Study-Buddy_App.html (~10,667 lines)  
**Purpose:** Navigation guide for developers and AI agents working with this codebase

---

## 📋 Table of Contents

1. [Quick Reference](#quick-reference)
2. [Repository Structure](#repository-structure)
3. [HTML File Architecture](#html-file-architecture)
4. [Major Code Sections](#major-code-sections)
5. [JavaScript Function Reference](#javascript-function-reference)
6. [Data Structures](#data-structures)
7. [CSS Architecture](#css-architecture)
8. [Content Organization](#content-organization)
9. [Development Workflow](#development-workflow)
10. [Navigation Tips](#navigation-tips)

---

## 🚀 Quick Reference

### File Sizes & Stats
- **Study-Buddy_App.html**: 10,667 lines (main application)
- **Organized-Content-Library.md**: 1,433 lines (content source)
- **README.md**: 469 lines (user & developer documentation)
- **Total Quiz Questions**: 89 (15 legacy precalc + 35 calculus + 39 expansion)
- **Total Flashcards**: 120+ items
- **Expansion Topics**: 27 (A1-A13 precalc + B1-B14 trig)

### Key Technologies
- **Pure HTML5** - No build tools required
- **Vanilla JavaScript** (ES5-compatible)
- **CSS3** with custom properties
- **Single-Page Application** (SPA) architecture
- **No external dependencies** - completely self-contained

### Quick File Navigation
```
Repository Root
├── Study-Buddy_App.html          ← Main app (START HERE)
├── Organized-Content-Library.md  ← Content source/reference
├── README.md                      ← User documentation
├── CODEMAP.md                     ← This file (developer guide)
├── IMPLEMENTATION_SUMMARY.md      ← Development notes
├── ExpansionPlan--Complete/       ← Planning documents
│   ├── Study_App_Expansion_Plan.md
│   ├── Website-Content-Inventory.md
│   └── InstructionsForAgent.md
└── UpdatePlan/                    ← Update planning
    └── UpdatePlan-Instructions.md
```

---

## 🏗️ Repository Structure

### Core Files

#### `Study-Buddy_App.html` (10,667 lines)
The complete single-page application containing:
- All HTML markup
- Inline CSS styles (~1,800 lines)
- JavaScript code (~2,500 lines)
- Embedded content data (~6,000+ lines)

#### `Organized-Content-Library.md` (1,433 lines)
Structured content source file with uniform tagging:
- Review cards (R-ALG-01, R-TRIG-01, etc.)
- Expansion review cards (E-ALG-01, E-TRIG-01, etc.)
- Flashcards (FC-ALG-01, FC-TRIG-01, etc.)
- Quiz questions (QZ-ALG-01, QZ-CALC-01, etc.)

**Tag Schema**: Each item has HTML comment tags with:
- `id`: Unique identifier
- `course`: precalc | calculus
- `area`: algebra | trig | calculus | precalc-general
- `type`: review-card | expansion-review | flashcard | quiz
- `subtopic`: Fine-grained classification
- `tier`: 1-essential | 2-important | 3-advanced
- `code`: A1-A13 or B1-B14 (expansion items)
- `yugioh`: yes | no

#### `README.md` (469 lines)
Comprehensive documentation with:
- User guide (how to use the app)
- Developer/codebase overview
- Architecture explanation
- Content organization details

### Supporting Files

#### `IMPLEMENTATION_SUMMARY.md`
Development notes and implementation history

#### `ExpansionPlan--Complete/`
Planning documents for expanded content:
- Study_App_Expansion_Plan.md
- Website-Content-Inventory.md
- InstructionsForAgent.md

#### `UpdatePlan/`
Update planning and instructions

---

## 🎯 HTML File Architecture

### Overall Structure

The `Study-Buddy_App.html` file is organized in this order:

```
<!DOCTYPE html>
<html>
<head>
  └─ <style> CSS (lines ~7-1800)
</head>
<body>
  ├─ Sidebar Navigation (lines ~1801-1950)
  ├─ Main Container
  │  ├─ Header (lines ~1951-1980)
  │  ├─ Hero Section (lines ~1981-2010)
  │  ├─ Tab: Home (lines ~2011-2300)
  │  ├─ Tab: Directory Search (lines ~2301-2550)
  │  ├─ Tab: Review Topics (lines ~2551-4800)
  │  ├─ Tab: Unit Circle (lines ~4801-5100)
  │  ├─ Tab: Flashcards (lines ~5101-5350)
  │  └─ Tab: Quiz Mode (lines ~5351-5650)
  │
  └─ <script> JavaScript
     ├─ Content Data (lines ~5651-9400)
     │  ├─ CONTENT_INDEX_DATA (main content index)
     │  ├─ Legacy flashcard arrays
     │  └─ Quiz question pools
     ├─ Core Functions (lines ~9401-10300)
     │  ├─ Content loading
     │  ├─ Tab switching
     │  ├─ Flashcard engine
     │  ├─ Quiz system
     │  ├─ Directory search
     │  └─ Focus mode
     └─ Event Listeners & Init (lines ~10301-10667)
</script>
</body>
</html>
```

### Section Landmarks (approximate line numbers)

Use these markers to navigate the large file:

| Section | Start Line | Identifier |
|---------|------------|------------|
| **CSS Styles** | ~7 | `:root {` CSS variables |
| **Sidebar HTML** | ~1801 | `<div id="sidebar"` |
| **Home Tab** | ~2011 | `<section id="home"` |
| **Directory Tab** | ~2301 | `<section id="directory"` |
| **Review Tab** | ~2551 | `<section id="review"` |
| **Unit Circle Tab** | ~4801 | `<section id="unit-circle"` |
| **Flashcards Tab** | ~5101 | `<section id="flashcards"` |
| **Quiz Tab** | ~5351 | `<section id="quiz"` |
| **Content Data** | ~5651 | `var CONTENT_INDEX_DATA = {` |
| **Flashcard Arrays** | ~8200 | `var LEGACY_FLASHCARDS = [` |
| **Quiz Pools** | ~8800 | `var quizQuestions = [` |
| **Functions** | ~9401 | `// ===== FUNCTIONS =====` |
| **Event Listeners** | ~10301 | `// ===== EVENT LISTENERS =====` |

---

## 📦 Major Code Sections

### 1. CSS Styles (Lines ~7-1800)

#### CSS Variables (`:root`)
```css
--color-white, --color-black
--color-teal-*, --color-blue-*, etc. (color palette)
--space-8, --space-16, --space-24, --space-32 (spacing system)
--radius-base, --radius-lg, --radius-full
--shadow-sm, --shadow-md, --shadow-lg
```

#### Major CSS Blocks
- Global styles (`*, html, body`)
- Container & header
- Sidebar & navigation (`.sidebar`, `.sidebar-toggle`)
- Tab system (`.tab-content`, `.active`)
- Area cards (`.area-card`, `.area-expanded`)
- Concept cards (`.concept-card`, `.collapsible`)
- Flashcards (`.flashcard-card`, `.flipped`)
- Quiz cards (`.quiz-card`, `.quiz-choices`)
- Directory items (`.directory-item`)
- Focus mode (`.focus-mode`, `.focused`)
- Utility classes (`.area-algebra`, `.area-trig`, etc.)
- Responsive media queries

### 2. HTML Markup (Lines ~1801-5650)

#### Sidebar Navigation
```html
<div id="sidebar">
  ├─ Yu-Gi-Oh! Mode Toggle
  ├─ Navigation Menu
  │  ├─ Home
  │  ├─ Directory Search
  │  ├─ Review Topics
  │  ├─ Unit Circle
  │  ├─ Flashcards
  │  └─ Quiz Mode
  └─ Sidebar sections (expandable)
```

#### Tab: Home
- Hero section with title/image
- 4 area cards: Algebra, Trig, Calculus, Precalc General
- Each card has expandable content with topic groups

#### Tab: Directory Search
- Type selector (Review/Flashcard/Quiz)
- Filter dropdowns (Course, Area, Subtopic, Tier)
- Results container
- Reset button

#### Tab: Review Topics
- Topic dropdown selector
- Review grid with concept cards
- Collapsible cards with → indicator
- Focus mode support

#### Tab: Unit Circle
- Complete unit circle reference table
- Angles in degrees and radians
- Coordinates (cos, sin, tan)

#### Tab: Flashcards
- Flashcard display area
- Flip button
- Navigation (Previous/Next)
- Shuffle button
- Topic filter dropdown
- Card counter

#### Tab: Quiz Mode
- Quiz setup interface
- Topic filter dropdown
- Question display area
- Progress bar
- Navigation buttons
- Results display
- Quiz history section

### 3. JavaScript Data (Lines ~5651-9400)

#### CONTENT_INDEX_DATA (Lines ~5651-8100)
Main content object with structure:
```javascript
{
  items: [
    {
      id: "R-ALG-01",
      course: "precalc",
      area: "algebra",
      type: "review-card",
      subtopic: "functions-notation",
      title: "Functions and Notation",
      content: "...",
      yugioh: "no"
    },
    // ... 200+ more items
  ],
  indexByTag: {
    "course:precalc": [...],
    "area:algebra": [...],
    "type:review-card": [...],
    // ... more indexes
  },
  itemsById: {
    "R-ALG-01": {...},
    "FC-TRIG-03": {...},
    // ... all items by ID
  }
}
```

#### Legacy Flashcards (Lines ~8200-8700)
Array of 120+ flashcard objects:
```javascript
var LEGACY_FLASHCARDS = [
  { topic: "functions", q: "Question text", a: "Answer text" },
  // ...
];
```

#### Quiz Pools (Lines ~8800-9400)
Three quiz arrays:
```javascript
var quizQuestions = [/* 15 precalc questions */];
var calculusQuizPool = [/* 35 calculus questions */];
var expansionQuizPool = [/* 39 expansion questions */];
var allQuizQuestions = quizQuestions
  .concat(calculusQuizPool)
  .concat(expansionQuizPool); // 89 total
```

### 4. JavaScript Functions (Lines ~9401-10300)

See [JavaScript Function Reference](#javascript-function-reference) for complete list.

### 5. Event Listeners & Initialization (Lines ~10301-10667)

- DOMContentLoaded handler
- Sidebar toggle listeners
- Tab switching listeners
- Focus mode click handlers
- Flashcard controls
- Quiz controls
- Directory filters
- Area card interactions

---

## 🔧 JavaScript Function Reference

### Navigation & UI Control

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `switchTab(tab)` | Switch between main tabs | `tab` - Tab ID string |
| `toggleSidebar()` | Open/close navigation sidebar | None |
| `toggleSidebarSection(sectionId)` | Expand/collapse sidebar section | `sectionId` - Section identifier |
| `updateHero(activeTab)` | Show/hide hero image based on tab | `activeTab` - Current tab ID |

### Area Cards (Home Page)

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `selectArea(areaId)` | Expand an area card | `areaId` - 'algebra', 'trig', etc. |
| `deselectArea()` | Return to four-card grid | None |
| `navigateToArea(section, area)` | Jump to section with area filter | `section`, `area` |

### Content Loading

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `loadContentIndex()` | Load and process CONTENT_INDEX_DATA | None |
| `initContentIndex()` | Initialize content system | None |

### Flashcard System

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `toggleFlashcard()` | Flip card to show answer | None |
| `nextCard()` | Advance to next card | None |
| `previousCard()` | Go to previous card | None |
| `shuffleCards()` | Randomize deck order | None |
| `updateFlashcard()` | Render current card | None |
| `filterFlashcards(topicId)` | Filter cards by topic | `topicId` - Topic identifier |
| `getFilteredFlashcards()` | Get current filtered deck | None - Returns array |

### Quiz System

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `initQuiz()` | Generate new quiz (10 questions) | None |
| `renderQuestionCard()` | Display current question | None |
| `selectAnswer(idx)` | Record user's answer | `idx` - Answer index (0-3) |
| `nextQuestion()` | Advance to next question | None |
| `prevQuestion()` | Go back to previous question | None |
| `endQuizEarly()` | Finish quiz before completion | None |
| `showQuizResults()` | Display final score | None |
| `getFilteredQuizPool()` | Get filtered question pool | None - Returns array |
| `saveQuizResult(score, total, date)` | Save quiz to history | `score`, `total`, `date` |
| `getQuizHistory()` | Retrieve quiz history | None - Returns array |
| `renderQuizHistory()` | Display quiz history | None |
| `clearQuizHistory()` | Clear all quiz history | None |
| `downloadQuizPDF()` | Export quiz history as PDF | None |

### Directory Search

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `selectDirectoryType(type)` | Set search type | `type` - 'review', 'flashcard', 'quiz' |
| `applyDirectoryFilters()` | Apply dropdown filters | None |
| `resetDirectoryFilters()` | Clear all filters | None |
| `getFilteredDirectoryItems()` | Get matching items | None - Returns array |
| `renderDirectoryResults()` | Display search results | None |
| `handleDirectoryItemClick(id)` | Navigate to clicked item | `id` - Item identifier |
| `populateSubtopicFilter()` | Update subtopic dropdown | None |

### Focus Mode

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `enterFocusMode(cardEl)` | Enter full-screen card view | `cardEl` - DOM element |
| `exitFocusMode()` | Return to normal view | None |

### Yu-Gi-Oh! Mode

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `toggleYugioh()` | Toggle Yu-Gi-Oh! mode on/off | None |
| `applyYugiohVisibility()` | Update content visibility | None |
| `initYugiohToggle()` | Initialize toggle control | None |

### Content Mapping

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `findReviewCardElement(id)` | Find review card in DOM | `id` - Item identifier |
| `scrollToReviewCard(id)` | Scroll to specific review card | `id` - Item identifier |

### Utility Functions

| Function | Purpose | Key Parameters |
|----------|---------|----------------|
| `shuffleArray(array)` | Randomize array order | `array` - Array to shuffle |

---

## 📊 Data Structures

### Global State Variables

```javascript
// Flashcard State
var cardDeck = [];           // Current flashcard array
var currentCardIndex = 0;    // Current position in deck
var isFlipped = false;       // Is card showing answer?

// Quiz State
var quizState = {
  current: 0,                // Current question index
  answers: [],               // User's answers (array of indices)
  submitted: false,          // Has quiz been submitted?
  activeQuiz: []             // Current quiz questions (10 items)
};

// Filter State
var currentFlashcardFilter = null;  // Active flashcard filter
var currentQuizFilter = null;       // Active quiz filter

// Yu-Gi-Oh! Mode
var yugiohMode = false;             // Is Yu-Gi-Oh! mode active?

// Directory State
var selectedDirectoryType = null;   // 'review', 'flashcard', or 'quiz'
```

### Content Item Schema

#### Review Cards & Expansion Review
```javascript
{
  id: "R-ALG-01",           // Unique ID
  course: "precalc",        // Course level
  area: "algebra",          // Subject area
  type: "review-card",      // Content type
  subtopic: "functions",    // Fine-grained topic
  title: "Functions",       // Display title
  content: "...",           // HTML content
  yugioh: "no"             // Has Yu-Gi-Oh! content?
}
```

#### Flashcards
```javascript
{
  id: "FC-TRIG-01",
  course: "precalc",
  area: "trig",
  type: "flashcard",
  subtopic: "unit-circle",
  q: "Question text",       // Question
  a: "Answer text",         // Answer
  yugioh: "no"
}
```

#### Quiz Questions
```javascript
{
  id: "QZ-CALC-01",
  course: "calculus",
  area: "calculus",
  type: "quiz",
  subtopic: "derivatives",
  q: "Question text",       // Question
  choices: ["A", "B", "C", "D"],  // Answer choices
  correct: 2,               // Correct answer index (0-3)
  yugioh: "no"
}
```

### Expansion Topic Codes

#### A-Series: Precalculus Topics (A1-A13)
- A1: Sequences and Series
- A2: Binomial Theorem
- A3: Parametric Equations
- A4: Polar Coordinates
- A5: Vectors (2D)
- A6: Complex Numbers
- A7: Matrices (Intro)
- A8: Rational Functions (Advanced)
- A9: Conic Sections
- A10: Partial Fractions
- A11: Function Composition Deep Dive
- A12: Inverse Trig Functions
- A13: Logarithm Properties (Advanced)

#### B-Series: Trigonometry Topics (B1-B14)
- B1: Trigonometric Identities (Advanced)
- B2: Double Angle & Half Angle
- B3: Sum-to-Product & Product-to-Sum
- B4: Solving Trig Equations
- B5: Inverse Trig Functions (Extended)
- B6: Law of Sines & Cosines
- B7: Area Formulas (Trig)
- B8: Polar Form of Complex Numbers
- B9: De Moivre's Theorem
- B10: Trigonometric Substitution
- B11: Graphing Trig Functions (Advanced)
- B12: Amplitude, Period, Phase Shift
- B13: Secant, Cosecant, Cotangent
- B14: Unit Circle Applications

### Topic Registry

```javascript
var TOPICS = [
  { id: 'functions', label: 'Functions' },
  { id: 'factoring', label: 'Factoring' },
  { id: 'quadratics', label: 'Quadratics' },
  { id: 'rational-functions', label: 'Rational Functions' },
  { id: 'lines', label: 'Lines' },
  { id: 'transformations', label: 'Transformations' },
  { id: 'absolute-value', label: 'Absolute Value' },
  { id: 'exponentials', label: 'Exponentials' },
  { id: 'logs', label: 'Logarithms' },
  { id: 'unit-circle', label: 'Unit Circle' },
  { id: 'identities', label: 'Trig Identities' },
  { id: 'sinusoidal', label: 'Sinusoidal Models' },
  { id: 'quadrant-patterns', label: 'Quadrant Patterns' },
  { id: 'limits', label: 'Limits' },
  { id: 'derivatives', label: 'Derivatives' },
  { id: 'integrals', label: 'Integrals' },
  { id: 'continuity', label: 'Continuity' },
  // ... expansion topics A1-A13, B1-B14
];
```

---

## 🎨 CSS Architecture

### Color System

#### Base Colors
- `--color-white`: Pure white
- `--color-black`: Pure black
- `--color-bg`: Dark surface background
- `--color-surface`: Card/component background
- `--color-text`: Primary text color
- `--color-text-secondary`: Secondary text color
- `--color-primary`: Primary accent (teal)
- `--color-primary-hover`: Hover state
- `--color-primary-active`: Active state

#### Subject Area Colors
- **Algebra**: Purple/violet (`--color-purple-*`)
- **Trigonometry**: Blue (`--color-blue-*`)
- **Calculus**: Green (`--color-green-*`)
- **Precalc General**: Orange/amber (`--color-orange-*`)

### Spacing System
- `--space-8`: 8px (smallest)
- `--space-12`: 12px
- `--space-16`: 16px (base)
- `--space-20`: 20px
- `--space-24`: 24px
- `--space-32`: 32px
- `--space-40`: 40px (largest)

### Component Classes

#### Area-Specific Modifiers
```css
.area-algebra   /* Purple theme */
.area-trig      /* Blue theme */
.area-calculus  /* Green theme */
.area-precalc-general  /* Orange theme */
```

#### State Classes
```css
.active         /* Active tab/element */
.flipped        /* Flipped flashcard */
.selected       /* Selected answer */
.correct        /* Correct quiz answer */
.incorrect      /* Incorrect quiz answer */
.expanded       /* Expanded card */
.focused        /* Focus mode card */
.collapsed      /* Collapsed section */
```

#### Card Components
```css
.concept-card        /* Review card container */
.flashcard-card      /* Flashcard container */
.quiz-card           /* Quiz question container */
.directory-item      /* Directory result item */
.area-card           /* Home page area card */
```

### Responsive Breakpoints
- Mobile: `max-width: 768px`
- Tablet: `768px - 1024px`
- Desktop: `min-width: 1024px`

---

## 📚 Content Organization

### ID Naming Conventions

#### Prefix Codes
- `R-` = Review Card
- `E-` = Expansion Review Card
- `FC-` = Flashcard
- `QZ-` = Quiz Question

#### Area Codes
- `ALG` = Algebra
- `TRIG` = Trigonometry
- `CALC` = Calculus
- `GEN` = Precalc General

#### Examples
- `R-ALG-01`: Review Card, Algebra, #01
- `FC-TRIG-05`: Flashcard, Trigonometry, #05
- `QZ-CALC-12`: Quiz Question, Calculus, #12
- `E-ALG-A1`: Expansion Review, Algebra, Topic A1

### Content Categories

#### Core Review (15 cards)
Essential precalculus concepts for foundation building.

#### Calculus Content (35 quiz questions)
- Limits (10 questions)
- Derivatives (10 questions)
- Integrals (10 questions)
- Calculus concepts (5 questions)

#### Expansion Content (27 topics, 39 quiz questions)
- A-Series: 13 precalculus topics (19 quiz questions)
- B-Series: 14 trigonometry topics (20 quiz questions)

### Tier System (Expansion Content)

- **Tier 1 (Essential)**: Must-know topics for strong foundation
- **Tier 2 (Important)**: Commonly needed, high-value topics
- **Tier 3 (Advanced)**: Deeper dives, specialized applications

---

## 🛠️ Development Workflow

### Making Changes

#### 1. Content Updates
To add/modify content:
1. Edit `Organized-Content-Library.md` (optional - for reference)
2. Directly edit the `CONTENT_INDEX_DATA` object in `Study-Buddy_App.html`
3. Ensure proper tagging (id, course, area, type, subtopic, etc.)
4. Refresh browser to test

#### 2. Style Changes
1. Modify CSS in `<style>` section (lines ~7-1800)
2. Use existing CSS variables when possible
3. Follow naming conventions for classes
4. Test responsive behavior

#### 3. Functionality Changes
1. Locate relevant function in JavaScript section (lines ~9401-10300)
2. Make minimal, surgical changes
3. Test all affected features
4. Check browser console for errors

### Testing Checklist

- [ ] Test all 6 tabs (Home, Directory, Review, Unit Circle, Flashcards, Quiz)
- [ ] Test sidebar toggle on mobile
- [ ] Test Yu-Gi-Oh! mode toggle
- [ ] Test flashcard flip, next/previous, shuffle
- [ ] Test quiz: answer selection, navigation, results
- [ ] Test directory search with various filters
- [ ] Test focus mode enter/exit
- [ ] Test area card expansion/collapse
- [ ] Verify responsive design on mobile/tablet/desktop
- [ ] Check browser console for errors

### Browser Compatibility

**Minimum Requirements:**
- Modern browser with ES5 JavaScript support
- CSS3 support for animations and flexbox

**Tested Browsers:**
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- iOS Safari
- Chrome Mobile

### Performance Considerations

- **File Size**: ~10,667 lines is manageable for modern browsers
- **Load Time**: All content loads at once (no lazy loading)
- **No Build Process**: Direct edit and refresh workflow
- **Memory**: All content stays in memory (acceptable for this data size)

---

## 🧭 Navigation Tips

### Finding Specific Content

#### By Feature
1. **Flashcards**: Search for `function toggleFlashcard()` or `function updateFlashcard()`
2. **Quiz**: Search for `function initQuiz()` or `var quizState`
3. **Directory**: Search for `function applyDirectoryFilters()` or `selectDirectoryType`
4. **Focus Mode**: Search for `function enterFocusMode()` or `.focus-mode`
5. **Yu-Gi-Oh!**: Search for `function toggleYugioh()` or `yugiohMode`

#### By Content Type
1. **Review Cards**: Search for `CONTENT_INDEX_DATA` → look in `items` array
2. **Flashcards**: Search for `type: "flashcard"` in CONTENT_INDEX_DATA
3. **Quiz Questions**: Search for `var quizQuestions` or `calculusQuizPool`

#### By Area
1. **Algebra**: Search for `area: "algebra"` or `.area-algebra`
2. **Trig**: Search for `area: "trig"` or `.area-trig`
3. **Calculus**: Search for `area: "calculus"` or `.area-calculus`

### Using Search Effectively

**Search Patterns:**
```
function <functionName>(    # Find function definitions
var <variableName>          # Find variable declarations
id="<elementId>"            # Find HTML elements by ID
class="<className>"         # Find elements by class
<!-- tags: id:<itemId>      # Find content items in library
```

**Common Markers:**
```
// ===== SECTION NAME =====  # Major section dividers
/* COMMENT BLOCK */          # CSS section comments
<section id="             # Main tab sections
```

### Section Comments in Code

The code uses comment markers to divide sections:

```javascript
// ===== FLASHCARD FUNCTIONS =====
// ===== QUIZ FUNCTIONS =====
// ===== DIRECTORY FUNCTIONS =====
// ===== FOCUS MODE =====
// ===== YU-GI-OH MODE =====
// ===== EVENT LISTENERS =====
```

These make navigation easier in large files.

---

## 📖 Cross-Reference Guide

### Related Files

| What You Need | Look Here |
|---------------|-----------|
| **User documentation** | README.md |
| **Content source** | Organized-Content-Library.md |
| **Developer guide** | CODEMAP.md (this file) |
| **Implementation notes** | IMPLEMENTATION_SUMMARY.md |
| **Expansion planning** | ExpansionPlan--Complete/ |
| **Update planning** | UpdatePlan/ |

### Feature-to-Code Mapping

| Feature | HTML Section | JavaScript Functions | CSS Classes |
|---------|--------------|---------------------|-------------|
| **Home Page** | `<section id="home">` | `selectArea()`, `deselectArea()` | `.area-card`, `.area-expanded` |
| **Directory** | `<section id="directory">` | `applyDirectoryFilters()`, `renderDirectoryResults()` | `.directory-item`, `.directory-results` |
| **Review** | `<section id="review">` | `enterFocusMode()`, `exitFocusMode()` | `.concept-card`, `.focused` |
| **Unit Circle** | `<section id="unit-circle">` | N/A (static content) | `.unit-circle-table` |
| **Flashcards** | `<section id="flashcards">` | `toggleFlashcard()`, `nextCard()`, `shuffleCards()` | `.flashcard-card`, `.flipped` |
| **Quiz** | `<section id="quiz">` | `initQuiz()`, `renderQuestionCard()`, `showQuizResults()` | `.quiz-card`, `.quiz-progress` |
| **Sidebar** | `<div id="sidebar">` | `toggleSidebar()`, `toggleSidebarSection()` | `.sidebar`, `.sidebar-toggle` |

---

## 🚀 Quick Start for Developers

### Adding New Content

1. **Add a Review Card:**
```javascript
// In CONTENT_INDEX_DATA.items array:
{
  id: "R-ALG-XX",
  course: "precalc",
  area: "algebra",
  type: "review-card",
  subtopic: "topic-name",
  title: "Card Title",
  content: "<p>Card content HTML</p>",
  yugioh: "no"
}
```

2. **Add a Flashcard:**
```javascript
{
  id: "FC-TRIG-XX",
  course: "precalc",
  area: "trig",
  type: "flashcard",
  subtopic: "topic-name",
  q: "Question text",
  a: "Answer text",
  yugioh: "no"
}
```

3. **Add a Quiz Question:**
```javascript
// In appropriate quiz pool array:
{
  id: "QZ-CALC-XX",
  course: "calculus",
  area: "calculus",
  type: "quiz",
  subtopic: "topic-name",
  q: "Question text",
  choices: ["A", "B", "C", "D"],
  correct: 0,  // Index of correct answer
  yugioh: "no"
}
```

### Modifying Styles

1. **Change Area Colors:**
```css
/* Find area-specific color variables */
.area-algebra { --area-color: var(--color-purple-500); }
.area-trig { --area-color: var(--color-blue-500); }
/* etc. */
```

2. **Adjust Spacing:**
```css
/* Use existing spacing variables */
margin: var(--space-16);
padding: var(--space-24);
```

3. **Add New Animations:**
```css
@keyframes animationName {
  from { /* start state */ }
  to { /* end state */ }
}
```

### Adding New Features

1. **Create HTML structure** in appropriate `<section>` tag
2. **Add CSS styles** in `<style>` section
3. **Write JavaScript function** in functions section
4. **Add event listener** in initialization section
5. **Update navigation** if adding new tab

---

## 🎯 Common Tasks

### Task: Find all algebra content
**Search:** `area: "algebra"` or `area-algebra`

### Task: Modify quiz length
**Location:** Line ~9746 - `var count = Math.min(10, shuffled.length);`

### Task: Change color scheme
**Location:** Lines ~7-80 - CSS `:root` variables

### Task: Add new expansion topic
1. Add to `CONTENT_INDEX_DATA.items`
2. Add to `TOPICS` array (if needed)
3. Add to `CODE_TO_TOPIC_ID` mapping (if A## or B## code)

### Task: Update documentation
1. Edit `README.md` for user-facing changes
2. Edit `CODEMAP.md` for developer/structural changes
3. Edit `Organized-Content-Library.md` to update content source

---

## 📝 Notes for AI Agents

### When Analyzing This Codebase:

1. **The file is large but well-structured** - Use section comments and line number ranges to navigate
2. **Content is embedded** - No external API calls or data files
3. **No build process** - Direct HTML editing, no compilation needed
4. **ES5 JavaScript** - Broad browser compatibility, no modern syntax
5. **Vanilla implementation** - No frameworks (React, Vue, etc.)

### Common Patterns:

1. **Tab Switching**: CSS display property toggled via `switchTab()`
2. **Content Filtering**: Filter arrays → render to DOM
3. **State Management**: Global variables, no Redux/state library
4. **Event Handling**: Direct event listeners, no event delegation framework
5. **Styling**: Utility classes + component classes

### What to Watch For:

1. **ID uniqueness**: Ensure new content has unique IDs
2. **Tag consistency**: All content items need proper tags
3. **Filter compatibility**: New content must work with existing filters
4. **Mobile responsiveness**: Test changes on small screens
5. **Browser compatibility**: Avoid ES6+ features

---

## 🔍 Troubleshooting Guide

### Quiz not working?
- Check `quizState` object initialization
- Verify `allQuizQuestions` array has items
- Check filter function `getFilteredQuizPool()`

### Flashcards not flipping?
- Check `toggleFlashcard()` function
- Verify CSS `.flipped` class and transform
- Check `isFlipped` state variable

### Directory search returns nothing?
- Verify `selectedDirectoryType` is set
- Check `getFilteredDirectoryItems()` logic
- Verify content items have correct `type` tag

### Focus mode not working?
- Check `enterFocusMode()` function
- Verify `.focus-mode` CSS class
- **Note**: ESC key support is NOT implemented

### Sidebar won't toggle?
- Check `toggleSidebar()` function
- Verify sidebar overlay click handler
- Check mobile media queries

---

## 📄 Version History

**v1.0** (2026-02-18)
- Initial code map creation
- Documented all major sections and functions
- Added navigation guide for 10K+ line file
- Cross-referenced with README and content library

---

## 🤝 Contributing

When making changes:
1. **Maintain existing patterns** - Follow established conventions
2. **Test thoroughly** - Check all affected features
3. **Update documentation** - Keep README and CODEMAP in sync
4. **Use minimal changes** - Surgical edits, not rewrites
5. **Preserve compatibility** - Don't break existing functionality

---

**For questions or issues, refer to repository documentation or open a GitHub issue.**
