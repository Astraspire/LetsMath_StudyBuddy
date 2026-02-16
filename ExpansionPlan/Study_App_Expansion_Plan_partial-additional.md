
# Study App Content Expansion Plan
## Gap Analysis & New Content (Precalc + Trigonometry Textbooks)

---

# PART 1: GAP ANALYSIS — Topics NOT Currently in the Website

Below is every major topic from the Precalc.pdf and Trigonometry.pdf that is **missing or only superficially covered** in the current Website-Content-Inventory.md. Each topic includes teachable key points, formulas, flashcards, quiz questions, and (where applicable) Yu-Gi-Oh! conceptual crossovers.

---

## SECTION A: PRECALCULUS GAPS

---

### A1. Domain and Range (Detailed Treatment)
**Status:** Current site mentions domain/range in passing under "Functions and Notation." The textbook devotes an entire section (1.2) with interval notation, set-builder notation, toolkit function domains, and piecewise functions.

**Key Points:**
- Domain = set of all valid inputs; Range = set of all valid outputs.
- Three main domain restrictions: division by zero, even roots of negatives, log of non-positives.
- Interval notation: (a, b) open, [a, b] closed, use ∪ for union.
- Set-builder notation: {x | condition}.
- Toolkit function domains/ranges (constant, identity, quadratic, cubic, reciprocal, square root, cube root, absolute value).
- Piecewise functions: formula changes based on which sub-domain the input lies in.

**Formulas:**
- Reciprocal: f(x) = 1/x → Domain: (-∞, 0) ∪ (0, ∞), Range: (-∞, 0) ∪ (0, ∞)
- Square root: f(x) = √x → Domain: [0, ∞), Range: [0, ∞)
- Reciprocal squared: f(x) = 1/x² → Domain: (-∞, 0) ∪ (0, ∞), Range: (0, ∞)

**Flashcards:**
- Q: What three things restrict a function's domain?
  A: 1) Denominator = 0, 2) Even root of a negative, 3) Log of zero or negative.
- Q: Write the domain of f(x) = √(4 - x) in interval notation.
  A: (-∞, 4].
- Q: What is the domain of f(x) = 1/(x - 3)?
  A: (-∞, 3) ∪ (3, ∞).

**Quiz:**
- Q: What is the domain of f(x) = √(x - 2)?
  Options: A) [2, ∞)  B) (2, ∞)  C) (-∞, 2]  D) All reals
  Answer: A) [2, ∞)
- Q: What is the range of f(x) = x²?
  Options: A) All reals  B) [0, ∞)  C) (0, ∞)  D) (-∞, 0]
  Answer: B) [0, ∞)

**🎴 Yu-Gi-Oh! Crossover: Activation Conditions as Domain Restrictions**
In Yu-Gi-Oh!, many cards have activation conditions — "You can only activate this card when your opponent controls a monster" is a *domain restriction*. The card's "function" (its effect) is undefined when the condition isn't met, just like f(x) = 1/x is undefined at x = 0. Piecewise functions mirror cards with multiple effects depending on conditions (e.g., "If your LP are 1000 or less, do X; otherwise, do Y").

---

### A2. Rates of Change and Behavior of Graphs
**Status:** Not in current site. Textbook Section 1.3 covers average rate of change, increasing/decreasing intervals, local extrema, and concavity.

**Key Points:**
- Average rate of change = Δy/Δx = [f(b) - f(a)] / (b - a).
- A function is increasing on an interval if f(b) > f(a) for b > a.
- A function is decreasing on an interval if f(b) < f(a) for b > a.
- Local maximum: function changes from increasing to decreasing.
- Local minimum: function changes from decreasing to increasing.
- Concave up: rate of change is increasing (curves upward like a smile).
- Concave down: rate of change is decreasing (curves downward like a frown).
- Inflection point: where concavity changes.

**Formulas:**
- Average rate of change: [f(b) - f(a)] / (b - a)

**Flashcards:**
- Q: What is the average rate of change of f(x) = x² on [1, 5]?
  A: (25 - 1)/(5 - 1) = 24/4 = 6.
- Q: What is an inflection point?
  A: A point where the function changes from concave up to concave down, or vice versa.
- Q: How do you tell if a function is concave up from a table?
  A: The rate of change between consecutive points is increasing.

