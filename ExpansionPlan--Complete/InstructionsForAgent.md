Study App – Single‑File HTML Implementation Plan

All content and logic must live in LetsMath_App.html. This plan assumes:

    The agent can edit LetsMath_App.html directly.​

    The agent can reference Website-Content-Inventory.md, Precalc.pdf, and Trigonometry.pdf for content.

    The agent will maintain compatibility with the current UI (tabs, flashcards, quiz behavior).

0. Analyze Existing Structure

    Map Current Sections

        In LetsMath_App.html, locate:

            The Review tab content (static notes, unit circle, algebra, etc.).​

            The Flashcards logic and data (JS arrays / HTML templates).

            The Quiz logic and question pool.

        Identify how topics are currently grouped (e.g., “Algebra”, “Exponentials and Logs”, “Trigonometry”, “Calculus”) from the content inventory.​

        Note the pattern in the HTML:

            Are topics separated by headings?

            How are flashcards/quiz questions linked to topics (tags, arrays, IDs)?

    Define Internal Topic IDs

        For every existing topic in Website-Content-Inventory.md, assign a short topicId string (e.g., algebra_functions, trig_unit_circle).

        For each new topic from the expansion plan (A1–A13, B1–B14), define a topicId too (e.g., precalc_domain_range, trig_inverse_functions).

    Add a Lightweight Topic Registry (Inside HTML)

        In a <script> block, define a JS object/array describing topics:

        js
        const TOPICS = [
          { id: 'precalc_domain_range', label: 'Domain & Range', category: 'Precalculus', tier: 1 },
          { id: 'precalc_composition', label: 'Function Composition', category: 'Precalculus', tier: 1 },
          // ... all topics, including current ones
        ];

        This registry will be used for:

            Filtering flashcards and quiz items by topic.

            Future topic navigation.

1. Content Organization Inside the Single HTML File
1.1 Add Topic-Level Anchors

    Create Anchor Targets

        For each topic (existing + new), wrap its Review tab content in a <section> or <div> with an id matching topicId, e.g.:

        xml
        <section id="precalc_domain_range" class="topic-section">
          <h2>Domain & Range</h2>
          <!-- Explanatory content goes here -->
        </section>

        Ensure headings are consistent (<h2> for topic title, <h3> for sub-sections like “Key Ideas”, “Formulas”, “Examples”).

    Insert New Topic Sections

        For each new topic (from the plan), add a corresponding <section> into the Review tab area.

        Follow this internal structure:

        xml
        <section id="precalc_domain_range" class="topic-section">
          <h2>Domain & Range</h2>

          <h3>Key Ideas</h3>
          <ul>
            <li>Domain = set of all valid inputs; range = set of all possible outputs.</li>
            <!-- etc. from the plan, condensed -->
          </ul>

          <h3>Formulas</h3>
          <ul>
            <li>Reciprocal: f(x) = 1/x, Domain: (-∞, 0) ∪ (0, ∞).</li>
            <!-- etc. -->
          </ul>

          <h3>Examples</h3>
          <!-- a couple of short worked examples -->

          <h3>Yu-Gi-Oh! Connection (optional)</h3>
          <p>Explain the analogy here, short and clear.</p>
        </section>

        Repeat for all topics in the expansion plan (A1–A13, B1–B14), pulling the exact bullet points and formulas from the plan document.

1.2 Add “Yu-Gi-Oh! Connection” Subsections

    For topics with a crossover in the plan (domain, composition, polynomials, exponential decay, etc.), add a short subsection at the bottom:

    xml
    <details class="ygo-connection">
      <summary>Yu-Gi-Oh! Connection</summary>
      <p>...</p>
    </details>

    Keep each note tight (1–3 sentences) and strictly conceptual.

2. Flashcards in Single HTML
2.1 Understand Current Flashcard Implementation

    Inspect JS Structure

        Locate the JS array(s) that hold flashcards in LetsMath_App.html (e.g., flashcards = [...]).​

        Determine fields:

            Question text

            Answer text

            Category / Topic / Tags (if any)

            Any IDs

    Standardize Flashcard Schema

        Ensure flashcards follow a uniform structure:

        js
        const FLASHCARDS = [
          {
            id: 'fc_precalc_domain_range_1',
            topicId: 'precalc_domain_range',
            question: 'What three things restrict a function’s domain?',
            answer: '1) Denominator = 0, 2) Even roots of negatives, 3) Logs of non-positives.'
          },
          // ...
        ];

2.2 Add New Flashcards per Topic

