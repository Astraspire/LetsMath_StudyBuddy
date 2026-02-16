
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



### A13. Logarithmic Functions (Expanded)
**Status:** Site has log properties. Missing: graphs of log functions, solving log equations, applications (pH, decibels, Richter scale), log scales.

**Key Points:**
- log_a(x) is defined only for x > 0.
- Graph of y = log_a(x): passes through (1, 0), has vertical asymptote at x = 0.
- Domain of log: (0, ∞). Range: all reals.
- Solving log equations: convert to exponential form, or condense/expand using log properties.
- Common applications: pH = -log[H⁺], Richter scale, decibel scale.
- Change of base: log_a(x) = ln(x)/ln(a).

**Flashcards:**
- Q: Solve log₂(x) = 5.
  A: x = 2⁵ = 32.
- Q: Solve ln(x) + ln(x - 2) = ln(3).
  A: ln(x(x-2)) = ln(3) → x² - 2x = 3 → x² - 2x - 3 = 0 → x = 3 (reject x = -1).
- Q: What is the domain of f(x) = log(x - 5)?
  A: x > 5, or (5, ∞).

**Quiz:**
- Q: Solve: log₃(x + 1) = 2.
  Options: A) x = 8  B) x = 7  C) x = 9  D) x = 5
  Answer: A) x = 8

---

## SECTION B: TRIGONOMETRY GAPS

---

### B1. Angles and Their Measure (Expanded)
**Status:** Site has degree/radian conversion and key angles. Missing: DMS system, arc length, sector area, circular motion, angular/linear velocity.

**Key Points:**
- DMS (Degree-Minute-Second): 1° = 60', 1' = 60".
- Converting DMS ↔ decimal degrees.
- Complementary angles: sum = 90°. Supplementary angles: sum = 180°.
- Coterminal angles: differ by multiples of 360° (or 2π).
- Arc length: s = rθ (θ in radians).
- Sector area: A = (1/2)r²θ.
- Linear velocity: v = rω (ω = angular velocity in rad/s).

**Formulas:**
- Arc length: s = rθ
- Sector area: A = (1/2)r²θ
- Angular velocity: ω = θ/t
- Linear velocity: v = rω

**Flashcards:**
- Q: Convert 42°7'30" to decimal degrees.
  A: 42 + 7/60 + 30/3600 = 42.125°.
- Q: Find the arc length of a sector with radius 5 and central angle π/3.
  A: s = 5 · π/3 = 5π/3 ≈ 5.24.
- Q: What are coterminal angles?
  A: Angles that share the same terminal side; they differ by multiples of 360° (or 2π).

**Quiz:**
- Q: What is the arc length of a circle with radius 10 and central angle 2 radians?
  Options: A) 20  B) 5  C) 10  D) 40
  Answer: A) 20
- Q: Which angle is coterminal with 450°?
  Options: A) 90°  B) 180°  C) 270°  D) 360°
  Answer: A) 90°

**🎴 Yu-Gi-Oh! Crossover: Phase Rotation as Coterminal Angles**
Each game turn in Yu-Gi-Oh! cycles through phases: Draw → Standby → Main 1 → Battle → Main 2 → End. After a full "revolution" (one complete turn), you're back to Draw Phase — that's a coterminal angle. Turn 1's Draw Phase and Turn 3's Draw Phase are coterminal (differ by full revolutions). The concept of "which phase are you in?" is like finding a reference angle from a large angle measure.

---

### B2. The Six Circular Functions and Fundamental Identities
**Status:** Site covers sin, cos, tan, and the basic Pythagorean identity. Missing: csc, sec, cot definitions, all three Pythagorean identities, reciprocal identities, quotient identities, and cofunction identities.

**Key Points:**
- Six trig functions: sin, cos, tan, csc, sec, cot.
- Reciprocal identities: csc(θ) = 1/sin(θ), sec(θ) = 1/cos(θ), cot(θ) = 1/tan(θ).
- Quotient identities: tan(θ) = sin(θ)/cos(θ), cot(θ) = cos(θ)/sin(θ).
- Three Pythagorean identities:
  1. sin²(θ) + cos²(θ) = 1
  2. 1 + tan²(θ) = sec²(θ)
  3. 1 + cot²(θ) = csc²(θ)