**Quiz:**
- Q: If f(x) = x² - 4x, what is the average rate of change on [1, 3]?
  Options: A) 0  B) -2  C) 2  D) 4
  Answer: A) 0
- Q: A function that is concave down has what shape?
  Options: A) Frown (∩)  B) Smile (∪)  C) Straight line  D) Vertical
  Answer: A) Frown (∩)

---

### A3. Composition of Functions
**Status:** Not in current site. Textbook Section 1.4 covers composition notation, evaluating compositions from tables/graphs/formulas, domain of compositions, and decomposition.

**Key Points:**
- Composition: (f ∘ g)(x) = f(g(x)) — evaluate the inner function first, then the outer.
- The output of g becomes the input of f.
- Domain of f(g(x)): x must be in the domain of g, AND g(x) must be in the domain of f.
- Decomposition: breaking a complex function into simpler composed parts.

**Formulas:**
- (f ∘ g)(x) = f(g(x))
- (g ∘ f)(x) = g(f(x))
- Order matters: f(g(x)) ≠ g(f(x)) in general.

**Flashcards:**
- Q: If f(x) = x² and g(x) = x + 3, what is f(g(2))?
  A: g(2) = 5, then f(5) = 25.
- Q: What is the domain of f(g(x)) if f(x) = √x and g(x) = x - 4?
  A: Need g(x) ≥ 0, so x - 4 ≥ 0, meaning x ≥ 4. Domain: [4, ∞).
- Q: What does "decomposition" of a function mean?
  A: Writing a function as a composition of two simpler functions. E.g., h(x) = √(x² + 5) can be decomposed as f(x) = √x, g(x) = x² + 5, so h = f ∘ g.

**Quiz:**
- Q: If f(x) = 2x + 1 and g(x) = x², what is (f ∘ g)(3)?
  Options: A) 49  B) 19  C) 7  D) 13
  Answer: B) 19 [g(3) = 9, f(9) = 19]
- Q: f(g(x)) is the same as g(f(x)). True or false?
  Options: A) True  B) False
  Answer: B) False

**🎴 Yu-Gi-Oh! Crossover: Chain Links as Composition**
A Yu-Gi-Oh! chain is literally function composition. Chain Link 1 activates an effect (function g), its resolution becomes the "input" for Chain Link 2 (function f). The final game state is f(g(initial state)). Importantly, just like f(g(x)) ≠ g(f(x)), resolving effects in a different chain order produces different outcomes. A chain of "Mystical Space Typhoon targeting a set card" → "Torrential Tribute" produces a completely different result if you reverse the chain order.

---

### A4. Linear Functions (Detailed Treatment)
**Status:** Site has "Lines and Slopes" with formulas. Missing: modeling, interpretation of slope as rate of change, finding equations from data, and applications.

**Key Points:**
- Linear function: f(x) = mx + b, where m = rate of change, b = initial value.
- Finding equations from two points: compute slope, then use point-slope form.
- Interpreting slope in context (e.g., "population increases by 1700 people per year").
- Parallel lines: same slope. Perpendicular lines: slopes are negative reciprocals.
- Intersection of two lines: set f(x) = g(x) and solve for x.

**Flashcards:**
- Q: A town had population 45,000 in 2003 and grows by 1,700/year. Write the equation.
  A: P(t) = 1700t + 45000, where t = years after 2003.
- Q: Find the equation of the line through (2, 4) and (4, 10).
  A: m = (10-4)/(4-2) = 3. y - 4 = 3(x - 2) → y = 3x - 2.

**Quiz:**
- Q: What is the slope of a line passing through (-1, 4) and (5, 2)?
  Options: A) -1/3  B) 1/3  C) -3  D) 3
  Answer: A) -1/3

---

### A5. Power Functions and Polynomial Functions (Deep Dive)
**Status:** Site has "Factoring Patterns" and brief polynomial references. Missing: power functions, long-run behavior, end behavior, short-run behavior (intercepts, turning points, multiplicity), sketching polynomial graphs.

**Key Points:**
- Power function: f(x) = xᵖ. Toolkit: x², x³, 1/x, √x, ³√x.
- Long-run (end) behavior determined by degree and leading coefficient:
  - Even degree, positive lead → both ends up.
  - Even degree, negative lead → both ends down.
  - Odd degree, positive lead → left down, right up.
  - Odd degree, negative lead → left up, right down.