For each new topic from the plan:

    Insert 3–5 new flashcards into FLASHCARDS for:

        A1: Domain & Range

        A3: Composition

        A5/A6/A7/A8/A9/A10/A11/A12/A13

        B1/B2/B3/B4/B5/B6/B7/B8/B9/B10/B11/B12/B13/B14

Implementation steps:

    Add Entries

        Scroll to the flashcard array in the HTML <script> and append new entries, setting topicId appropriately.

    Topic Filter Logic (Optional but Recommended)

        Add a dropdown or buttons in the Flashcards tab to filter by topic.

        Implement filtering in JS:

        js
        function getFlashcardsForTopic(topicId) {
          return FLASHCARDS.filter(fc => !topicId || fc.topicId === topicId);
        }

    Testing

        Confirm cards flip correctly and cycle properly with the new entries.

3. Quiz Questions in Single HTML
3.1 Inspect Quiz Implementation

    Find Quiz Array(s)

        Locate quiz question data (e.g., quizQuestions = [...]).​

        Check fields: question, options, correctIndex, explanation?, category/topic?.

    Unify Quiz Schema

        Use a consistent structure:

        js
        const QUIZ_QUESTIONS = [
          {
            id: 'qq_precalc_domain_range_1',
            topicId: 'precalc_domain_range',
            question: 'What is the domain of f(x) = √(x - 2)?',
            options: ['[2, ∞)', '(2, ∞)', '(-∞, 2]', 'All reals'],
            correctIndex: 0
          },
          // ...
        ];

3.2 Insert New Quiz Items

For each topic:

    Insert 3–5 quiz questions for:

        Key Tier 1 topics first: A1, A3, A5–A7, B2, B3, B5, B6.

        Then Tier 2 and 3 topics as you have time.

Implement:

    Appending Questions

        Add questions into QUIZ_QUESTIONS in a <script> block.

    Topic-Based Quiz Selection

        If not already supported, add a way to:

            Choose a topic (dropdown).

            Generate quizzes only from that topic’s items:

            js
            function getQuestionsForTopic(topicId) {
              return QUIZ_QUESTIONS.filter(q => !topicId || q.topicId === topicId);
            }

    Validation

        Check that:

            All correctIndex values are within range.

            Questions render and score correctly.

4. Topic Content Integration by Tier

You already have a conceptual/topic plan. Here’s the implementation order, specifically for this single file.
4.1 Tier 1 – Implement First

Precalc:

    precalc_domain_range (A1)

    precalc_composition (A3)

    precalc_polynomials_deep (A5)

    precalc_quadratics_expanded (A6)

    precalc_factor_remainder (A7)

Trig:

    trig_six_functions_identities (B2)

    trig_identities_proofs (B3)

    trig_inverse_functions (B5)

    trig_equations (B6)

For each of these:

    Add the Review section HTML with Key Ideas + Formulas + Examples + YGO note.

    Add corresponding FLASHCARDS entries.

    Add corresponding QUIZ_QUESTIONS entries.

    Mark progress by adding a comment block in HTML:

    xml
    <!-- TODO: precalc_domain_range: review=done, flashcards=done, quiz=done -->

4.2 Tier 2 – Implement Next

Precalc (A2, A8, A9, A10, A12, A13)
Trig (B1, B4, B7, B8)

Follow the same three-step pattern per topic:

    Review HTML

    Flashcards

    Quiz items

4.3 Tier 3 – Implement After Core is Stable

Precalc (A11)
Trig (B9–B14)

Same pattern, but these can be shorter initial writeups.
5. Internal Navigation & UX

    Topic Navigation in Review Tab

        Add a sidebar or dropdown listing all topics (from TOPICS).

        On selection, scroll or jump to the corresponding <section id="...">.

        js
        function goToTopic(topicId) {
          document.getElementById(topicId)?.scrollIntoView({ behavior: 'smooth' });
        }

    Sync Review/Flashcards/Quiz by Topic (Optional but Ideal)

        When a user selects a topic in the Review tab, remember the currentTopicId.

        In Flashcards and Quiz tabs, default to currentTopicId for their content filters.

6. Maintenance & Logging (Inside HTML)

Because everything is in one file:

    At the bottom of LetsMath_App.html, add a maintenance comment block or <pre> log:

    xml
    <!--
    IMPLEMENTATION LOG
    2026-02-16: Added topic registry and structure.
    2026-02-17: Implemented A1 Domain & Range (review, flashcards, quiz).
    2026-02-18: Implemented B2 Six Trig Functions & Identities.
    ... etc.
    -->

    When completing a topic, update this log so you (and future you) can see progress in the single file itself.