- Cofunction identities: sin(π/2 - θ) = cos(θ), etc.
- Signs by quadrant: ASTC ("All Students Take Calculus").

**Flashcards:**
- Q: State the three Pythagorean identities.
  A: sin²θ + cos²θ = 1; 1 + tan²θ = sec²θ; 1 + cot²θ = csc²θ.
- Q: If sin(θ) = 3/5 and θ is in QI, find all six trig values.
  A: cos = 4/5, tan = 3/4, csc = 5/3, sec = 5/4, cot = 4/3.
- Q: State the cofunction identity for sin.
  A: sin(π/2 - θ) = cos(θ).

**Quiz:**
- Q: If tan(θ) = 3 and θ is in QIII, what is sin(θ)?
  Options: A) 3/√10  B) -3/√10  C) -1/√10  D) 1/√10
  Answer: B) -3/√10
- Q: sec(θ) is the reciprocal of:
  Options: A) sin(θ)  B) cos(θ)  C) tan(θ)  D) cot(θ)
  Answer: B) cos(θ)

---

### B3. Trigonometric Identities (Proving and Verifying)
**Status:** Site lists a few identities. Missing: techniques for proving identities, sum/difference formulas, double-angle formulas (full set), half-angle formulas, power-reducing formulas.

**Key Points:**
- Sum/Difference formulas:
  - sin(A ± B) = sinA·cosB ± cosA·sinB
  - cos(A ± B) = cosA·cosB ∓ sinA·sinB
  - tan(A ± B) = (tanA ± tanB) / (1 ∓ tanA·tanB)
- Double-angle formulas:
  - sin(2θ) = 2sinθ·cosθ
  - cos(2θ) = cos²θ - sin²θ = 2cos²θ - 1 = 1 - 2sin²θ
  - tan(2θ) = 2tanθ / (1 - tan²θ)
- Half-angle formulas:
  - sin(θ/2) = ±√[(1 - cosθ)/2]
  - cos(θ/2) = ±√[(1 + cosθ)/2]
- Power-reducing: sin²θ = (1 - cos2θ)/2, cos²θ = (1 + cos2θ)/2.
- Proof strategies: work one side only, convert everything to sin/cos, factor, use known identities.

**Flashcards:**
- Q: State the sum formula for sin(A + B).
  A: sin(A + B) = sinA·cosB + cosA·sinB.
- Q: Find the exact value of cos(75°) using sum formulas.
  A: cos(45° + 30°) = cos45·cos30 - sin45·sin30 = (√2/2)(√3/2) - (√2/2)(1/2) = (√6 - √2)/4.
- Q: State the half-angle formula for sin(θ/2).
  A: sin(θ/2) = ±√[(1 - cosθ)/2], sign depends on quadrant of θ/2.

**Quiz:**
- Q: What is sin(2θ) equal to?
  Options: A) 2sinθ  B) sin²θ  C) 2sinθcosθ  D) cos²θ - sin²θ
  Answer: C) 2sinθcosθ
- Q: cos(A - B) =
  Options: A) cosAcosB + sinAsinB  B) cosAcosB - sinAsinB  C) sinAcosB - cosAsinB  D) sinAcosB + cosAsinB
  Answer: A) cosAcosB + sinAsinB

**🎴 Yu-Gi-Oh! Crossover: Proving Identities = Proving Rulings**
Proving a trig identity is exactly like proving that two different card combos produce the same end result. You have Side A and Side B — you can't "move things across the equal sign" (that's like illegally moving cards between zones). Instead, you manipulate one side using known rules (identities = established rulings) until it matches the other. Just as you'd cite "PSCT says 'if' means the activation is conditional," you cite "by the Pythagorean identity, sin²θ = 1 - cos²θ."

---

### B4. Graphs of Trigonometric Functions (Expanded)
**Status:** Site has sin/cos sinusoidal model formula. Missing: graphs of all six trig functions, period/asymptote analysis for tan/cot/sec/csc, transformations of trig graphs.

**Key Points:**
- y = sin(x) and y = cos(x): period 2π, amplitude 1, smooth waves.
- y = tan(x): period π, vertical asymptotes at x = π/2 + nπ, no amplitude.
- y = cot(x): period π, vertical asymptotes at x = nπ.
- y = sec(x): period 2π, vertical asymptotes where cos(x) = 0, U-shapes.
- y = csc(x): period 2π, vertical asymptotes where sin(x) = 0, U-shapes.
- Transformations: y = A·tan(B(x - C)) + D — period = π/|B|, phase shift = C, vertical shift = D.