- A degree-n polynomial has at most n horizontal intercepts and at most n-1 turning points.
- Multiplicity of zeros:
  - Multiplicity 1 (single zero): graph crosses axis linearly.
  - Multiplicity 2 (double zero): graph bounces off axis.
  - Multiplicity 3 (triple zero): graph crosses with cubic flattening.
- Polynomial inequalities: use sign charts or test values in intervals between zeros.

**Formulas:**
- General polynomial: f(x) = aₙxⁿ + aₙ₋₁xⁿ⁻¹ + … + a₁x + a₀
- End behavior determined by leading term aₙxⁿ.

**Flashcards:**
- Q: What determines the end behavior of a polynomial?
  A: The degree (even/odd) and the sign of the leading coefficient.
- Q: What happens at a zero with multiplicity 2?
  A: The graph touches (bounces off) the x-axis but doesn't cross it.
- Q: A degree-5 polynomial has at most how many turning points?
  A: 4.

**Quiz:**
- Q: What is the end behavior of f(x) = -2x⁵ + 3x² - 1?
  Options: A) Both ends up  B) Both ends down  C) Left up, right down  D) Left down, right up
  Answer: C) Left up, right down
- Q: At a zero of multiplicity 3, the graph:
  Options: A) Bounces  B) Crosses linearly  C) Crosses with flattening  D) Has a vertical asymptote
  Answer: C) Crosses with flattening

**🎴 Yu-Gi-Oh! Crossover: Chain of Effects as Multiplicity**
Think of multiplicity like stacking the same continuous effect. A single "Skill Drain" (multiplicity 1) negates monster effects — the game state "crosses" from effects-on to effects-off cleanly. But if you have two copies active (multiplicity 2), removing one doesn't change the game state — it "bounces" back to the same condition. The more layers of the same restriction, the "flatter" the transition when you try to remove them, just like higher-multiplicity zeros flatten the crossing.

---

### A6. Quadratic Functions (Expanded)
**Status:** Site has quadratic formula and discriminant. Missing: vertex form, completing the square (applied to quadratics), max/min applications, revenue/area optimization problems.

**Key Points:**
- Standard form: f(x) = ax² + bx + c.
- Vertex form: f(x) = a(x - h)² + k, where vertex is (h, k).
- Vertex formula: h = -b/(2a), k = f(h).
- If a > 0, parabola opens up → vertex is a minimum.
- If a < 0, parabola opens down → vertex is a maximum.
- Applications: maximizing area, revenue, projectile motion.

**Flashcards:**
- Q: Find the vertex of f(x) = 2x² - 12x + 7.
  A: h = 12/4 = 3, k = f(3) = 18 - 36 + 7 = -11. Vertex: (3, -11).
- Q: When does a quadratic have a maximum vs. minimum?
  A: Maximum when a < 0 (opens down); minimum when a > 0 (opens up).

**Quiz:**
- Q: What is the vertex of f(x) = -x² + 6x - 5?
  Options: A) (3, 4)  B) (-3, -4)  C) (3, -4)  D) (-3, 4)
  Answer: A) (3, 4)

---

### A7. Factor Theorem, Remainder Theorem, and Synthetic Division
**Status:** Not in current site. Textbook Section 3.4 is entirely missing.

**Key Points:**
- Remainder Theorem: When p(x) is divided by (x - c), the remainder is p(c).
- Factor Theorem: (x - c) is a factor of p(x) if and only if p(c) = 0.
- Polynomial long division: divide leading terms, multiply, subtract, repeat.
- Synthetic division: shortcut for dividing by (x - c). Write c on the left, coefficients across; bring down, multiply, add, repeat.
- Use to find zeros: if synthetic division gives remainder 0, then c is a zero and the quotient gives the reduced polynomial.

**Flashcards:**
- Q: What does the Remainder Theorem state?
  A: When polynomial p(x) is divided by (x - c), the remainder equals p(c).
- Q: What does the Factor Theorem tell us?
  A: (x - c) is a factor of p(x) ⟺ p(c) = 0.
- Q: Describe synthetic division in 3 steps.
  A: 1) Write c and the coefficients. 2) Bring down first coeff. 3) Multiply by c, add to next coeff, repeat.

