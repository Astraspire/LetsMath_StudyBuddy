# Let's Math!

An interactive web application for mastering precalculus and calculus concepts through multiple study modes: review cards, flashcards, quizzes, and comprehensive content search.

---

## ⬇️ How to Download the App from GitHub

You don't need to install anything — just download the HTML file and open it in your browser!

1. Go to the repository page on GitHub: [https://github.com/Astraspire/LetsMath_StudyBuddy](https://github.com/Astraspire/LetsMath_StudyBuddy)
2. Click on the file **`LetsMath_App_v1.html`** in the file list.
3. On the file page, click the **"Download raw file"** button (or press the download icon ⬇️ in the top-right of the file view).
4. Save the file anywhere on your computer.
5. Open the saved file in any modern web browser (Chrome, Firefox, Safari, Edge) — no internet connection needed after downloading!

> **Tip:** If you right-click the file link and choose "Save link as…", you can save it directly.

---

## 📚 Table of Contents

1. [How to Download the App](#️-how-to-download-the-app-from-github)
2. [Recent Changes](#-recent-changes)
3. [How to Use the App](#-how-to-use-the-app)
   - [Getting Started](#getting-started)
   - [Navigation](#navigation)
   - [Study Modes](#study-modes)
   - [Special Features](#special-features)
4. [Codebase Overview](#-codebase-overview)
   - [Project Structure](#project-structure)
   - [Architecture](#architecture)
   - [Content Organization](#content-organization)
   - [Key Components](#key-components)

---

## 🆕 Recent Changes

### v1 Release
- **File renamed** to `LetsMath_App_v1.html` to mark the first stable version.
- **Tier System added** to all 21 core review cards (R-*):
  - **Tier 1 – Essential** (17 cards): Absolute must-know foundations (unit circle, function notation, derivative/integral basics, fundamental identities, etc.)
  - **Tier 2 – Important** (4 cards): High-value topics that are commonly needed (rationalizing denominators, absolute value/piecewise functions, solving inequalities, sequences & series)
  - **Tier 3 – Advanced**: Used only for expansion content (E-* cards)
- **Tiered tag format** standardized across all content items (id → course → area → type → subtopic → yugioh → tier → code)
- **Tier filter** in Directory Search lets you browse content by tier level
- **Tier badges** displayed on review cards in the app
- **Quiz Results Panel** added: after completing a quiz, an expandable/collapsible panel shows a per-question breakdown with correct/incorrect/skipped indicators
- **Topic tags** on quiz results and history: clickable area and subtopic tags link directly to the matching review card
- **Quiz History** enhancements: per-item deletion (🗑 trash icon), "Clear All" button, and CSV export
- **PDF Export** for quiz results
- **Full Results Panel** defaults to collapsed; click "📋 View Full Results" to expand
- **89+ quiz questions** across all topic areas
- **141 flashcard Q/A pairs** across 47 flashcard items

---

## 🚀 How to Use the App

### Getting Started

1. **Open the App**: Simply open `LetsMath_App_v1.html` in any modern web browser (Chrome, Firefox, Safari, Edge).
2. **No Installation Required**: This is a self-contained single-page application - no server or dependencies needed.
3. **Works Offline**: Once loaded, the app works completely offline.

### Navigation

#### App Title
- **Click "Let's Math!"**: Clicking the app title at the top navigates back to the Home tab from any section.

#### Sidebar Menu
- **Toggle Sidebar**: Click the hamburger menu (☰) in the top-left corner to open/close the navigation sidebar
- **Quick Access**: Sidebar provides instant access to all major sections:
  - 🏠 **Home** - Landing page with subject area cards
  - 📂 **Directory Search** - Advanced content filtering and search
  - 📖 **Review Topics** - In-depth concept explanations
  - 🔄 **Unit Circle** - Comprehensive unit circle reference
  - 🎴 **Flashcards** - Interactive study cards
  - ❓ **Quiz Mode** - Test your knowledge

#### Yu-Gi-Oh! Mode Toggle
Located in the sidebar, this toggle enables/disables Yu-Gi-Oh! themed crossover examples integrated throughout the content. Cards with Yu-Gi-Oh! content are specially tagged and can be filtered.

---

### Study Modes

#### 1. 🏠 Home Page

The home page features **four subject area cards**:
- **Algebra** - Functions, polynomials, exponentials, logarithms
- **Trigonometry** - Unit circle, identities, graphs, applications
- **Calculus** - Limits, derivatives, integrals (preview/core concepts)
- **Precalc General** - Mixed topics and foundational concepts

**How to Use:**
- Click any area card to expand it and see topic categories
- Each expanded view shows topic groups with quick-access buttons
- Use buttons like "Review It", "Flashcards", or "Quiz Me" to jump directly to filtered content for that area
- Click "← Back to Areas" to return to the four-card view

#### 2. 📂 Directory Search

A powerful content browser that lets you find exactly what you need.

**Search Interface:**
1. **Select Content Type** (required first step):
   - Review Cards - Detailed concept explanations
   - Flashcards - Quick study cards (Q&A format)
   - Quiz - Practice questions

2. **Apply Filters** (optional):
   - **Course**: Precalc or Calculus
   - **Area**: Algebra, Trig, Calculus, Precalc-General
   - **Subtopic**: Fine-grained topics (e.g., "unit-circle", "exponentials")
   - **Tier**: For review and expansion content - 1-essential, 2-important, 3-advanced

3. **View Results**:
   - Results show as colored cards with tags
   - Result count displayed at top
   - Click any item to navigate directly to that content

**Pro Tip**: Start broad (just select type), then narrow with filters as needed.

#### 3. 📖 Review Topics

Comprehensive concept cards with detailed explanations, formulas, and examples.

**Features:**
- **Area Filter Dropdown**: Filter review cards by major section:
  - Algebra Review — shows all algebra, exponentials/logs, and expanded precalc cards
  - Trigonometry Review — shows all trig and expanded trig cards
  - Calculus Review — shows all calculus cards
  - Precalc General — shows sequences, limits preview, common mistakes, calculator skills
  - All Topics (default) — shows every card
- **Focus Mode**: Click any concept card to enter full-screen focus mode
  - Exit with the "← Back to all topics" button
  - Minimizes distractions for deep study
- **Color-Coded Cards**: Each subject area has a distinct color scheme
- **Rich Content**: Includes formulas, tables, graphs, and step-by-step explanations
- **Yu-Gi-Oh! Integration**: 31+ topics include optional Yu-Gi-Oh! themed analogies

**Topics Include:**
- Core Review: Functions, Factoring, Quadratics, Rational Functions, Lines, Transformations, etc.
- Trig Review: Unit Circle, Identities, Sinusoidal Models, Quadrant Patterns
- Calculus Preview: Limits, Derivatives, Integrals, Continuity
- Calculus Core: Critical Points, Inflection Points, MVT, Rolle's Theorem
- Expansion Topics: 27 advanced topics (A1-A13 precalc, B1-B14 trig)

#### 4. 🔄 Unit Circle

A dedicated, comprehensive reference for the unit circle.

**Contents:**
- Complete table of all key angles (0° to 360°)
- Degree and radian measures
- Coordinates (cos θ, sin θ, tan θ) for each angle
- Quadrant identification
- Conversion formulas
- Highlighted key angles (30°, 45°, 60°, 90°)

**Use Case**: Perfect for quick reference during problem-solving or memorization practice.

#### 5. 🎴 Flashcards

Interactive study cards with question/answer flip functionality.

**Controls:**
- **Click Card** or **"Flip Card" button** - Reveal the answer
- **Next/Previous arrows** - Navigate through the deck
- **"🔀 Shuffle Cards"** - Randomize the deck order
- **Topic Filter** - Dropdown to filter by topic group:
  - Core Review (essential precalc/trig cards)
  - All Calculus (calculus cards)
  - Expanded Precalc (advanced precalc cards)
  - Expanded Trig (advanced trig cards)

**Card Display:**
- 141 total flashcard Q/A pairs across 47 flashcard items
- Current position shown (e.g., "3 / 15")
- Cards automatically filtered based on Yu-Gi-Oh! mode
- Smooth flip animation
- Large, readable text

**Study Tips:**
- Start with "Core Review" for fundamentals
- Use shuffle to prevent memorizing order
- Try to answer before flipping
- Repeat until you can answer all cards confidently

#### 6. ❓ Quiz Mode

Test your knowledge with multiple-choice quizzes.

**How It Works:**
1. **Select Topic** (optional): Choose from Core Review, Calculus, Expanded Precalc, or Expanded Trig
2. **Quiz Generation**: App randomly selects 10 questions (or fewer if pool is small)
3. **Answer Questions**: Click your answer choice
4. **Navigate**: Use "Next →" and "← Previous" buttons
5. **Review**: Questions are automatically checked when you move forward
6. **Score**: See your final results at the end

**Features:**
- **Progress Bar**: Visual progress indicator at top
- **Immediate Feedback**: Correct answers shown in green, incorrect in red
- **Question Counter**: "Question X of 10"
- **End Quiz Early**: Button to finish and see results before completing all questions
- **Retry**: Start a new quiz at any time
- **Full Results Panel**: After quiz completion, an expandable/collapsible panel shows per-question breakdown:
  - Question text with all options listed
  - Correct answer highlighted green, wrong answers struck through in red
  - Skipped questions marked with gray indicator
  - **Topic tags** below each question showing area (e.g., "Algebra") and clickable subtopic
  - Clicking a subtopic tag navigates to the matching review card in the Review Topics tab with a brief highlight
  - Defaults to collapsed; click "📋 View Full Results" to expand
- **PDF Export**: Download a PDF of your quiz results (includes topic tags)
- **Quiz History**: Past quiz attempts saved to localStorage with score, date, and percentage
  - **Topic tags** displayed below each history entry showing areas and clickable subtopics covered
  - Per-item deletion via 🗑 trash icon on each history row
  - "Clear All" button to reset entire history
  - CSV export of all quiz results (includes per-question area, subtopic, and result)

**Quiz Pool**: 89+ total questions across all topics

---

### Special Features

#### Focus Mode
- Click any review card to enter full-screen focus mode
- Large, center-aligned content for deep study
- Click "← Back to all topics" button to exit focus mode
- Exiting focus mode resets any active area filter

#### Yu-Gi-Oh! Mode
- Toggle in sidebar to show/hide Yu-Gi-Oh! themed content
- Integrates trading card game examples with math concepts
- Specially tagged cards throughout flashcards and quizzes
- All content remains educational and relevant to the math topics

#### Color-Coded System
- **Algebra**: Teal/cyan theme
- **Trigonometry**: Purple theme  
- **Calculus**: Green theme
- **Precalc-General**: Orange/amber theme
- **Mixed/Neutral**: Slate gray

#### Responsive Design
- Works on desktop, tablet, and mobile devices
- Touch-friendly interface
- Collapsible sidebar for mobile
- Optimized text sizing for readability

#### Cross-Tab Synchronization
When you navigate to a specific topic in one mode, the app remembers it when you switch to other modes. For example, selecting a trigonometry topic in Review will automatically filter to trig content when you switch to Flashcards or Quiz.

---

## 🧑‍💻 Codebase Overview

### Project Structure

```
LetsMath_StudyBuddy/
├── LetsMath_App_v1.html                 # Main application (single-page app)
├── Organized-Content-Library.md            # Content source with structured tagging (includes tier tags)
├── Updated-Organized-Content-Library.md    # Updated content library with tier assignments
├── README.md                               # This file (user & developer documentation)
├── CODEMAP.md                              # Code map & developer navigation guide
├── Implementation-Summary.md               # Development notes and tier assignment summary
├── TieredTag_DisplayFormat_UpdateInstructions.md  # Update instructions for tiered tag system
├── ExpansionPlan--Complete/                # Planning documents for expanded content
└── UpdatePlan/                             # Update planning documents
```

### Architecture

**Single-Page Application (SPA)**
- Everything is contained in one HTML file: `LetsMath_App_v1.html`
- No external dependencies (no npm, no build process)
- Self-contained: all CSS and JavaScript inline
- Data embedded as JavaScript object literals

**Technology Stack:**
- Pure HTML5
- Vanilla JavaScript (ES5-compatible for broad browser support)
- CSS3 with custom properties (CSS variables)
- No frameworks or libraries

### Content Organization

#### Content Index Structure
All content is organized in a unified `CONTENT_INDEX_DATA` object:

```javascript
{
  "items": [array of content objects],
  "indexByTag": {tag-based lookup maps},
  "itemsById": {id-based lookup map}
}
```

#### Content Item Schema
Each content item has these properties:
- `id`: Unique identifier (e.g., "R-ALG-01", "FC-TRIG-03", "QZ-CALC-07")
- `course`: "precalc" or "calculus"
- `area`: "algebra", "trig", "calculus", or "precalc-general"
- `type`: "review-card", "expansion-review", "flashcard", or "quiz"
- `subtopic`: Fine-grained classification (e.g., "functions-domain-range", "factoring-patterns")
- `tier`: "1-essential", "2-important", or "3-advanced" (for review cards and expansion content)
- `code`: A1-A13 or B1-B14 (for expansion topics)
- `yugioh`: "yes" or "no" (Yu-Gi-Oh! crossover availability)
- `title`: Display title
- `body`: The actual content text
- `qa`: Array of `{q, a}` pairs (for flashcards)
- `questions`: Array of `{q, opts, ans}` objects (for quiz items)

#### ID Format Convention
- `R-{AREA}-{##}` - Review Cards
- `E-{AREA}-{##}` - Expansion Review Cards
- `FC-{AREA}-{##}` - Flashcards
- `QZ-{AREA}-{##}` - Quiz Questions

Where `{AREA}` is:
- `ALG` = algebra
- `TRIG` = trigonometry
- `CALC` = calculus
- `GEN` = precalc-general

### Key Components

#### 1. Navigation System
- **Tab Switching**: `switchTab(tab)` - Controls which section is visible
- **Sidebar Toggle**: `toggleSidebar()` - Opens/closes navigation sidebar
- **Hero Management**: `updateHero(activeTab)` - Fades hero image in/out
- **Title Navigation**: Clicking the "Let's Math!" title (`#app-title`) calls `switchTab('home')`
- **Review Area Filter**: `filterReviewByArea(area)` - Shows/hides review cards by major area using `REVIEW_AREA_MAP`

#### 2. Flashcard Engine
```javascript
// Core functions:
toggleFlashcard()  // Flips card to show answer
nextCard()         // Advances to next card
previousCard()     // Goes to previous card
shuffleCards()     // Randomizes deck
updateFlashcard()  // Renders current card
```

- Card state managed by: `currentCardIndex`, `isFlipped`, `cardDeck`
- Filtering: `filterFlashcards(topicId)` and `getFilteredFlashcards()`

#### 3. Quiz System
```javascript
// Core functions:
initQuiz()            // Generates new quiz (10 random questions)
renderQuestionCard()  // Displays current question
selectAnswer(idx)     // Records user's answer
nextQuestion()        // Advances quiz
prevQuestion()        // Goes back
showResults()         // Shows final score + full results panel
toggleQuizResultsPanel()  // Expand/collapse per-question breakdown
deleteQuizHistoryItem(i)  // Remove individual history record
refreshQuizHistorySection()  // Re-render quiz history
```

- Quiz state: `quizState` object tracks current position, answers, submission status
- Three question pools: `quizQuestions` (core), `calculusQuizPool`, `expansionQuizPool`
- Combined pool: `allQuizQuestions` (89+ questions total)
- Quiz history persisted in `localStorage` under `precalcQuizResults`
- PDF export via `downloadQuizPDF()` and CSV export via `exportQuizResults()`
- Topic tagging: `deriveQuizArea()`, `deriveQuizSubtopic()`, `friendlyArea()` derive metadata for quiz result tags
- Result navigation: `handleQuizTagClick(subtopic)` navigates from quiz results/history to matching review card with highlight

#### 4. Directory Search
```javascript
// Core functions:
selectDirectoryType(type)      // Sets search type (review/flashcard/quiz)
applyDirectoryFilters()         // Applies dropdowns filters
getFilteredDirectoryItems()     // Returns matching items
renderDirectoryResults()        // Displays results
handleDirectoryItemClick(id)   // Navigates to clicked item
```

- Filters: course, area, subtopic, tier, yugioh mode
- Dynamic result counting and empty state handling

#### 5. Focus Mode
```javascript
// Core functions:
enterFocusMode(element)  // Enters full-screen card view
exitFocusMode()          // Returns to normal view, resets area filter
```

- Creates overlay and cloned card
- Exiting resets `display: ''` on all cards and area filter dropdown

#### 6. Area Cards (Home Page)
```javascript
// Core functions:
selectArea(areaId)   // Expands an area card
deselectArea()       // Returns to four-card grid
navigateToArea(section, area)  // Jumps to section with area filter
```

- Four areas: algebra, trig, calculus, precalc-general
- Each area has expandable view with topic groups

#### 7. Content Mapping
- `CODE_TO_TOPIC_ID`: Maps expansion codes (A1-A13, B1-B14) to topic IDs
- `SUBTOPIC_TO_ELEMENT`: Maps subtopic names to DOM element IDs
- `findReviewCardElement(id)`: Intelligent search for review cards in DOM

#### 8. Topic Registry
The `TOPICS` array defines all review topics:
```javascript
[
  {id: 'functions', label: 'Functions'},
  {id: 'factoring', label: 'Factoring'},
  // ... etc
]
```

Used for dropdown navigation and cross-referencing.

### CSS Architecture

**CSS Custom Properties (Variables):**
- Color system: `--color-primary`, `--color-secondary`, etc.
- Spacing system: `--space-8`, `--space-16`, `--space-24`, `--space-32`
- Typography: Font families, sizes, weights
- Theme-specific colors for each subject area

**Component Classes:**
- `.concept-card` - Review card container
- `.flashcard-card` - Flashcard container
- `.quiz-card` - Quiz question container
- `.directory-item` - Directory search result item
- `.area-card` - Home page area cards
- `.sidebar` - Navigation sidebar
- `.focus-overlay` - Focus mode overlay
- `.quiz-results-collapsible` - Expandable/collapsible full results panel
- `.quiz-result-item` - Per-question result card (`.correct`, `.incorrect`, `.skipped`)
- `.quiz-result-meta` - Topic tag container in quiz result items
- `.quiz-tag` - Base class for topic tags (`.quiz-tag-area`, `.quiz-tag-subtopic`, `.quiz-tag-id`)
- `.quiz-history-meta` - Topic tag container in quiz history rows
- `.quiz-history-delete` - Per-item trash delete button in quiz history
- `.concept-card.highlight` - Temporary highlight when navigating from quiz tags to review cards

**Utility Classes:**
- Color modifiers: `.area-algebra`, `.area-trig`, etc.
- State classes: `.active`, `.flipped`, `.selected`, `.correct`, `.incorrect`
- Responsive helpers: `.sidebar-toggle`, `.sidebar-overlay`

### Data Flow

1. **Page Load**:
   - `CONTENT_INDEX_DATA` embedded in `<script>` tag
   - `loadContentIndex()` processes data
   - Initializes flashcards, quiz pools, directory filters
   - Sets up event listeners

2. **User Interaction**:
   - User clicks navigation → `switchTab()`
   - User selects filter → updates state → re-renders
   - User interacts with card → updates local state → re-renders component

3. **State Management**:
   - Global variables for state (no framework needed)
   - Synchronization between tabs via shared state variables
   - `localStorage` used for quiz history persistence (`precalcQuizResults`)

### Browser Compatibility

- **Minimum Requirements**: Modern browser with ES5 support
- **Tested On**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **Mobile Support**: iOS Safari, Chrome Mobile, Samsung Internet
- **Graceful Degradation**: Core functionality works even without full CSS3 support

### Content Source

The content is derived from `Organized-Content-Library.md` (updated with tier tags):
- Structured markdown with HTML comment tags for tagging (id, course, area, type, subtopic, yugioh, tier, code)
- 150 tagged content items: 38 review cards (with tier tags), 27 expansion reviews, 47 flashcard items (141 Q/A pairs), 38 quiz items
- 31+ topics include Yu-Gi-Oh! crossover analogies
- Content extracted and transformed into `CONTENT_INDEX_DATA`
- To update content: modify library file, then regenerate index data

### Expansion Content

**Tiered System:**
- **Tier 1 (Essential)**: Must-know topics for strong foundation (applies to both review cards and expansion content)
- **Tier 2 (Important)**: Commonly needed, high-value topics (applies to both review cards and expansion content)
- **Tier 3 (Advanced)**: Deeper dives, specialized applications (expansion content only)

**Topic Coverage:**
- **A-Series (A1-A13)**: Advanced precalculus topics
- **B-Series (B1-B14)**: Trigonometry deep dives

### Development Notes

- **No Build Process**: Edit HTML directly, refresh browser to test
- **Version Control**: Git-tracked, hosted on GitHub
- **Maintenance**: Add new content by updating content index in HTML
- **Performance**: All content loads at once (no lazy loading needed - file size manageable)
- **Future Enhancements**: See `ExpansionPlan--Complete/` and `UpdatePlan/` directories

---

## 📖 Quick Reference

| Feature | Location | Purpose |
|---------|----------|---------|
| Comprehensive topics | Review Tab | Deep study and understanding |
| Area filtering | Review Dropdown | Show only Algebra, Trig, Calculus, or Precalc General cards |
| Quick memorization | Flashcards | Active recall practice |
| Self-testing | Quiz Mode | Knowledge assessment |
| Full quiz results | Quiz Results Panel | Per-question breakdown with topic tags |
| Quiz result tags | Quiz Results Panel | Clickable area/subtopic tags linking to review content |
| Quiz history | Quiz History Section | Track past attempts with topic tags, delete individual records |
| Find specific content | Directory | Advanced search and filtering (including tier filter) |
| Unit circle reference | Unit Circle Tab | Quick angle/value lookup |
| Subject overview | Home | Navigate by subject area |
| Title navigation | App Title | Click "Let's Math!" to return Home |

---

## 🎓 Study Tips

1. **Build a Foundation**: Start with Core Review flashcards and review topics
2. **Master the Unit Circle**: Essential for all trig work
3. **Active Recall**: Use flashcards before looking at review cards
4. **Test Yourself**: Regular quizzes help identify weak areas
5. **Focus Mode**: Use for deep study of challenging concepts
6. **Spaced Repetition**: Return to quiz and flashcards regularly
7. **Yu-Gi-Oh! Mode**: If helpful, use crossover examples to make concepts memorable

---

## 🤝 Contributing

This is a personal study project. For suggestions or issues, please open a GitHub issue on the repository.

---

**Happy Studying! 📐✨**