**Flashcards:**
- Q: What is the period of y = tan(x)?
  A: π.
- Q: Where are the vertical asymptotes of y = csc(x)?
  A: At x = nπ for integer n (wherever sin(x) = 0).
- Q: What is the period of y = 3tan(2x)?
  A: π/2.

**Quiz:**
- Q: The period of y = sec(3x) is:
  Options: A) 2π  B) 2π/3  C) π/3  D) 3π
  Answer: B) 2π/3

---

### B5. Inverse Trigonometric Functions
**Status:** Not in current site. Trigonometry textbook Section 10.6.

**Key Points:**
- arcsin(x): domain [-1, 1], range [-π/2, π/2].
- arccos(x): domain [-1, 1], range [0, π].
- arctan(x): domain (-∞, ∞), range (-π/2, π/2).
- These are the "undo" functions: sin(arcsin(x)) = x for x ∈ [-1, 1].
- Composing trig and inverse trig functions requires care with domain restrictions.
- arcsec(x): domain |x| ≥ 1, range [0, π], excluding π/2.

**Flashcards:**
- Q: What is arcsin(1/2)?
  A: π/6 (30°).
- Q: What is the range of arccos(x)?
  A: [0, π].
- Q: Evaluate cos(arctan(3/4)).
  A: Draw right triangle with opposite 3, adjacent 4, hypotenuse 5. cos = 4/5.

**Quiz:**
- Q: arctan(1) = ?
  Options: A) π/6  B) π/4  C) π/3  D) π/2
  Answer: B) π/4
- Q: The domain of arcsin(x) is:
  Options: A) All reals  B) [-1, 1]  C) [0, 1]  D) (-π/2, π/2)
  Answer: B) [-1, 1]

---

### B6. Trigonometric Equations and Inequalities
**Status:** Site has one basic example (sin(x) = 1/2). Missing: systematic solving techniques, general solutions with +2πk, equations involving multiple angles, trig inequalities.

**Key Points:**
- General solutions: if sin(θ) = k, then θ = arcsin(k) + 2πn or θ = π - arcsin(k) + 2πn.
- For cos(θ) = k: θ = ±arccos(k) + 2πn.
- For tan(θ) = k: θ = arctan(k) + πn.
- Multi-angle equations: sin(2x) = √3/2 → solve for 2x first, then divide.
- Quadratic-type trig equations: 2cos²x - cosx - 1 = 0 → factor as (2cosx + 1)(cosx - 1) = 0.
- Trig inequalities: solve the equality first, then use sign charts or unit circle to find intervals.

**Flashcards:**
- Q: Find all solutions to sin(x) = √3/2 in [0, 2π).
  A: x = π/3 and x = 2π/3.
- Q: Find the general solution to cos(x) = -1/2.
  A: x = 2π/3 + 2πk or x = 4π/3 + 2πk, where k is any integer.
- Q: Solve 2sin²(x) - sin(x) - 1 = 0.
  A: Factor: (2sinx + 1)(sinx - 1) = 0 → sinx = -1/2 or sinx = 1.

**Quiz:**
- Q: How many solutions does sin(x) = 1/2 have in [0, 2π)?
  Options: A) 1  B) 2  C) 3  D) Infinite
  Answer: B) 2
- Q: The general solution to tan(x) = 1 is:
  Options: A) x = π/4 + 2πk  B) x = π/4 + πk  C) x = π/4 only  D) x = 3π/4 + πk
  Answer: B) x = π/4 + πk

---

### B7. Law of Sines
**Status:** Not in current site. Trig textbook Section 11.2.

**Key Points:**
- For any triangle with sides a, b, c opposite angles A, B, C:
  a/sin(A) = b/sin(B) = c/sin(C).
- Used when you know: AAS, ASA, or SSA (ambiguous case).
- Ambiguous case (SSA): zero, one, or two triangles possible.
- Always check: does the given information yield a valid triangle?

**Formulas:**
- a/sin(A) = b/sin(B) = c/sin(C)
- Area = (1/2)ab·sin(C)