**Quiz:**
- Q: If p(x) = x³ - 4x² + 5x - 14, what is the remainder when divided by (x - 2)?
  Options: A) 0  B) -12  C) -16  D) 2
  Answer: C) p(2) = 8 - 16 + 10 - 14 = -12 → B) -12
- Q: If p(3) = 0 for polynomial p(x), which is true?
  Options: A) (x + 3) is a factor  B) (x - 3) is a factor  C) x = -3 is a zero  D) None of these
  Answer: B) (x - 3) is a factor

**🎴 Yu-Gi-Oh! Crossover: Ruling Verification as the Factor Theorem**
Testing if a card interaction is legal is exactly the Factor Theorem. You "plug in" a specific game state (c) into the ruling (polynomial). If the result is 0 (legal / the effect resolves successfully), then that game state is a "zero" — it satisfies the condition. If you get a non-zero remainder (illegal activation), the ruling doesn't factor through that game state. Synthetic division is like systematically checking each link in a chain to see which card effects "factor out."

---

### A8. Real Zeros of Polynomials (Rational Roots Theorem, Cauchy's Bound)
**Status:** Not in current site.

**Key Points:**
- Cauchy's Bound: All real zeros lie in the interval [-M-1, M+1] where M = max(|aᵢ/aₙ|).
- Rational Roots Theorem: If p/q is a rational zero, then p divides the constant term and q divides the leading coefficient.
- Strategy: List possible rational zeros → test using synthetic division → reduce polynomial → use quadratic formula on remainder.

**Flashcards:**
- Q: State the Rational Roots Theorem.
  A: For polynomial aₙxⁿ + … + a₀ with integer coefficients, any rational zero p/q has p | a₀ and q | aₙ.
- Q: What are the possible rational zeros of 2x³ + 3x² - 1?
  A: ±{1, 1/2}.

**Quiz:**
- Q: What are the possible rational zeros of f(x) = 3x³ - x² + 2?
  Options: A) ±{1, 2, 1/3, 2/3}  B) ±{1, 3}  C) ±{1, 2}  D) ±{2, 3}
  Answer: A) ±{1, 2, 1/3, 2/3}

---

### A9. Complex Zeros
**Status:** Not in current site.

**Key Points:**
- Imaginary unit: i = √(-1), i² = -1.
- Complex number: a + bi. Conjugate: a - bi.
- Fundamental Theorem of Algebra: every polynomial of degree n ≥ 1 has at least one complex zero.
- A degree-n polynomial has exactly n complex zeros (counting multiplicities).
- Complex zeros of real-coefficient polynomials come in conjugate pairs.
- An irreducible quadratic (negative discriminant) produces complex zeros.
- To multiply complex numbers: use FOIL, replace i² with -1.
- To divide: multiply by conjugate of denominator.

**Flashcards:**
- Q: What is the conjugate of 3 - 2i?
  A: 3 + 2i.
- Q: Simplify (2 + i)(3 - 4i).
  A: 6 - 8i + 3i - 4i² = 6 - 5i + 4 = 10 - 5i.
- Q: Why do complex zeros come in conjugate pairs for real-coefficient polynomials?
  A: Because the complex conjugate of each step in evaluation also equals zero.

**Quiz:**
- Q: What are the zeros of f(x) = x² + 4?
  Options: A) ±2  B) ±2i  C) ±4i  D) No zeros
  Answer: B) ±2i
- Q: How many complex zeros does a degree-5 polynomial have?
  Options: A) At most 5  B) Exactly 5  C) At least 1  D) Both B and C
  Answer: D) Both B and C

**🎴 Yu-Gi-Oh! Crossover: Hidden Information as Complex Numbers**
Complex zeros are "invisible" on the real number line, just like face-down cards are hidden information in Yu-Gi-Oh!. You know they *exist* (the Fundamental Theorem guarantees it), but you can't see them on the real graph — they're in the "complex plane." Conjugate pairs are like a set card and its mirror ruling: "Solemn Judgment" negates a summon (a + bi), and if it exists in the rulings, its conjugate scenario (a - bi) must also be accounted for.

---

### A10. Rational Functions (Deep Dive)
**Status:** Site has vertical/horizontal asymptote basics. Missing: oblique asymptotes, holes, writing equations from graphs, sign analysis, long-run behavior details.