**Flashcards:**
- Q: State the Law of Sines.
  A: a/sinA = b/sinB = c/sinC.
- Q: When is the Law of Sines ambiguous?
  A: In the SSA case — you might get 0, 1, or 2 valid triangles.
- Q: Find side b if A = 30°, B = 45°, a = 10.
  A: b = 10·sin(45°)/sin(30°) = 10·(√2/2)/(1/2) = 10√2 ≈ 14.14.

**Quiz:**
- Q: The Law of Sines is useful when you know:
  Options: A) SSS  B) SAS  C) AAS  D) All of these
  Answer: C) AAS

---

### B8. Law of Cosines
**Status:** Not in current site. Trig textbook Section 11.3.

**Key Points:**
- For any triangle: c² = a² + b² - 2ab·cos(C).
- Used when you know: SAS or SSS.
- Reduces to Pythagorean theorem when C = 90°.
- Can also find angles from three known sides by rearranging: cos(C) = (a² + b² - c²)/(2ab).

**Formulas:**
- c² = a² + b² - 2ab·cos(C)
- cos(C) = (a² + b² - c²)/(2ab)

**Flashcards:**
- Q: State the Law of Cosines.
  A: c² = a² + b² - 2ab·cos(C).
- Q: If a = 5, b = 7, C = 60°, find c.
  A: c² = 25 + 49 - 2(5)(7)cos(60°) = 74 - 35 = 39. c = √39 ≈ 6.24.
- Q: When does the Law of Cosines reduce to the Pythagorean theorem?
  A: When C = 90° (cos90° = 0), so c² = a² + b².

**Quiz:**
- Q: Given a = 8, b = 6, c = 10, find angle C.
  Options: A) 90°  B) 60°  C) 120°  D) 45°
  Answer: A) 90° [cos(C) = (64+36-100)/96 = 0]

**🎴 Yu-Gi-Oh! Crossover: Damage Calculation as Triangle Solving**
Battle damage in Yu-Gi-Oh! involves comparing ATK/DEF values, but imagine a more complex scenario with three interacting monsters (a triangular relationship). The Law of Cosines is like calculating the "effective damage" when two stat values and the "angle" between them (game mechanic interaction) are known. The Law of Sines lets you find unknown stats from known ratios — like back-calculating a monster's original ATK from the battle damage dealt.

---

### B9. Polar Coordinates
**Status:** Not in current site. Trig textbook Section 11.4-11.5.

**Key Points:**
- A point in polar: (r, θ) where r = distance from origin, θ = angle from positive x-axis.
- Conversion: x = r·cos(θ), y = r·sin(θ), r² = x² + y², tan(θ) = y/x.
- Same point has infinitely many polar representations: (r, θ + 2πk) and (-r, θ + π + 2πk).
- Polar graphs: circles, cardioids, rose curves, limaçons, lemniscates.
- Rose curve r = a·cos(nθ): n petals if n odd, 2n petals if n even.

**Flashcards:**
- Q: Convert (3, π/4) from polar to Cartesian.
  A: x = 3cos(π/4) = 3√2/2, y = 3sin(π/4) = 3√2/2.
- Q: Convert (1, 1) from Cartesian to polar.
  A: r = √2, θ = arctan(1) = π/4. Polar: (√2, π/4).
- Q: How many petals does r = 3cos(4θ) have?
  A: 8 (2n = 2·4 = 8, since n is even).

**Quiz:**
- Q: The Cartesian coordinates of the polar point (4, π/3) are:
  Options: A) (2, 2√3)  B) (2√3, 2)  C) (4, 4)  D) (2, 2)
  Answer: A) (2, 2√3)

---

### B10. Vectors
**Status:** Not in current site. Trig textbook Section 11.8-11.9.

**Key Points:**
- A vector has magnitude and direction: v = ⟨a, b⟩.
- Magnitude: ||v|| = √(a² + b²).
- Unit vector: v/||v||.
- Vector operations: addition ⟨a₁+a₂, b₁+b₂⟩, scalar multiplication ⟨ca, cb⟩.
- Dot product: v · w = a₁a₂ + b₁b₂ = ||v|| ||w|| cos(θ).
- Angle between vectors: cos(θ) = (v · w)/(||v|| ||w||).
- Perpendicular vectors: v · w = 0.
- Projection of v onto w: proj_w(v) = [(v · w)/(w · w)] · w.
- Work: W = F · d = ||F|| ||d|| cos(θ).

**Flashcards:**
- Q: Find the magnitude of v = ⟨3, 4⟩.
  A: ||v|| = √(9 + 16) = 5.
- Q: Find the dot product of ⟨2, -1⟩ and ⟨3, 4⟩.
  A: 2(3) + (-1)(4) = 6 - 4 = 2.
- Q: When are two vectors perpendicular?
  A: When their dot product equals zero.

**Quiz:**
- Q: What is the dot product of ⟨1, 2⟩ and ⟨-2, 1⟩?
  Options: A) 0  B) 4  C) -4  D) 2
  Answer: A) 0 (they are perpendicular)
- Q: The work done by a force F = 10 lbs at 30° over 50 ft is:
  Options: A) 250√3  B) 500  C) 250  D) 125√3
  Answer: A) 250√3

---

### B11. Parametric Equations
**Status:** Not in current site. Trig textbook Section 11.10.

**Key Points:**
- System: x = f(t), y = g(t), where t is the parameter.
- The parameter adds orientation (direction of travel) to a curve.
- Eliminating the parameter: solve one equation for t, substitute into the other.
- Common parametrizations:
  - Line from (x₀,y₀) to (x₁,y₁): x = x₀ + (x₁-x₀)t, y = y₀ + (y₁-y₀)t, 0 ≤ t ≤ 1.
  - Circle: x = h + r·cos(t), y = k + r·sin(t), 0 ≤ t ≤ 2π.
  - Ellipse: x = h + a·cos(t), y = k + b·sin(t).
- Parametric equations are foundational for computer graphics and VR world-building.

**Flashcards:**
- Q: Eliminate the parameter from x = t², y = 2t + 1.
  A: From y: t = (y-1)/2. Substituting: x = ((y-1)/2)² = (y-1)²/4. So 4x = (y-1)².
- Q: Parametrize the line segment from (1, 3) to (4, 7).
  A: x = 1 + 3t, y = 3 + 4t, for 0 ≤ t ≤ 1.
- Q: What do parametric equations add that y = f(x) doesn't?
  A: Direction/orientation and the ability to represent curves that aren't functions.

**Quiz:**
- Q: The parametric equations x = 3cos(t), y = 3sin(t) trace out:
  Options: A) A line  B) A parabola  C) A circle of radius 3  D) An ellipse
  Answer: C) A circle of radius 3

**🎴 Yu-Gi-Oh! Crossover: Turn Sequence as Parametric Equations**
A Yu-Gi-Oh! duel's game state can be described parametrically with "turn number" as the parameter t. At each t, the player's LP = f(t), hand size = g(t), field state = h(t). The parameter t gives the game an *orientation* (you can't go backwards), just like parametric equations give a curve a direction. Eliminating the parameter is like summarizing a whole duel replay into just "final LP vs. cards used" — you lose the turn-by-turn sequence.

---

### B12. Polar Form of Complex Numbers
**Status:** Not in current site. Trig textbook Section 11.7.

**Key Points:**
- Complex number z = a + bi can be written as z = r(cosθ + i·sinθ) = r·cis(θ).
- r = |z| = √(a² + b²), θ = arg(z) = arctan(b/a).
- Multiplication: r₁cis(θ₁) · r₂cis(θ₂) = r₁r₂ · cis(θ₁ + θ₂).
- Division: (r₁/r₂) · cis(θ₁ - θ₂).
- De Moivre's Theorem: [r·cis(θ)]ⁿ = rⁿ · cis(nθ).
- nth roots of a complex number: n equally-spaced points on a circle of radius r^(1/n).

**Flashcards:**
- Q: Write z = 1 + i in polar form.
  A: r = √2, θ = π/4. z = √2 · cis(π/4).
- Q: State De Moivre's Theorem.
  A: [r·cis(θ)]ⁿ = rⁿ · cis(nθ).
- Q: Multiply 2cis(π/3) and 3cis(π/6).
  A: 6·cis(π/3 + π/6) = 6·cis(π/2) = 6i.

**Quiz:**
- Q: The modulus of z = 3 + 4i is:
  Options: A) 5  B) 7  C) √7  D) 25
  Answer: A) 5