**Key Points:**
- Vertical asymptotes: denominator = 0 (where numerator ≠ 0).
- Holes: both numerator and denominator are 0 at the same x-value.
- Horizontal asymptotes: compare degrees of numerator (n) and denominator (m):
  - n < m → y = 0.
  - n = m → y = ratio of leading coefficients.
  - n > m → no horizontal asymptote (check for oblique).
- Oblique (slant) asymptote: when n = m + 1, perform polynomial long division; the quotient is the oblique asymptote.
- Writing equations: identify intercepts, asymptotes, and multiplicities; form f(x) = a · (numerator factors) / (denominator factors); solve for stretch factor a using a known point.

**Flashcards:**
- Q: When does a rational function have a hole instead of a vertical asymptote?
  A: When a factor cancels from both numerator and denominator (both zero at the same x).
- Q: What is an oblique asymptote?
  A: A slant line that the function approaches as x → ±∞. Occurs when degree of numerator = degree of denominator + 1.
- Q: Find the oblique asymptote of f(x) = (x² + 2x + 1)/(x - 1).
  A: Perform long division: quotient is x + 3. So oblique asymptote is y = x + 3.

**Quiz:**
- Q: f(x) = (x - 2)/((x - 2)(x + 3)) has:
  Options: A) VA at x = 2 and x = -3  B) Hole at x = 2, VA at x = -3  C) VA at x = -3 only  D) Both B and C
  Answer: B) Hole at x = 2, VA at x = -3

---

### A11. Inverses and Radical Functions
**Status:** Site has basic inverse steps. Missing: restricting domains, inverse of quadratics, radical functions, solving radical equations.

**Key Points:**
- To find the inverse of a non-one-to-one function, restrict the domain first.
- Inverse of f(x) = x² (x ≥ 0) is f⁻¹(x) = √x.
- Radical equations: isolate the radical, raise both sides to the appropriate power, CHECK for extraneous solutions.
- The domain of the inverse becomes the range of the original function, and vice versa.

**Flashcards:**
- Q: Why must we check for extraneous solutions when solving radical equations?
  A: Squaring both sides can introduce solutions that don't satisfy the original equation.
- Q: What is the inverse of f(x) = x² for x ≥ 0?
  A: f⁻¹(x) = √x.

**Quiz:**
- Q: Solve √(x + 3) = 5.
  Options: A) x = 22  B) x = 28  C) x = 8  D) x = 2
  Answer: A) x = 22

---

### A12. Exponential Functions (Expanded)
**Status:** Site has core exp/log relationship and log properties. Missing: exponential growth/decay models, half-life, doubling time, compound interest, fitting exponential models.

**Key Points:**
- Exponential growth: f(t) = a · bᵗ, b > 1. Decay: 0 < b < 1.
- Continuous growth/decay: f(t) = a · eʳᵗ.
- Compound interest: A = P(1 + r/n)^(nt). Continuous: A = Peʳᵗ.
- Doubling time: t = ln(2)/r (continuous) or t = ln(2)/ln(1+r) (periodic).
- Half-life: t = ln(1/2)/r = ln(2)/|r|.
- Solving exponential equations: take log of both sides.

**Flashcards:**
- Q: What is the formula for continuous compound interest?
  A: A = Peʳᵗ, where P = principal, r = rate, t = time.
- Q: If a population doubles every 5 years with continuous growth, what is r?
  A: r = ln(2)/5 ≈ 0.1386.
- Q: Solve 3ˣ = 81.
  A: 3ˣ = 3⁴, so x = 4.

**Quiz:**
- Q: An investment of $1000 at 5% compounded continuously is worth how much after 10 years?
  Options: A) $1,628.89  B) $1,500  C) $1,648.72  D) $1,050
  Answer: C) $1,648.72

**🎴 Yu-Gi-Oh! Crossover: LP Halving as Exponential Decay**
Cards like "Ring of Destruction" or repeated effect damage follow exponential patterns. If your LP get halved each turn (8000 → 4000 → 2000 → 1000), that's exponential decay with b = 0.5. The half-life concept maps directly: "How many turns until LP drop below 500?" is the same calculation as radioactive half-life. Compound interest is like stacking LP-gain effects — each application multiplies the existing total.

---