---

### B13. Applications of Sinusoids / Harmonic Motion
**Status:** Site has basic sinusoidal model formula. Missing: applications — Ferris wheels, springs, sound waves, daylight models, harmonic motion.

**Key Points:**
- S(t) = A·sin(ωt - φ) + B models periodic real-world phenomena.
- Amplitude A: maximum displacement from baseline.
- Angular frequency ω = 2π/period. Ordinary frequency f = ω/(2π).
- Phase shift: -φ/ω. Vertical shift (baseline): B.
- Harmonic motion: x(t) = A·sin(ωt + φ) models spring/pendulum motion.
- ω for a spring: ω = √(k/m), where k = spring constant, m = mass.
- Fitting sinusoidal models to data: estimate A, B, ω, φ from max/min/period.

**Flashcards:**
- Q: A Ferris wheel has diameter 128 ft and completes 2 revolutions in 127 seconds. What is the angular frequency?
  A: ω = 2·(2π)/127 = 4π/127 rad/s.
- Q: How do you find amplitude from a graph?
  A: Amplitude = (max - min)/2.
- Q: What is the midline of a sinusoid with max 80 and min 20?
  A: Midline = (80 + 20)/2 = 50.

**Quiz:**
- Q: The period of S(t) = 5sin(πt/3) is:
  Options: A) 6  B) 3  C) π/3  D) 2π/3
  Answer: A) 6 [Period = 2π/(π/3) = 6]

---

### B14. Conic Sections in Polar Form / Rotation of Axes
**Status:** Not in current site. Trig textbook Section 11.6.

**Key Points:**
- Polar form of conics: r = ed/(1 ± e·cos(θ)) or r = ed/(1 ± e·sin(θ)).
  - e < 1: ellipse. e = 1: parabola. e > 1: hyperbola.
- Rotation of axes removes the xy-term from Ax² + Bxy + Cy² + Dx + Ey + F = 0.
- Rotation angle: cot(2α) = (A - C)/B.
- After rotation: new coordinates X, Y are related by x = Xcosα - Ysinα, y = Xsinα + Ycosα.

**Flashcards:**
- Q: What determines if a polar conic is an ellipse, parabola, or hyperbola?
  A: The eccentricity e: e < 1 → ellipse, e = 1 → parabola, e > 1 → hyperbola.
- Q: What is the rotation angle formula for eliminating an xy-term?
  A: cot(2α) = (A - C)/B.

**Quiz:**
- Q: A conic with eccentricity e = 0.5 is:
  Options: A) Circle  B) Ellipse  C) Parabola  D) Hyperbola
  Answer: B) Ellipse

---

# PART 2: IMPLEMENTATION PRIORITY & SUMMARY

## Priority Tiers

| Tier | Topics | Rationale |
|------|--------|-----------|
| **Tier 1 (Essential)** | A1 (Domain/Range), A3 (Composition), A5 (Polynomials Deep), A6 (Quadratics Expanded), A7 (Factor/Remainder Theorem), B2 (Six Trig Functions), B3 (Trig Identities), B5 (Inverse Trig), B6 (Trig Equations) | These are foundational for calculus readiness and appear most on exams |
| **Tier 2 (Important)** | A2 (Rates of Change), A8 (Rational Roots), A9 (Complex Zeros), A10 (Rational Functions Deep), A12-A13 (Exp/Log Expanded), B1 (Angles Expanded), B4 (Trig Graphs), B7-B8 (Law of Sines/Cosines) | Strong supporting material for problem solving |
| **Tier 3 (Advanced)** | A11 (Inverses/Radicals), B9 (Polar), B10 (Vectors), B11 (Parametric), B12 (Polar Complex), B13 (Harmonic Motion), B14 (Polar Conics) | Important for full precalc coverage but more specialized |

## Content Counts

| Category | New Topics | New Flashcards | New Quiz Questions |
|----------|-----------|----------------|-------------------|
| Precalc Gaps (A1-A13) | 13 | ~45 | ~30 |
| Trig Gaps (B1-B14) | 14 | ~45 | ~30 |
| Yu-Gi-Oh! Crossovers | ~10 subsections | — | — |
| **TOTAL** | **27 new topics** | **~90 new flashcards** | **~60 new quiz questions** |

