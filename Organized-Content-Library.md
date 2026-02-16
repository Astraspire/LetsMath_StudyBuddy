# Precalc & Calculus Master Content Library
# ============================================
# Uniformly tagged resource file for coding agent consumption.
#
# ## Tagging Schema
#
# Every item carries an HTML comment tag block with these fields:
#   - `id:`        Unique identifier code (R-ALG-01, FC-TRIG-03, QZ-CALC-07, etc.)
#   - `course:`    precalc | calculus
#   - `area:`      algebra | trig | calculus | precalc-general
#   - `type:`      review-card | expansion-review | flashcard | quiz
#   - `subtopic:`  Finer-grained label (e.g., functions-notation, unit-circle)
#   - `tier:`      1-essential | 2-important | 3-advanced  (expansion items only)
#   - `code:`      A1–A13, B1–B14 (expansion items only)
#   - `yugioh:`    yes | no  (whether Yu-Gi-Oh! crossover exists)
#
# ## ID Format
#   R-{AREA}-{##}     Review Cards
#   E-{AREA}-{##}     Expansion Review Cards
#   FC-{AREA}-{##}    Flashcards
#   QZ-{AREA}-{##}    Quiz Questions
#
# ## Area Abbreviations
#   ALG = algebra, TRIG = trigonometry, CALC = calculus, GEN = precalc-general
#
# Source: Study-Buddy_App.html
# Generated: 2026-02-16

---

# PART 1 — REVIEW CARDS
# ======================

---

## 1A. Algebra Review Cards

<!-- tags: id:R-ALG-01, course:precalc, area:algebra, type:review-card, subtopic:functions-notation -->
### R-ALG-01 · Functions and Notation
- f(x) means "plug x into the expression".
- f(3) = replace every x with 3.
- f(a + h) = replace x with (a + h).
- Domain: all valid x-values (watch for division by zero, sqrt of negatives, log issues).
- Range: all possible y-values.

<!-- tags: id:R-ALG-02, course:precalc, area:algebra, type:review-card, subtopic:factoring -->
### R-ALG-02 · Factoring Patterns
- Difference of squares: a^2 - b^2 = (a + b)(a - b)
- Perfect square: a^2 +/- 2ab + b^2 = (a +/- b)^2
- Sum/difference of cubes: a^3 +/- b^3 = (a +/- b)(a^2 -/+ ab + b^2)

<!-- tags: id:R-ALG-03, course:precalc, area:algebra, type:review-card, subtopic:quadratics -->
### R-ALG-03 · Solving Quadratics
- Quadratic formula: x = (-b +/- sqrt(b^2 - 4ac)) / (2a)
- Discriminant: Delta = b^2 - 4ac
  - Delta > 0: two real solutions
  - Delta = 0: one solution
  - Delta < 0: no real solutions

<!-- tags: id:R-ALG-04, course:precalc, area:algebra, type:review-card, subtopic:algebra-manipulation -->
### R-ALG-04 · More Algebra Skills
- Completing the square:
  - x^2 + bx -> x^2 + bx + (b/2)^2 - (b/2)^2 = (x + b/2)^2 - (b/2)^2
  - Example: x^2 + 6x + 1 = 0 -> (x + 3)^2 = 8 -> x = -3 +/- 2*sqrt(2)
- Rationalizing denominators:
  - 1/sqrt(a) -> multiply by sqrt(a)/sqrt(a)
  - 1/(a + sqrt(b)) -> multiply by (a - sqrt(b))/(a - sqrt(b))
  - Use the conjugate to eliminate radicals in the denominator.

<!-- tags: id:R-ALG-05, course:precalc, area:algebra, type:review-card, subtopic:rational-functions -->
### R-ALG-05 · Rational Functions
- Vertical asymptotes: set denominator = 0.
- Horizontal asymptotes:
  - deg(P) < deg(Q) -> y = 0
  - deg(P) = deg(Q) -> y = leading coefficient ratio
  - deg(P) > deg(Q) -> none

<!-- tags: id:R-ALG-06, course:precalc, area:algebra, type:review-card, subtopic:inverse-functions -->
### R-ALG-06 · Inverse Functions
- Steps:
  1. Write y = f(x)
  2. Swap x and y
  3. Solve for y
  4. Write f^-1(x)
- Graphs are reflections across y = x.

<!-- tags: id:R-ALG-07, course:precalc, area:algebra, type:review-card, subtopic:linear-functions -->
### R-ALG-07 · Lines and Slopes
- Slope: m = (y2 - y1) / (x2 - x1)
- Forms of linear equations:
  - Slope-intercept: y = mx + b
  - Point-slope: y - y1 = m(x - x1)
  - Standard: Ax + By = C
- Parallel lines: same slope (m1 = m2)
- Perpendicular lines: negative reciprocal slopes (m1 * m2 = -1)

<!-- tags: id:R-ALG-08, course:precalc, area:algebra, type:review-card, subtopic:absolute-value-piecewise -->
### R-ALG-08 · Absolute Value and Piecewise
- |x| = x if x >= 0, and -x if x < 0
- Solving |expression| = k:
  - expression = k OR expression = -k
- Absolute value inequalities:
  - |expr| < k -> -k < expr < k
  - |expr| > k -> expr < -k OR expr > k
- Piecewise functions: choose the rule based on the domain condition.

<!-- tags: id:R-ALG-09, course:precalc, area:algebra, type:review-card, subtopic:transformations -->
### R-ALG-09 · Function Transformations
- y = a * f(b(x - h)) + k
  - k: vertical shift
  - h: horizontal shift
  - a: vertical stretch/compress
  - b: horizontal compress/stretch
- Reflections:
  - -f(x): reflect over x-axis
  - f(-x): reflect over y-axis
- Inside changes affect x (opposite direction); outside changes affect y (same direction).

<!-- tags: id:R-ALG-10, course:precalc, area:algebra, type:review-card, subtopic:inequalities -->
### R-ALG-10 · Inequalities
- Linear inequalities: flip the sign when multiplying or dividing by a negative.
- Polynomial/rational inequalities (sign chart):
  1. Move everything to one side (>= 0 or <= 0)
  2. Factor completely
  3. Find critical values (zeros/undefined points)
  4. Test signs in each interval
  5. Select intervals that satisfy the inequality
- Interval notation:
  - (a, b) open, [a, b] closed
  - (-inf, a) union (b, inf)

<!-- tags: id:R-ALG-11, course:precalc, area:algebra, type:review-card, subtopic:exponentials-logs -->
### R-ALG-11 · Exponentials and Logs
- Core relationship: a^x = y <-> log_a(y) = x
- Natural base: e^x = y <-> ln(y) = x
- Exponentials and logs are inverse operations.

<!-- tags: id:R-ALG-12, course:precalc, area:algebra, type:review-card, subtopic:log-properties -->
### R-ALG-12 · Log Properties
- Product: log(MN) = log(M) + log(N)
- Quotient: log(M/N) = log(M) - log(N)
- Power: log(M^k) = k * log(M)
- Wrong rule: ln(a + b) != ln(a) + ln(b)

<!-- tags: id:R-ALG-13, course:precalc, area:algebra, type:review-card, subtopic:sequences-series -->
### R-ALG-13 · Sequences and Series
- Arithmetic sequence (constant difference d):
  - an = a1 + (n - 1)d
  - Sum: Sn = n(a1 + an)/2
- Geometric sequence (constant ratio r):
  - an = a1 * r^(n-1)
  - Sum: Sn = a1(1 - r^n) / (1 - r)
- Infinite geometric series converges when |r| < 1:
  - S = a1 / (1 - r)

---

## 1B. Trigonometry Review Cards

<!-- tags: id:R-TRIG-01, course:precalc, area:trig, type:review-card, subtopic:unit-circle -->
### R-TRIG-01 · The Unit Circle
- Radius 1, centered at origin. Every point is (cos(theta), sin(theta)).
- Degree/radian conversion:
  - radians = (pi/180) * degrees
  - degrees = (180/pi) * radians
- Key angles table:

| Degrees | Radians | cos(theta) | sin(theta) | tan(theta) |
| --- | --- | --- | --- | --- |
| 0 | 0 | 1 | 0 | 0 |
| 30 | pi/6 | sqrt(3)/2 | 1/2 | sqrt(3)/3 |
| 45 | pi/4 | sqrt(2)/2 | sqrt(2)/2 | 1 |
| 60 | pi/3 | 1/2 | sqrt(3)/2 | sqrt(3) |
| 90 | pi/2 | 0 | 1 | undef |
| 120 | 2pi/3 | -1/2 | sqrt(3)/2 | -sqrt(3) |
| 135 | 3pi/4 | -sqrt(2)/2 | sqrt(2)/2 | -1 |
| 150 | 5pi/6 | -sqrt(3)/2 | 1/2 | -sqrt(3)/3 |
| 180 | pi | -1 | 0 | 0 |
| 270 | 3pi/2 | 0 | -1 | undef |
| 360 | 2pi | 1 | 0 | 0 |

- Highlighted key angles to memorize: 0, 30, 45, 60, 90, 180, 360 degrees.

<!-- tags: id:R-TRIG-02, course:precalc, area:trig, type:review-card, subtopic:quick-trig-reference -->
### R-TRIG-02 · Quick Trig Reference

| Angle | sin | cos | tan |
| --- | --- | --- | --- |
| 0 / pi/2 | 0 / 1 | 1 / 0 | 0 / undef |
| pi/6 (30) | 1/2 | sqrt(3)/2 | sqrt(3)/3 |
| pi/4 (45) | sqrt(2)/2 | sqrt(2)/2 | 1 |
| pi/3 (60) | sqrt(3)/2 | 1/2 | sqrt(3) |

<!-- tags: id:R-TRIG-03, course:precalc, area:trig, type:review-card, subtopic:trig-identities -->
### R-TRIG-03 · Key Identities
- sin^2(x) + cos^2(x) = 1
- tan(x) = sin(x) / cos(x)
- sin(2x) = 2 sin(x) cos(x)
- Even/odd:
  - sin(-x) = -sin(x)
  - cos(-x) = cos(x)

<!-- tags: id:R-TRIG-04, course:precalc, area:trig, type:review-card, subtopic:sinusoidal-models -->
### R-TRIG-04 · Sinusoidal Models
- y = A sin(bx + c) + D
  - A = amplitude
  - b = 2pi / period
  - D = vertical shift (midline)

<!-- tags: id:R-TRIG-05, course:precalc, area:trig, type:review-card, subtopic:unit-circle-deep -->
### R-TRIG-05 · Understanding the Unit Circle (Deep Dive)
- Unit circle: radius 1 centered at (0, 0). Every point is (cos(theta), sin(theta)).
- Key insight: x-coordinate = cos(theta), y-coordinate = sin(theta).
- Conversion formulas:
  - Radians to degrees: degrees = (180/pi) * radians
  - Degrees to radians: radians = (pi/180) * degrees
- Key angles to memorize: 0, 30 (pi/6), 45 (pi/4), 60 (pi/3), 90 (pi/2).

<!-- tags: id:R-TRIG-06, course:precalc, area:trig, type:review-card, subtopic:complete-unit-circle -->
### R-TRIG-06 · Complete Unit Circle Reference Table

| Degrees | Radians | cos(theta) | sin(theta) | tan(theta) | Quadrant |
| --- | --- | --- | --- | --- | --- |
| 0 | 0 | 1 | 0 | 0 | Start (positive x-axis) |
| 30 | pi/6 | sqrt(3)/2 | 1/2 | sqrt(3)/3 | QI (key angle) |
| 45 | pi/4 | sqrt(2)/2 | sqrt(2)/2 | 1 | QI (key angle) |
| 60 | pi/3 | 1/2 | sqrt(3)/2 | sqrt(3) | QI (key angle) |
| 90 | pi/2 | 0 | 1 | undefined | Positive y-axis |
| 120 | 2pi/3 | -1/2 | sqrt(3)/2 | -sqrt(3) | QII |
| 135 | 3pi/4 | -sqrt(2)/2 | sqrt(2)/2 | -1 | QII |
| 150 | 5pi/6 | -sqrt(3)/2 | 1/2 | -sqrt(3)/3 | QII |
| 180 | pi | -1 | 0 | 0 | Negative x-axis |
| 210 | 7pi/6 | -sqrt(3)/2 | -1/2 | sqrt(3)/3 | QIII |
| 225 | 5pi/4 | -sqrt(2)/2 | -sqrt(2)/2 | 1 | QIII |
| 240 | 4pi/3 | -1/2 | -sqrt(3)/2 | sqrt(3) | QIII |
| 270 | 3pi/2 | 0 | -1 | undefined | Negative y-axis |
| 300 | 5pi/3 | 1/2 | -sqrt(3)/2 | -sqrt(3) | QIV |
| 315 | 7pi/4 | sqrt(2)/2 | -sqrt(2)/2 | -1 | QIV |
| 330 | 11pi/6 | sqrt(3)/2 | -1/2 | -sqrt(3)/3 | QIV |
| 360 | 2pi | 1 | 0 | 0 | Back to start |

<!-- tags: id:R-TRIG-07, course:precalc, area:trig, type:review-card, subtopic:quadrant-patterns -->
### R-TRIG-07 · Quadrant Patterns
- Quadrant I: all trig functions positive.
- Quadrant II: sin positive, cos and tan negative.
- Quadrant III: tan positive, sin and cos negative.
- Quadrant IV: cos positive, sin and tan negative.
- Study tip: master Quadrant I first, then use reference angles and sign patterns.

---

## 1C. Calculus Preview Review Cards

<!-- tags: id:R-CALC-01, course:precalc, area:calculus, type:review-card, subtopic:limits-preview -->
### R-CALC-01 · Limits (Calculus Preview)
- Core idea: what value does f(x) approach as x -> c?
- Strategy:
  1. Try direct substitution
  2. If 0/0, factor/cancel/rationalize
  3. For limits at infinity, divide by highest power of x
- Key facts:
  - lim(x->0) sin(x)/x = 1
  - lim(x->inf) 1/x^n = 0 for n > 0
  - lim(x->a) [polynomial] = substitute a

<!-- tags: id:R-CALC-02, course:precalc, area:calculus, type:review-card, subtopic:what-is-a-function -->
### R-CALC-02 · What Is a Function?
- Relationship between domain (inputs) and codomain (outputs), one output per input.
- Vertical line test.
- Descriptions: algebraic, graphical, numerical, verbal.
- Types: polynomial, rational, exponential, logarithmic, trigonometric.
- Example: f(x) = 2x + 3 (linear, slope 2, y-intercept 3).

<!-- tags: id:R-CALC-03, course:precalc, area:calculus, type:review-card, subtopic:what-is-a-limit -->
### R-CALC-03 · What Is a Limit?
- lim(x->a) f(x) = L.
- Two-sided and one-sided limits.
- Techniques: direct substitution, factoring, rationalizing.
- Example: lim(x->1) (x^2 - 1)/(x - 1) = 2.

<!-- tags: id:R-CALC-04, course:precalc, area:calculus, type:review-card, subtopic:what-is-a-derivative -->
### R-CALC-04 · What Is a Derivative?
- f'(x) = lim(h->0) [f(x+h) - f(x)] / h
- Interpretations: tangent slope, instantaneous rate of change.
- Rules: power, product, quotient, chain.
- Example: f(x) = x^2 -> f'(x) = 2x, slope at x=2 is 4.

<!-- tags: id:R-CALC-05, course:precalc, area:calculus, type:review-card, subtopic:what-is-an-integral -->
### R-CALC-05 · What Is an Integral?
- Integral from a to b is area under the curve.
- Definite vs indefinite integrals.
- Techniques: antiderivatives, substitution, integration by parts, partial fractions.
- Example: int_0^1 x^2 dx = 1/3.

<!-- tags: id:R-CALC-06, course:precalc, area:calculus, type:review-card, subtopic:continuity -->
### R-CALC-06 · What Is Continuity?
- Conditions at x = a:
  1. f(a) defined
  2. lim(x->a) f(x) exists
  3. lim(x->a) f(x) = f(a)
- Discontinuities: removable, jump, infinite.
- Intermediate Value Theorem (IVT).

---

## 1D. Calculus Core Review Cards

<!-- tags: id:R-CALC-07, course:calculus, area:calculus, type:review-card, subtopic:quick-reference-chart -->
### R-CALC-07 · Quick Reference Chart

| Term | Meaning |
| --- | --- |
| Critical point | f'(x) = 0 or undefined |
| Increasing interval | f'(x) > 0 |
| Decreasing interval | f'(x) < 0 |
| Inflection point | f''(x) = 0 with sign change |
| Concave up | f''(x) > 0 |
| Concave down | f''(x) < 0 |

<!-- tags: id:R-CALC-08, course:calculus, area:calculus, type:review-card, subtopic:graph-reference -->
### R-CALC-08 · Graph Reference Key

| # | Location | Property | Description |
| --- | --- | --- | --- |
| 1 | Top center | Critical point | f'(x) = 0, local max |
| 2 | Upper right | Concave down | f''(x) < 0 |
| 3 | Left side | Increasing | f'(x) > 0 |
| 4 | Lower left | Concave down | f''(x) < 0 |
| 5 | Bottom center | Critical point | f'(x) = 0, local min |
| 6 | Lower right | Concave down | f''(x) < 0 |
| 7 | Right side | Decreasing | f'(x) < 0 |
| 8 | Upper left | Inflection point | f''(x) = 0 with sign change |

<!-- tags: id:R-CALC-09, course:calculus, area:calculus, type:review-card, subtopic:definitions -->
### R-CALC-09 · Definitions

| Term | Condition | Meaning |
| --- | --- | --- |
| Critical point | f'(x) = 0 | Horizontal tangent (max/min) |
| Increasing | f'(x) > 0 | Function rising |
| Decreasing | f'(x) < 0 | Function falling |
| Inflection point | f''(x) = 0 (sign change) | Concavity changes |
| Concave up | f''(x) > 0 | Curves upward |
| Concave down | f''(x) < 0 | Curves downward |

<!-- tags: id:R-CALC-10, course:calculus, area:calculus, type:review-card, subtopic:rolles-theorem -->
### R-CALC-10 · Rolle's Theorem
- Conditions:
  1. f continuous on [a, b]
  2. f differentiable on (a, b)
  3. f(a) = f(b)
- If all 3 hold, there exists c in (a, b) with f'(c) = 0.

<!-- tags: id:R-CALC-11, course:calculus, area:calculus, type:review-card, subtopic:mean-value-theorem -->
### R-CALC-11 · Mean Value Theorem (MVT)
- Conditions:
  1. f continuous on [a, b]
  2. f differentiable on (a, b)
- There exists c in (a, b) with f'(c) = (f(b) - f(a)) / (b - a).

<!-- tags: id:R-CALC-12, course:calculus, area:calculus, type:review-card, subtopic:corollaries -->
### R-CALC-12 · Corollaries
- If f'(x) = 0 for all x in I, then f(x) is constant on I.
- If f'(x) = g'(x) for all x in I, then f(x) = g(x) + C.
- If f'(x) > 0 on (a, b), f increases on [a, b]. If f'(x) < 0 on (a, b), f decreases on [a, b].

<!-- tags: id:R-CALC-13, course:calculus, area:calculus, type:review-card, subtopic:first-derivative-test -->
### R-CALC-13 · First Derivative Test
- f' changes + -> - at c: local maximum
- f' changes - -> + at c: local minimum
- f' same sign on both sides: neither

<!-- tags: id:R-CALC-14, course:calculus, area:calculus, type:review-card, subtopic:second-derivative-test -->
### R-CALC-14 · Second Derivative Test
- Steps:
  1. Find critical points from f'(x) = 0
  2. Compute f''(x)
  3. Evaluate f''(c)
- f''(c) > 0 -> local minimum
- f''(c) < 0 -> local maximum
- f''(c) = 0 -> inconclusive (use first derivative test)

<!-- tags: id:R-CALC-15, course:calculus, area:calculus, type:review-card, subtopic:graphing-with-derivatives -->
### R-CALC-15 · Graphing with Derivatives
- Step 1: Find f'(x); locate critical points and increasing/decreasing intervals.
- Step 2: Find f''(x); locate inflection points and concavity.
- Step 3: Analyze sign charts for f'(x), f''(x).
- Step 4: Identify key points (local max/min, inflection).
- Step 5: Sketch using behavior info.

<!-- tags: id:R-CALC-16, course:calculus, area:calculus, type:review-card, subtopic:integration-formulas -->
### R-CALC-16 · Integration Formulas

| Differentiation | Indefinite Integral |
| --- | --- |
| d/dx (k) = 0 | int k dx = kx + C |
| d/dx (x^n) = n x^(n-1) | int x^n dx = x^(n+1)/(n+1) + C, n != -1 |
| d/dx (ln|x|) = 1/x | int (1/x) dx = ln|x| + C |
| d/dx (e^x) = e^x | int e^x dx = e^x + C |
| d/dx (sin x) = cos x | int cos x dx = sin x + C |
| d/dx (cos x) = -sin x | int sin x dx = -cos x + C |
| d/dx (tan x) = sec^2 x | int sec^2 x dx = tan x + C |
| d/dx (csc x) = -csc x cot x | int csc x cot x dx = -csc x + C |
| d/dx (sec x) = sec x tan x | int sec x tan x dx = sec x + C |
| d/dx (cot x) = -csc^2 x | int csc^2 x dx = -cot x + C |
| d/dx (sin^-1 x) = 1/sqrt(1 - x^2) | int 1/sqrt(1 - x^2) dx = sin^-1 x + C |
| d/dx (tan^-1 x) = 1/(1 + x^2) | int 1/(1 + x^2) dx = tan^-1 x + C |
| d/dx (sec^-1 |x|) = 1/(x * sqrt(x^2 - 1)) | int 1/(x * sqrt(x^2 - 1)) dx = sec^-1 |x| + C |

---

## 1E. General Precalc Review Cards

<!-- tags: id:R-GEN-01, course:precalc, area:precalc-general, type:review-card, subtopic:common-mistakes -->
### R-GEN-01 · Common Mistakes to Avoid
- ln(a + b) != ln(a) + ln(b)
- (a + b)^2 != a^2 + b^2 -> a^2 + 2ab + b^2
- sqrt(a^2 + b^2) != a + b
- 1/(a + b) != 1/a + 1/b
- Also watch out for:
  - forgetting to flip inequality sign when multiplying/dividing by a negative
  - ignoring domain restrictions (division by 0, sqrt of negatives, log of <= 0)
  - dropping parentheses: -3^2 = -9 but (-3)^2 = 9

<!-- tags: id:R-GEN-02, course:precalc, area:precalc-general, type:review-card, subtopic:calculator-skills -->
### R-GEN-02 · Calculator Skills
- Essential buttons: sin, cos, tan, sin^-1, cos^-1, tan^-1, ln, log, e^x, 10^x, x^2, sqrt, pi, ^
- Always check degree vs radian mode (use radian for calculus).
- Change of base: log_a(M) = ln(M) / ln(a)
- Parentheses matter: -3^2 = -9 vs (-3)^2 = 9

---
---

# PART 2 — EXPANSION REVIEW CARDS (A1–A13, B1–B14)
# ===================================================

---

## 2A. Precalculus Expansion (A1–A13)

### Tier 1 (Essential)

<!-- tags: id:E-ALG-01, course:precalc, area:algebra, type:expansion-review, code:A1, tier:1-essential, subtopic:domain-range, yugioh:yes -->
### E-ALG-01 · A1. Domain & Range
- Interval notation, set-builder notation, toolkit function domains, piecewise functions
- Three main domain restrictions: division by zero, even roots of negatives, log of non-positives
- Formulas: reciprocal, square root, reciprocal squared domain/range examples

<!-- tags: id:E-ALG-02, course:precalc, area:algebra, type:expansion-review, code:A3, tier:1-essential, subtopic:function-composition, yugioh:yes -->
### E-ALG-02 · A3. Function Composition
- Composition notation (f∘g)(x) = f(g(x)), evaluating from tables/graphs/formulas
- Domain of compositions: x in domain of g AND g(x) in domain of f
- Decomposition of complex functions; order matters: f(g(x)) != g(f(x))

<!-- tags: id:E-ALG-03, course:precalc, area:algebra, type:expansion-review, code:A5, tier:1-essential, subtopic:polynomials-deep, yugioh:yes -->
### E-ALG-03 · A5. Power Functions & Polynomial Functions (Deep Dive)
- Power functions, end behavior (4 cases by degree parity & leading coefficient sign)
- Max n intercepts, max n-1 turning points for degree-n polynomial
- Multiplicity of zeros: 1 → crosses, 2 → bounces, 3 → cubic flattening

<!-- tags: id:E-ALG-04, course:precalc, area:algebra, type:expansion-review, code:A6, tier:1-essential, subtopic:quadratics-expanded -->
### E-ALG-04 · A6. Quadratic Functions (Expanded)
- Vertex form f(x) = a(x-h)^2+k, completing the square, vertex formula h = -b/(2a)
- Parabola opens up (a>0) → min; opens down (a<0) → max
- Applications: area, revenue, projectile motion optimization

<!-- tags: id:E-ALG-05, course:precalc, area:algebra, type:expansion-review, code:A7, tier:1-essential, subtopic:factor-remainder, yugioh:yes -->
### E-ALG-05 · A7. Factor Theorem, Remainder Theorem & Synthetic Division
- Remainder Theorem: p(x) / (x-c) remainder = p(c)
- Factor Theorem: (x-c) is factor iff p(c) = 0
- Polynomial long division and synthetic division procedures

### Tier 2 (Important)

<!-- tags: id:E-ALG-06, course:precalc, area:precalc-general, type:expansion-review, code:A2, tier:2-important, subtopic:rates-of-change -->
### E-ALG-06 · A2. Rates of Change & Behavior of Graphs
- Average rate of change = [f(b)-f(a)]/(b-a)
- Increasing/decreasing intervals, local max/min definitions
- Concave up vs concave down, inflection points

<!-- tags: id:E-ALG-07, course:precalc, area:algebra, type:expansion-review, code:A4, tier:2-important, subtopic:linear-functions -->
### E-ALG-07 · A4. Linear Functions (Detailed Treatment)
- f(x) = mx + b, modeling, slope interpretation in context
- Finding equations from two points, point-slope form
- Parallel lines (same slope), perpendicular lines (negative reciprocal)

<!-- tags: id:E-ALG-08, course:precalc, area:algebra, type:expansion-review, code:A8, tier:2-important, subtopic:real-zeros -->
### E-ALG-08 · A8. Real Zeros of Polynomials
- Cauchy's Bound for locating real zeros
- Rational Roots Theorem: p divides constant term, q divides leading coefficient
- Strategy: list candidates → synthetic division → quadratic formula on remainder

<!-- tags: id:E-ALG-09, course:precalc, area:algebra, type:expansion-review, code:A9, tier:2-important, subtopic:complex-zeros, yugioh:yes -->
### E-ALG-09 · A9. Complex Zeros
- Imaginary unit i = sqrt(-1), complex number a + bi, conjugate a - bi
- Fundamental Theorem of Algebra: degree-n polynomial has exactly n complex zeros
- Complex zeros of real-coefficient polynomials come in conjugate pairs

<!-- tags: id:E-ALG-10, course:precalc, area:algebra, type:expansion-review, code:A10, tier:2-important, subtopic:rational-functions-deep -->
### E-ALG-10 · A10. Rational Functions (Deep Dive)
- Vertical asymptotes, holes (common factors), horizontal asymptote rules
- Oblique/slant asymptotes when degree numerator = degree denominator + 1
- Writing equations from graphs: intercepts, asymptotes, stretch factor

<!-- tags: id:E-ALG-11, course:precalc, area:algebra, type:expansion-review, code:A12, tier:2-important, subtopic:exponential-models, yugioh:yes -->
### E-ALG-11 · A12. Exponential Functions (Expanded)
- Growth: f(t) = a*b^t (b>1), decay (0<b<1), continuous: A = Pe^(rt)
- Compound interest: A = P(1+r/n)^(nt)
- Doubling time: t = ln(2)/r; half-life: t = ln(2)/|r|

<!-- tags: id:E-ALG-12, course:precalc, area:algebra, type:expansion-review, code:A13, tier:2-important, subtopic:logarithmic-models -->
### E-ALG-12 · A13. Logarithmic Functions (Expanded)
- log_a(x) defined for x > 0, graph passes through (1,0), VA at x = 0
- Solving log equations: convert to exponential form, condense/expand
- Applications: pH, Richter scale, decibels; change of base formula

### Tier 3 (Advanced)

<!-- tags: id:E-ALG-13, course:precalc, area:algebra, type:expansion-review, code:A11, tier:3-advanced, subtopic:inverses-radicals -->
### E-ALG-13 · A11. Inverses & Radical Functions
- Restricting domains for non-one-to-one functions before finding inverses
- Inverse of x^2 (x>=0) is sqrt(x)
- Radical equations: isolate, raise to power, check for extraneous solutions

---

## 2B. Trigonometry Expansion (B1–B14)

### Tier 1 (Essential)

<!-- tags: id:E-TRIG-01, course:precalc, area:trig, type:expansion-review, code:B2, tier:1-essential, subtopic:six-functions-identities -->
### E-TRIG-01 · B2. The Six Circular Functions & Fundamental Identities
- Six trig functions: sin, cos, tan, csc, sec, cot
- Reciprocal, quotient, Pythagorean (3), and cofunction identities
- ASTC rule for signs by quadrant

<!-- tags: id:E-TRIG-02, course:precalc, area:trig, type:expansion-review, code:B3, tier:1-essential, subtopic:trig-identities-proofs, yugioh:yes -->
### E-TRIG-02 · B3. Trigonometric Identities (Proving & Verifying)
- Sum/difference formulas for sin, cos, tan
- Double-angle formulas: sin(2x), cos(2x) (3 forms), tan(2x)
- Half-angle and power-reducing formulas; proof strategies

<!-- tags: id:E-TRIG-03, course:precalc, area:trig, type:expansion-review, code:B5, tier:1-essential, subtopic:inverse-trig -->
### E-TRIG-03 · B5. Inverse Trigonometric Functions
- arcsin: domain [-1,1], range [-pi/2, pi/2]
- arccos: domain [-1,1], range [0, pi]
- arctan: domain (-inf,inf), range (-pi/2, pi/2); composing trig/inverse trig

<!-- tags: id:E-TRIG-04, course:precalc, area:trig, type:expansion-review, code:B6, tier:1-essential, subtopic:trig-equations -->
### E-TRIG-04 · B6. Trigonometric Equations & Inequalities
- General solutions with +2pi*n for sin/cos, +pi*n for tan
- Multi-angle equations, quadratic-type trig equations
- Trig inequalities: solve equality, then sign chart/unit circle

### Tier 2 (Important)

<!-- tags: id:E-TRIG-05, course:precalc, area:trig, type:expansion-review, code:B1, tier:2-important, subtopic:angles-measure, yugioh:yes -->
### E-TRIG-05 · B1. Angles and Their Measure (Expanded)
- DMS system, DMS <-> decimal conversion
- Complementary, supplementary, coterminal angles
- Arc length: s = r*theta; sector area: A = (1/2)*r^2*theta
- Angular velocity omega = theta/t; linear velocity v = r*omega

<!-- tags: id:E-TRIG-06, course:precalc, area:trig, type:expansion-review, code:B4, tier:2-important, subtopic:trig-graphs -->
### E-TRIG-06 · B4. Graphs of Trigonometric Functions (Expanded)
- Graphs of all six trig functions with periods and asymptotes
- sin/cos: period 2pi; tan/cot: period pi; sec/csc: period 2pi
- Transformations: y = A*tan(B(x-C))+D, period = pi/|B|

<!-- tags: id:E-TRIG-07, course:precalc, area:trig, type:expansion-review, code:B7, tier:2-important, subtopic:law-of-sines -->
### E-TRIG-07 · B7. Law of Sines
- a/sin(A) = b/sin(B) = c/sin(C)
- Used for AAS, ASA, SSA cases
- Ambiguous case (SSA): 0, 1, or 2 triangles possible

<!-- tags: id:E-TRIG-08, course:precalc, area:trig, type:expansion-review, code:B8, tier:2-important, subtopic:law-of-cosines, yugioh:yes -->
### E-TRIG-08 · B8. Law of Cosines
- c^2 = a^2 + b^2 - 2ab*cos(C)
- Used for SAS and SSS cases; reduces to Pythagorean theorem at C = 90 deg
- Finding angles: cos(C) = (a^2 + b^2 - c^2)/(2ab)

### Tier 3 (Advanced)

<!-- tags: id:E-TRIG-09, course:precalc, area:trig, type:expansion-review, code:B9, tier:3-advanced, subtopic:polar-coordinates -->
### E-TRIG-09 · B9. Polar Coordinates
- Polar point (r, theta), conversion to/from Cartesian
- Polar graphs: circles, cardioids, rose curves, limacons, lemniscates

<!-- tags: id:E-TRIG-10, course:precalc, area:trig, type:expansion-review, code:B10, tier:3-advanced, subtopic:vectors -->
### E-TRIG-10 · B10. Vectors
- Vector v = <a, b>; magnitude, unit vector
- Dot product, perpendicularity, projection, work

<!-- tags: id:E-TRIG-11, course:precalc, area:trig, type:expansion-review, code:B11, tier:3-advanced, subtopic:parametric-equations, yugioh:yes -->
### E-TRIG-11 · B11. Parametric Equations
- x = f(t), y = g(t); eliminating parameter
- Common parametrizations: line, circle, ellipse

<!-- tags: id:E-TRIG-12, course:precalc, area:trig, type:expansion-review, code:B12, tier:3-advanced, subtopic:polar-complex -->
### E-TRIG-12 · B12. Polar Form of Complex Numbers
- z = r*cis(theta), De Moivre's Theorem, nth roots

<!-- tags: id:E-TRIG-13, course:precalc, area:trig, type:expansion-review, code:B13, tier:3-advanced, subtopic:harmonic-motion -->
### E-TRIG-13 · B13. Applications of Sinusoids / Harmonic Motion
- Model: S(t) = A*sin(omega*t - phi) + B
- Applications: Ferris wheels, springs, sound waves, daylight models

<!-- tags: id:E-TRIG-14, course:precalc, area:trig, type:expansion-review, code:B14, tier:3-advanced, subtopic:polar-conics-rotation -->
### E-TRIG-14 · B14. Conic Sections in Polar Form / Rotation of Axes
- Polar conics with eccentricity; rotation of axes to remove xy-term

---
---

# PART 3 — FLASHCARDS
# ====================

---

## 3A. Precalc Flashcards — Algebra

<!-- tags: id:FC-ALG-01, course:precalc, area:algebra, type:flashcard, subtopic:functions-notation -->
### FC-ALG-01 · Functions (4 cards)
- Q: What does f(a + h) mean?
  A: Replace every x in the function rule with (a + h). Example: if f(x) = x^2, then f(a + h) = (a + h)^2 = a^2 + 2ah + h^2.
- Q: What three things restrict the domain of a function?
  A: Division by zero (denominator != 0), even roots of negatives (radicand >= 0), logarithms of non-positives (argument > 0).
- Q: How do you evaluate the composition (f o g)(x)?
  A: (f o g)(x) = f(g(x)). Evaluate g(x) first, then plug into f. Domain: x in domain of g with g(x) in domain of f.
- Q: What is the difference between domain and range?
  A: Domain = all valid input values. Range = all possible outputs.

<!-- tags: id:FC-ALG-02, course:precalc, area:algebra, type:flashcard, subtopic:exponentials-logs -->
### FC-ALG-02 · Exponentials (4 cards)
- Q: State the core relationship between exponentials and logarithms.
  A: a^x = y <-> log_a(y) = x. They are inverse operations.
- Q: State all three logarithm properties (product, quotient, power).
  A: log(MN) = log(M) + log(N); log(M/N) = log(M) - log(N); log(M^k) = k * log(M).
- Q: What is the change of base formula?
  A: log_a(M) = ln(M) / ln(a).
- Q: State three key log/exp values you must memorize.
  A: ln(1) = 0, ln(e) = 1, e^(ln(x)) = x. Also log_a(1) = 0 and log_a(a) = 1.

<!-- tags: id:FC-ALG-03, course:precalc, area:algebra, type:flashcard, subtopic:polynomials -->
### FC-ALG-03 · Polynomials (3 cards)
- Q: How does the degree and leading coefficient determine end behavior?
  A: Even degree, positive lead -> both ends +inf. Even degree, negative lead -> both ends -inf. Odd degree, positive lead -> left -inf, right +inf. Odd degree, negative lead -> left +inf, right -inf.
- Q: How do you find the horizontal asymptote of a rational function P(x)/Q(x)?
  A: Compare degrees: deg(P) < deg(Q) -> y = 0; deg(P) = deg(Q) -> ratio of leading coefficients; deg(P) > deg(Q) -> no horizontal asymptote.
- Q: How do you find vertical asymptotes of a rational function?
  A: Set denominator = 0. x = a is a vertical asymptote only if the numerator is not also 0 at x = a.

<!-- tags: id:FC-ALG-04, course:precalc, area:algebra, type:flashcard, subtopic:algebra-manipulation -->
### FC-ALG-04 · Algebra Skills (4 cards)
- Q: State the difference of squares and sum/difference of cubes patterns.
  A: a^2 - b^2 = (a + b)(a - b); a^3 + b^3 = (a + b)(a^2 - ab + b^2); a^3 - b^3 = (a - b)(a^2 + ab + b^2).
- Q: State the quadratic formula and explain the discriminant.
  A: x = (-b +/- sqrt(b^2 - 4ac)) / (2a). Delta > 0 two distinct real roots; Delta = 0 one repeated real root; Delta < 0 no real roots.
- Q: What are the steps to complete the square for x^2 + bx?
  A: Take half of b, square it, add and subtract: x^2 + bx = (x + b/2)^2 - (b/2)^2. Example: x^2 + 6x = (x + 3)^2 - 9.
- Q: How do you rationalize a denominator with a binomial radical like 1/(sqrt(a) + b)?
  A: Multiply numerator and denominator by the conjugate (sqrt(a) - b).

<!-- tags: id:FC-ALG-05, course:precalc, area:algebra, type:flashcard, subtopic:linear-functions -->
### FC-ALG-05 · Lines (3 cards)
- Q: State the slope formula and the three main forms of a line.
  A: m = (y2 - y1)/(x2 - x1). Forms: y = mx + b, y - y1 = m(x - x1), Ax + By = C.
- Q: What is the relationship between slopes of parallel and perpendicular lines?
  A: Parallel: same slope. Perpendicular: negative reciprocal slopes (m1 * m2 = -1).
- Q: What does a slope of zero vs. an undefined slope look like?
  A: Slope 0 -> horizontal line. Undefined slope -> vertical line (not a function).

<!-- tags: id:FC-ALG-06, course:precalc, area:algebra, type:flashcard, subtopic:absolute-value-piecewise -->
### FC-ALG-06 · Absolute Value and Piecewise (3 cards)
- Q: State the formal definition of |x|.
  A: |x| = x if x >= 0, and -x if x < 0.
- Q: How do you solve |expression| = k?
  A: If k > 0: expression = k or expression = -k. If k = 0: expression = 0. If k < 0: no solution.
- Q: How do you solve |expression| < k (k > 0)?
  A: -k < expression < k. For |expression| > k: expression < -k or expression > k.

<!-- tags: id:FC-ALG-07, course:precalc, area:algebra, type:flashcard, subtopic:inverse-functions -->
### FC-ALG-07 · Inverses (3 cards)
- Q: What is the definition of an inverse function?
  A: f and g are inverses if f(g(x)) = x and g(f(x)) = x. Domain and range swap.
- Q: What are the steps to find an inverse function algebraically?
  A: 1) y = f(x). 2) Swap x and y. 3) Solve for y. 4) Write f^-1(x). 5) Verify f(f^-1(x)) = x.
- Q: How are the graphs of f and f^-1 related?
  A: f^-1 is the reflection of f across y = x.

<!-- tags: id:FC-ALG-08, course:precalc, area:algebra, type:flashcard, subtopic:transformations -->
### FC-ALG-08 · Transformations (4 cards)
- Q: What does y = f(x) + k do to the graph? What about y = f(x + h)?
  A: y = f(x) + k shifts up by k (down if k < 0). y = f(x + h) shifts left by h (right if h < 0).
- Q: How do vertical and horizontal stretches/compressions work?
  A: y = a f(x) stretches vertically by |a| if |a| > 1 (compress if 0 < |a| < 1). y = f(bx) compresses horizontally by 1/|b| if |b| > 1 (stretch if 0 < |b| < 1).
- Q: What do y = -f(x) and y = f(-x) do?
  A: -f(x) reflects across the x-axis. f(-x) reflects across the y-axis.
- Q: In what order should you apply multiple transformations?
  A: 1) Horizontal stretch/compress and reflection (inside). 2) Horizontal shift. 3) Vertical stretch/compress and reflection. 4) Vertical shift (outside).

<!-- tags: id:FC-ALG-09, course:precalc, area:algebra, type:flashcard, subtopic:inequalities -->
### FC-ALG-09 · Inequalities (3 cards)
- Q: What critical rule must you remember when solving inequalities?
  A: Multiply/divide by a negative -> flip the inequality sign.
- Q: How does the sign chart method work for polynomial/rational inequalities?
  A: Move to one side, factor, find zeros/undefined points, test signs in intervals, choose intervals that satisfy the inequality.
- Q: How do you write solutions in interval notation?
  A: Use ( ) for strict and [ ] for inclusive. Use parentheses with inf. Example: -3 <= x < 5 is [-3, 5). Use union for disjoint intervals.

<!-- tags: id:FC-ALG-10, course:precalc, area:algebra, type:flashcard, subtopic:sequences-series -->
### FC-ALG-10 · Sequences (4 cards)
- Q: State the formulas for the nth term and sum of an arithmetic sequence.
  A: an = a1 + (n - 1)d; Sn = n(a1 + an)/2.
- Q: State the formulas for the nth term and sum of a geometric sequence.
  A: an = a1 * r^(n-1); Sn = a1(1 - r^n)/(1 - r).
- Q: What is the formula for an infinite geometric series, and when does it converge?
  A: S = a1/(1 - r), valid only when |r| < 1.
- Q: How do you determine if a sequence is arithmetic vs. geometric?
  A: Arithmetic has constant difference; geometric has constant ratio.

---

## 3B. Precalc Flashcards — Trigonometry

<!-- tags: id:FC-TRIG-01, course:precalc, area:trig, type:flashcard, subtopic:trig-identities -->
### FC-TRIG-01 · Trigonometry (4 cards)
- Q: State the Pythagorean identity.
  A: sin^2(x) + cos^2(x) = 1.
- Q: State both double-angle formulas for sin(2x) and cos(2x).
  A: sin(2x) = 2 sin(x) cos(x). cos(2x) = cos^2(x) - sin^2(x) = 2 cos^2(x) - 1 = 1 - 2 sin^2(x).
- Q: Which trig functions are even and which are odd?
  A: Even: cos(-x) = cos(x), sec(-x) = sec(x). Odd: sin(-x) = -sin(x), tan(-x) = -tan(x), csc(-x) = -csc(x), cot(-x) = -cot(x).
- Q: Express tan(x) and the two other Pythagorean identities.
  A: tan(x) = sin(x)/cos(x); 1 + tan^2(x) = sec^2(x); 1 + cot^2(x) = csc^2(x).

<!-- tags: id:FC-TRIG-02, course:precalc, area:trig, type:flashcard, subtopic:unit-circle -->
### FC-TRIG-02 · Unit Circle (4 cards)
- Q: What are cos(pi/6) and sin(pi/6)?
  A: cos(pi/6) = sqrt(3)/2 and sin(pi/6) = 1/2.
- Q: What are cos(pi/4) and sin(pi/4)?
  A: cos(pi/4) = sqrt(2)/2 and sin(pi/4) = sqrt(2)/2.
- Q: Which trig functions are positive in each quadrant?
  A: QI: all positive. QII: sin, csc. QIII: tan, cot. QIV: cos, sec. Mnemonic: All Students Take Calculus.
- Q: How do you convert between degrees and radians?
  A: Degrees -> radians: multiply by pi/180. Radians -> degrees: multiply by 180/pi. Example: 60 deg * (pi/180) = pi/3.

<!-- tags: id:FC-TRIG-03, course:precalc, area:trig, type:flashcard, subtopic:sinusoidal-models -->
### FC-TRIG-03 · Sinusoidal (3 cards)
- Q: In y = A sin(bx + c) + D, what does each parameter control?
  A: A = amplitude, b = frequency with period 2pi/b, c = phase constant with phase shift -c/b, D = vertical shift (midline y = D).
- Q: How do you find the period of y = 3 sin(2x) - 5?
  A: Period = 2pi/b = 2pi/2 = pi.
- Q: How do you find amplitude from a graph showing max and min values?
  A: Amplitude = (max - min)/2. Midline D = (max + min)/2.

---

## 3C. Precalc Flashcards — Calculus Preview

<!-- tags: id:FC-CALC-P01, course:precalc, area:calculus, type:flashcard, subtopic:limits -->
### FC-CALC-P01 · Limits (3 cards)
- Q: What does lim(x->a) f(x) = L mean intuitively?
  A: As x approaches a, f(x) approaches L. f(a) does not need to exist.
- Q: What are the common indeterminate forms, and what do you do about 0/0?
  A: Common: 0/0 and inf/inf. For 0/0: factor, rationalize, or simplify to cancel, then substitute.
- Q: How do you find the limit of a polynomial as x -> c?
  A: Substitute x = c (polynomials are continuous).

---

## 3D. Precalc Flashcards — General

<!-- tags: id:FC-GEN-01, course:precalc, area:precalc-general, type:flashcard, subtopic:common-mistakes -->
### FC-GEN-01 · Common Mistakes (3 cards)
- Q: Why is ln(a + b) != ln(a) + ln(b)?
  A: Log product rule requires multiplication inside, not addition.
- Q: What is the correct expansion of (a + b)^2?
  A: a^2 + 2ab + b^2.
- Q: Is sqrt(a^2 + b^2) equal to a + b?
  A: No. sqrt does not distribute over addition.

<!-- tags: id:FC-GEN-02, course:precalc, area:precalc-general, type:flashcard, subtopic:calculator-skills -->
### FC-GEN-02 · Calculator (3 cards)
- Q: When should your calculator be in radian mode vs degree mode?
  A: Use radian mode for calculus and most precalc problems (especially with pi). Use degree mode only when angles are given in degrees.
- Q: How do you compute log base 5 of 20 on a calculator that only has ln?
  A: log_5(20) = ln(20) / ln(5) approx 1.861.
- Q: What is a common calculator pitfall with negative numbers and exponents?
  A: -3^2 = -9 (exponent first). Use parentheses: (-3)^2 = 9.

---

## 3E. Calculus Flashcards

<!-- tags: id:FC-CALC-01, course:calculus, area:calculus, type:flashcard, subtopic:limits -->
### FC-CALC-01 · Calc Limits (7 cards)
- Q: What is the limit of f(x) = 3x^2 - 2x + 1 as x approaches 2?  A: 9.
- Q: What is the value of lim(x->0) sin(x)/x?  A: 1.
- Q: What is the limit of (x^2 - 4)/(x - 2) as x approaches 2?  A: 4.
- Q: What is the value of lim(x->inf) (2x^2 + 3x)/(x^2 + 1)?  A: 2.
- Q: What is the limit of 1/x as x approaches infinity?  A: 0.
- Q: What is the value of lim(x->3) (x^2 - 9)/(x - 3)?  A: 6.
- Q: What is the limit of e^x as x approaches negative infinity?  A: 0.

<!-- tags: id:FC-CALC-02, course:calculus, area:calculus, type:flashcard, subtopic:derivatives -->
### FC-CALC-02 · Calc Derivatives (10 cards)
- Q: What is the derivative of f(x) = x^3?  A: 3x^2.
- Q: What is the derivative of f(x) = sin(x)?  A: cos(x).
- Q: What is the derivative of f(x) = e^x?  A: e^x.
- Q: What is the derivative of f(x) = ln(x)?  A: 1/x.
- Q: What is the derivative of f(x) = x^2 + 3x - 4?  A: 2x + 3.
- Q: What is the derivative of f(x) = cos(x)?  A: -sin(x).
- Q: What is the derivative of f(x) = tan(x)?  A: sec^2(x).
- Q: What is the derivative of f(x) = x sin(x)?  A: sin(x) + x cos(x).
- Q: What is the derivative of f(x) = 1/x?  A: -1/x^2.
- Q: What is the derivative of f(x) = x^4 - 2x^3 + 5x^2 - 3x + 1?  A: 4x^3 - 6x^2 + 10x - 3.

<!-- tags: id:FC-CALC-03, course:calculus, area:calculus, type:flashcard, subtopic:integrals -->
### FC-CALC-03 · Calc Integrals (10 cards)
- Q: What is the integral of f(x) = x^2?  A: x^3/3 + C.
- Q: What is the value of int e^x dx?  A: e^x + C.
- Q: What is the integral of f(x) = sin(x)?  A: -cos(x) + C.
- Q: What is the value of int (1/x) dx?  A: ln|x| + C.
- Q: What is the integral of f(x) = cos(x)?  A: sin(x) + C.
- Q: What is the value of int x^3 dx?  A: x^4/4 + C.
- Q: What is the integral of f(x) = 1/x^2?  A: -1/x + C.
- Q: What is the value of int (2x + 3) dx?  A: x^2 + 3x + C.
- Q: What is the integral of f(x) = tan(x)?  A: -ln|cos(x)| + C (equivalently ln|sec(x)| + C).
- Q: What is the value of int sqrt(x) dx?  A: (2/3)x^(3/2) + C.

<!-- tags: id:FC-CALC-04, course:calculus, area:calculus, type:flashcard, subtopic:applications -->
### FC-CALC-04 · Calc Applications (8 cards)
- Q: What is the slope of the tangent line to y = x^2 at x = 2?  A: 4.
- Q: What are the critical points of f(x) = x^3 - 3x^2?  A: x = 0 and x = 2.
- Q: What is the maximum value of f(x) = x^4 - 4x^3 + 4 on [0, 4]?  A: 4 (at x = 0 and x = 4).
- Q: What is the minimum value of f(x) = x^2 - 4x + 4?  A: 0 (at x = 2).
- Q: What is the rate of change of f(x) = x^2 at x = 3?  A: 6.
- Q: What is the derivative of f(x) = x^2 sin(x)?  A: 2x sin(x) + x^2 cos(x).
- Q: What is the slope of the tangent line to y = ln(x) at x = 1?  A: 1.
- Q: What are the critical points of f(x) = x^3 - 6x^2 + 11x - 6?  A: x = (6 +/- sqrt(3)) / 3.

---

## 3F. Expansion Flashcards — Precalculus (A-coded, 35 cards)

<!-- tags: id:FC-EA-01, course:precalc, area:algebra, type:flashcard, code:A1, subtopic:domain-range -->
### FC-EA-01 · A1. Domain & Range (3 cards)
- Q: What three things restrict a function's domain?
  A: 1) Denominator = 0, 2) Even root of a negative, 3) Log of zero or negative.
- Q: Write the domain of f(x) = sqrt(4 - x) in interval notation.
  A: (-inf, 4].
- Q: What is the domain of f(x) = 1/(x - 3)?
  A: (-inf, 3) union (3, inf).

<!-- tags: id:FC-EA-02, course:precalc, area:precalc-general, type:flashcard, code:A2, subtopic:rates-of-change -->
### FC-EA-02 · A2. Rates of Change (3 cards)
- Q: What is the average rate of change of f(x) = x^2 on [1, 5]?
  A: (25 - 1)/(5 - 1) = 6.
- Q: What is an inflection point?
  A: A point where the function changes from concave up to concave down, or vice versa.
- Q: How do you tell if a function is concave up from a table?
  A: The rate of change between consecutive points is increasing.

<!-- tags: id:FC-EA-03, course:precalc, area:algebra, type:flashcard, code:A3, subtopic:function-composition -->
### FC-EA-03 · A3. Function Composition (3 cards)
- Q: If f(x) = x^2 and g(x) = x + 3, what is f(g(2))?
  A: g(2) = 5, then f(5) = 25.
- Q: What is the domain of f(g(x)) if f(x) = sqrt(x) and g(x) = x - 4?
  A: Need g(x) >= 0, so x >= 4. Domain: [4, inf).
- Q: What does "decomposition" of a function mean?
  A: Writing a function as a composition of two simpler functions.

<!-- tags: id:FC-EA-04, course:precalc, area:algebra, type:flashcard, code:A4, subtopic:linear-functions -->
### FC-EA-04 · A4. Linear Functions (2 cards)
- Q: A town had population 45,000 in 2003 and grows by 1,700/year. Write the equation.
  A: P(t) = 1700t + 45000, where t = years after 2003.
- Q: Find the equation of the line through (2, 4) and (4, 10).
  A: m = 3. y = 3x - 2.

<!-- tags: id:FC-EA-05, course:precalc, area:algebra, type:flashcard, code:A5, subtopic:polynomials-deep -->
### FC-EA-05 · A5. Polynomials Deep (3 cards)
- Q: What determines the end behavior of a polynomial?
  A: The degree (even/odd) and the sign of the leading coefficient.
- Q: What happens at a zero with multiplicity 2?
  A: The graph touches (bounces off) the x-axis but doesn't cross it.
- Q: A degree-5 polynomial has at most how many turning points?
  A: 4.

<!-- tags: id:FC-EA-06, course:precalc, area:algebra, type:flashcard, code:A6, subtopic:quadratics-expanded -->
### FC-EA-06 · A6. Quadratics Expanded (2 cards)
- Q: Find the vertex of f(x) = 2x^2 - 12x + 7.
  A: h = 3, k = f(3) = -11. Vertex: (3, -11).
- Q: When does a quadratic have a maximum vs. minimum?
  A: Maximum when a < 0 (opens down); minimum when a > 0 (opens up).

<!-- tags: id:FC-EA-07, course:precalc, area:algebra, type:flashcard, code:A7, subtopic:factor-remainder -->
### FC-EA-07 · A7. Factor & Remainder (3 cards)
- Q: What does the Remainder Theorem state?
  A: When polynomial p(x) is divided by (x - c), the remainder equals p(c).
- Q: What does the Factor Theorem tell us?
  A: (x - c) is a factor of p(x) iff p(c) = 0.
- Q: Describe synthetic division in 3 steps.
  A: 1) Write c and the coefficients. 2) Bring down first coeff. 3) Multiply by c, add to next coeff, repeat.

<!-- tags: id:FC-EA-08, course:precalc, area:algebra, type:flashcard, code:A8, subtopic:real-zeros -->
### FC-EA-08 · A8. Real Zeros (2 cards)
- Q: State the Rational Roots Theorem.
  A: Any rational zero p/q has p | a_0 and q | a_n.
- Q: What are the possible rational zeros of 2x^3 + 3x^2 - 1?
  A: +/-{1, 1/2}.

<!-- tags: id:FC-EA-09, course:precalc, area:algebra, type:flashcard, code:A9, subtopic:complex-zeros -->
### FC-EA-09 · A9. Complex Zeros (3 cards)
- Q: What is the conjugate of 3 - 2i?  A: 3 + 2i.
- Q: Simplify (2 + i)(3 - 4i).  A: 10 - 5i.
- Q: Why do complex zeros come in conjugate pairs for real-coefficient polynomials?
  A: Because the complex conjugate of each step in evaluation also equals zero.

<!-- tags: id:FC-EA-10, course:precalc, area:algebra, type:flashcard, code:A10, subtopic:rational-functions-deep -->
### FC-EA-10 · A10. Rational Functions Deep (3 cards)
- Q: When does a rational function have a hole instead of a vertical asymptote?
  A: When a factor cancels from both numerator and denominator.
- Q: What is an oblique asymptote?
  A: A slant line the function approaches as x -> +/-inf. Occurs when deg(num) = deg(denom) + 1.
- Q: Find the oblique asymptote of f(x) = (x^2 + 2x + 1)/(x - 1).
  A: y = x + 3.

<!-- tags: id:FC-EA-11, course:precalc, area:algebra, type:flashcard, code:A11, subtopic:inverses-radicals -->
### FC-EA-11 · A11. Inverses & Radicals (2 cards)
- Q: Why must we check for extraneous solutions when solving radical equations?
  A: Squaring both sides can introduce solutions that don't satisfy the original equation.
- Q: What is the inverse of f(x) = x^2 for x >= 0?
  A: f^-1(x) = sqrt(x).

<!-- tags: id:FC-EA-12, course:precalc, area:algebra, type:flashcard, code:A12, subtopic:exponential-models -->
### FC-EA-12 · A12. Exponential Models (3 cards)
- Q: What is the formula for continuous compound interest?  A: A = Pe^(rt).
- Q: If a population doubles every 5 years with continuous growth, what is r?
  A: r = ln(2)/5 approx 0.1386.
- Q: Solve 3^x = 81.  A: x = 4.

<!-- tags: id:FC-EA-13, course:precalc, area:algebra, type:flashcard, code:A13, subtopic:logarithmic-models -->
### FC-EA-13 · A13. Logarithmic Models (3 cards)
- Q: Solve log_2(x) = 5.  A: x = 32.
- Q: Solve ln(x) + ln(x - 2) = ln(3).  A: x = 3 (reject x = -1).
- Q: What is the domain of f(x) = log(x - 5)?  A: (5, inf).

---

## 3G. Expansion Flashcards — Trigonometry (B-coded, 41 cards)

<!-- tags: id:FC-EB-01, course:precalc, area:trig, type:flashcard, code:B1, subtopic:angles-measure -->
### FC-EB-01 · B1. Angles & Measure (3 cards)
- Q: Convert 42 deg 7' 30" to decimal degrees.  A: 42.125 deg.
- Q: Find the arc length of a sector with radius 5 and central angle pi/3.  A: 5pi/3 approx 5.24.
- Q: What are coterminal angles?  A: Angles that share the same terminal side; they differ by multiples of 360 deg (or 2pi).

<!-- tags: id:FC-EB-02, course:precalc, area:trig, type:flashcard, code:B2, subtopic:six-functions-identities -->
### FC-EB-02 · B2. Six Trig Functions (3 cards)
- Q: State the three Pythagorean identities.
  A: sin^2(x) + cos^2(x) = 1; 1 + tan^2(x) = sec^2(x); 1 + cot^2(x) = csc^2(x).
- Q: If sin(theta) = 3/5 and theta is in QI, find all six trig values.
  A: cos = 4/5, tan = 3/4, csc = 5/3, sec = 5/4, cot = 4/3.
- Q: State the cofunction identity for sin.  A: sin(pi/2 - theta) = cos(theta).

<!-- tags: id:FC-EB-03, course:precalc, area:trig, type:flashcard, code:B3, subtopic:trig-identities-proofs -->
### FC-EB-03 · B3. Trig Identities Proofs (3 cards)
- Q: State the sum formula for sin(A + B).  A: sinA*cosB + cosA*sinB.
- Q: Find the exact value of cos(75 deg) using sum formulas.  A: (sqrt(6) - sqrt(2))/4.
- Q: State the half-angle formula for sin(theta/2).
  A: sin(theta/2) = +/-sqrt[(1 - cos(theta))/2], sign depends on quadrant.

<!-- tags: id:FC-EB-04, course:precalc, area:trig, type:flashcard, code:B4, subtopic:trig-graphs -->
### FC-EB-04 · B4. Trig Graphs (3 cards)
- Q: What is the period of y = tan(x)?  A: pi.
- Q: Where are the vertical asymptotes of y = csc(x)?  A: At x = n*pi for integer n (wherever sin(x) = 0).
- Q: What is the period of y = 3tan(2x)?  A: pi/2.

<!-- tags: id:FC-EB-05, course:precalc, area:trig, type:flashcard, code:B5, subtopic:inverse-trig -->
### FC-EB-05 · B5. Inverse Trig Functions (3 cards)
- Q: What is arcsin(1/2)?  A: pi/6 (30 deg).
- Q: What is the range of arccos(x)?  A: [0, pi].
- Q: Evaluate cos(arctan(3/4)).  A: 4/5 (draw right triangle: opp 3, adj 4, hyp 5).

<!-- tags: id:FC-EB-06, course:precalc, area:trig, type:flashcard, code:B6, subtopic:trig-equations -->
### FC-EB-06 · B6. Trig Equations (3 cards)
- Q: Find all solutions to sin(x) = sqrt(3)/2 in [0, 2pi).  A: x = pi/3 and x = 2pi/3.
- Q: Find the general solution to cos(x) = -1/2.  A: x = 2pi/3 + 2pi*k or x = 4pi/3 + 2pi*k.
- Q: Solve 2sin^2(x) - sin(x) - 1 = 0.
  A: (2sinx + 1)(sinx - 1) = 0 -> sinx = -1/2 or sinx = 1.

<!-- tags: id:FC-EB-07, course:precalc, area:trig, type:flashcard, code:B7, subtopic:law-of-sines -->
### FC-EB-07 · B7. Law of Sines (3 cards)
- Q: State the Law of Sines.  A: a/sinA = b/sinB = c/sinC.
- Q: When is the Law of Sines ambiguous?  A: In the SSA case — you might get 0, 1, or 2 valid triangles.
- Q: Find side b if A = 30 deg, B = 45 deg, a = 10.
  A: b = 10*sin(45 deg)/sin(30 deg) = 10*sqrt(2) approx 14.14.

<!-- tags: id:FC-EB-08, course:precalc, area:trig, type:flashcard, code:B8, subtopic:law-of-cosines -->
### FC-EB-08 · B8. Law of Cosines (3 cards)
- Q: State the Law of Cosines.  A: c^2 = a^2 + b^2 - 2ab*cos(C).
- Q: If a = 5, b = 7, C = 60 deg, find c.  A: c = sqrt(39) approx 6.24.
- Q: When does the Law of Cosines reduce to the Pythagorean theorem?  A: When C = 90 deg (cos 90 deg = 0).

<!-- tags: id:FC-EB-09, course:precalc, area:trig, type:flashcard, code:B9, subtopic:polar-coordinates -->
### FC-EB-09 · B9. Polar Coordinates (3 cards)
- Q: Convert (3, pi/4) from polar to Cartesian.  A: x = 3*sqrt(2)/2, y = 3*sqrt(2)/2.
- Q: Convert (1, 1) from Cartesian to polar.  A: (sqrt(2), pi/4).
- Q: How many petals does r = 3cos(4*theta) have?  A: 8 (2n = 2*4, since n is even).

<!-- tags: id:FC-EB-10, course:precalc, area:trig, type:flashcard, code:B10, subtopic:vectors -->
### FC-EB-10 · B10. Vectors (3 cards)
- Q: Find the magnitude of v = <3, 4>.  A: 5.
- Q: Find the dot product of <2, -1> and <3, 4>.  A: 2.
- Q: When are two vectors perpendicular?  A: When their dot product equals zero.

<!-- tags: id:FC-EB-11, course:precalc, area:trig, type:flashcard, code:B11, subtopic:parametric-equations -->
### FC-EB-11 · B11. Parametric Equations (3 cards)
- Q: Eliminate the parameter from x = t^2, y = 2t + 1.  A: 4x = (y - 1)^2.
- Q: Parametrize the line segment from (1, 3) to (4, 7).  A: x = 1 + 3t, y = 3 + 4t, for 0 <= t <= 1.
- Q: What do parametric equations add that y = f(x) doesn't?
  A: Direction/orientation and the ability to represent curves that aren't functions.

<!-- tags: id:FC-EB-12, course:precalc, area:trig, type:flashcard, code:B12, subtopic:polar-complex -->
### FC-EB-12 · B12. Polar Complex Numbers (3 cards)
- Q: Write z = 1 + i in polar form.  A: z = sqrt(2) * cis(pi/4).
- Q: State De Moivre's Theorem.  A: [r*cis(theta)]^n = r^n * cis(n*theta).
- Q: Multiply 2*cis(pi/3) and 3*cis(pi/6).  A: 6*cis(pi/2) = 6i.

<!-- tags: id:FC-EB-13, course:precalc, area:trig, type:flashcard, code:B13, subtopic:harmonic-motion -->
### FC-EB-13 · B13. Harmonic Motion (3 cards)
- Q: A Ferris wheel has diameter 128 ft and completes 2 revolutions in 127 seconds. What is the angular frequency?
  A: omega = 4pi/127 rad/s.
- Q: How do you find amplitude from a graph?  A: Amplitude = (max - min)/2.
- Q: What is the midline of a sinusoid with max 80 and min 20?  A: 50.

<!-- tags: id:FC-EB-14, course:precalc, area:trig, type:flashcard, code:B14, subtopic:polar-conics-rotation -->
### FC-EB-14 · B14. Polar Conics (2 cards)
- Q: What determines if a polar conic is an ellipse, parabola, or hyperbola?
  A: Eccentricity e: e < 1 -> ellipse, e = 1 -> parabola, e > 1 -> hyperbola.
- Q: What is the rotation angle formula for eliminating an xy-term?
  A: cot(2*alpha) = (A - C)/B.

---
---

# PART 4 — QUIZ QUESTIONS
# ========================

---

## 4A. Precalc Quiz — Algebra

<!-- tags: id:QZ-ALG-01, course:precalc, area:algebra, type:quiz, subtopic:functions-notation -->
### QZ-ALG-01 · Functions and Algebra
- Q: If f(x) = x^2 - 3x + 2, what is f(2)?
  Options: A) 0  B) 2  C) 4  D) 6
  Answer: A) 0
- Q: Factor: x^2 - 9
  Options: A) (x - 3)^2  B) (x + 3)^2  C) (x - 3)(x + 3)  D) (x - 3)(x - 3)
  Answer: C) (x - 3)(x + 3)
- Q: Solve: x^2 - 5x + 6 = 0
  Options: A) 1, 6  B) 2, 3  C) -2, -3  D) 2, -3
  Answer: B) 2, 3

<!-- tags: id:QZ-ALG-02, course:precalc, area:algebra, type:quiz, subtopic:exponentials-logs -->
### QZ-ALG-02 · Exponentials and Logs
- Q: Solve: 2^x = 16
  Options: A) 2  B) 3  C) 4  D) 8
  Answer: C) 4
- Q: Which is equivalent to ln(e^5)?
  Options: A) 1  B) e  C) 5  D) e^5
  Answer: C) 5
- Q: Expand: log(x^2 y / z)
  Options: A) 2log(x) + log(y) - log(z)  B) log(x) + log(y) - log(z)  C) 2log(x) - log(y) - log(z)  D) log(2x) + log(y) - log(z)
  Answer: A) 2log(x) + log(y) - log(z)
- Q: What is ln(1)?
  Options: A) 0  B) 1  C) undefined  D) e
  Answer: A) 0

<!-- tags: id:QZ-ALG-03, course:precalc, area:algebra, type:quiz, subtopic:absolute-value-piecewise -->
### QZ-ALG-03 · Absolute Value
- Q: Solve: |x - 3| = 5
  Options: A) 3  B) 8, -2  C) 5, -5  D) -2, 8
  Answer: D) -2, 8

<!-- tags: id:QZ-ALG-04, course:precalc, area:algebra, type:quiz, subtopic:linear-functions -->
### QZ-ALG-04 · Lines
- Q: Which are perpendicular lines?
  Options: A) m=2, m=2  B) m=2, m=-1/2  C) m=2, m=1/2  D) m=2, m=1
  Answer: B) m=2, m=-1/2

<!-- tags: id:QZ-ALG-05, course:precalc, area:algebra, type:quiz, subtopic:rational-functions -->
### QZ-ALG-05 · Rational Functions
- Q: For f(x) = 1/(x - 2), what is the vertical asymptote?
  Options: A) x=0  B) x=1  C) x=2  D) x=-2
  Answer: C) x=2

---

## 4B. Precalc Quiz — Trigonometry

<!-- tags: id:QZ-TRIG-01, course:precalc, area:trig, type:quiz, subtopic:trig-core -->
### QZ-TRIG-01 · Trigonometry and Unit Circle
- Q: What is cos(pi/3)?
  Options: A) 0  B) 1/2  C) sqrt(3)/2  D) 1
  Answer: B) 1/2
- Q: Solve: sin(x) = 1/2 for x in [0, 2pi)
  Options: A) pi/6, 5pi/6  B) pi/3, 2pi/3  C) pi/4, 3pi/4  D) pi/6, pi/3
  Answer: A) pi/6, 5pi/6
- Q: Simplify: sin^2(x) + cos^2(x)
  Options: A) 0  B) 1  C) sin(2x)  D) tan(x)
  Answer: B) 1
- Q: Find the period of y = cos(pi x)
  Options: A) pi  B) 2pi  C) 2  D) 1/2
  Answer: C) 2

<!-- tags: id:QZ-TRIG-02, course:precalc, area:trig, type:quiz, subtopic:sinusoidal-models -->
### QZ-TRIG-02 · Sinusoidal Models
- Q: Find the amplitude of y = 3sin(2x) - 5
  Options: A) 2  B) 3  C) 5  D) -5
  Answer: B) 3

---

## 4C. Calculus Quiz Pool (35 questions)

<!-- tags: id:QZ-CALC-01, course:calculus, area:calculus, type:quiz, subtopic:limits -->
### QZ-CALC-01 · Limits (7 Qs)
- Q: What is the limit of f(x) = 3x^2 - 2x + 1 as x approaches 2?
  Options: A) 9  B) 5  C) 11  D) 7   Answer: A) 9
- Q: Evaluate: lim(x->0) sin(x)/x
  Options: A) 0  B) 1  C) inf  D) undefined   Answer: B) 1
- Q: What is the limit of (x^2 - 4)/(x - 2) as x approaches 2?
  Options: A) 0  B) 2  C) 4  D) undefined   Answer: C) 4
- Q: Evaluate: lim(x->inf) (2x^2 + 3x)/(x^2 + 1)
  Options: A) 0  B) 1  C) 2  D) 3   Answer: C) 2
- Q: What is the limit of 1/x as x approaches infinity?
  Options: A) 0  B) 1  C) inf  D) undefined   Answer: A) 0
- Q: Evaluate: lim(x->3) (x^2 - 9)/(x - 3)
  Options: A) 0  B) 3  C) 6  D) 9   Answer: C) 6
- Q: What is the limit of e^x as x approaches negative infinity?
  Options: A) 0  B) 1  C) -inf  D) inf   Answer: A) 0

<!-- tags: id:QZ-CALC-02, course:calculus, area:calculus, type:quiz, subtopic:derivatives -->
### QZ-CALC-02 · Derivatives (10 Qs)
- Q: What is the derivative of f(x) = x^3?
  Options: A) x^2  B) 3x  C) 3x^2  D) x^3   Answer: C) 3x^2
- Q: Find the derivative of f(x) = sin(x).
  Options: A) cos(x)  B) -cos(x)  C) -sin(x)  D) tan(x)   Answer: A) cos(x)
- Q: What is the derivative of f(x) = e^x?
  Options: A) x e^(x-1)  B) e^x  C) e^(x-1)  D) ln(x)   Answer: B) e^x
- Q: Find the derivative of f(x) = ln(x).
  Options: A) x  B) 1/x  C) ln(x)/x  D) e^x   Answer: B) 1/x
- Q: What is the derivative of f(x) = x^2 + 3x - 4?
  Options: A) 2x + 3  B) x^2 + 3  C) 2x - 4  D) 2x + 3x   Answer: A) 2x + 3
- Q: Find the derivative of f(x) = cos(x).
  Options: A) sin(x)  B) -sin(x)  C) -cos(x)  D) tan(x)   Answer: B) -sin(x)
- Q: What is the derivative of f(x) = tan(x)?
  Options: A) sec(x)  B) cot(x)  C) sec^2(x)  D) -csc^2(x)   Answer: C) sec^2(x)
- Q: Find the derivative of f(x) = x sin(x).
  Options: A) cos(x)  B) x cos(x)  C) sin(x) + cos(x)  D) sin(x) + x cos(x)   Answer: D) sin(x) + x cos(x)
- Q: What is the derivative of f(x) = 1/x?
  Options: A) 1/x^2  B) -1/x^2  C) ln(x)  D) -ln(x)   Answer: B) -1/x^2
- Q: Find the derivative of f(x) = x^4 - 2x^3 + 5x^2 - 3x + 1.
  Options: A) 4x^3 - 6x^2 + 10x - 3  B) 4x^3 - 2x^2 + 5x - 3  C) x^3 - 6x^2 + 10x - 3  D) 4x^4 - 6x^3 + 10x^2 - 3x   Answer: A) 4x^3 - 6x^2 + 10x - 3

<!-- tags: id:QZ-CALC-03, course:calculus, area:calculus, type:quiz, subtopic:integrals -->
### QZ-CALC-03 · Integrals (10 Qs)
- Q: What is the integral of f(x) = x^2?
  Options: A) x^3/3 + C  B) 2x + C  C) x^3 + C  D) x^2/2 + C   Answer: A) x^3/3 + C
- Q: Evaluate: int e^x dx
  Options: A) e^x + C  B) x e^x + C  C) e^(x+1)/(x+1) + C  D) ln(x) + C   Answer: A) e^x + C
- Q: What is the integral of f(x) = sin(x)?
  Options: A) cos(x) + C  B) -cos(x) + C  C) -sin(x) + C  D) sin^2(x)/2 + C   Answer: B) -cos(x) + C
- Q: Evaluate: int (1/x) dx
  Options: A) x + C  B) ln(x) + C  C) ln|x| + C  D) -1/x^2 + C   Answer: C) ln|x| + C
- Q: What is the integral of f(x) = cos(x)?
  Options: A) sin(x) + C  B) -sin(x) + C  C) cos^2(x) + C  D) tan(x) + C   Answer: A) sin(x) + C
- Q: Evaluate: int x^3 dx
  Options: A) 3x^2 + C  B) x^4 + C  C) x^4/4 + C  D) x^3/3 + C   Answer: C) x^4/4 + C
- Q: What is the integral of f(x) = 1/x^2?
  Options: A) -1/x + C  B) 1/x + C  C) ln(x^2) + C  D) -2/x^3 + C   Answer: A) -1/x + C
- Q: Evaluate: int (2x + 3) dx
  Options: A) x^2 + 3x + C  B) 2x^2 + 3x + C  C) x^2 + 3 + C  D) 2 + C   Answer: A) x^2 + 3x + C
- Q: What is the integral of f(x) = tan(x)?
  Options: A) sec^2(x) + C  B) -ln|cos(x)| + C  C) ln|sin(x)| + C  D) -cot(x) + C   Answer: B) -ln|cos(x)| + C
- Q: Evaluate: int sqrt(x) dx
  Options: A) (2/3)x^(3/2) + C  B) (1/2)x^(1/2) + C  C) 2 sqrt(x) + C  D) (3/2)x^(1/2) + C   Answer: A) (2/3)x^(3/2) + C

<!-- tags: id:QZ-CALC-04, course:calculus, area:calculus, type:quiz, subtopic:applications -->
### QZ-CALC-04 · Applications (8 Qs)
- Q: What is the slope of the tangent line to y = x^2 at x = 2?
  Options: A) 2  B) 4  C) 8  D) 1   Answer: B) 4
- Q: Find the critical points of f(x) = x^3 - 3x^2.
  Options: A) x = 0 only  B) x = 3 only  C) x = 0 and x = 2  D) x = 1 and x = 3   Answer: C) x = 0 and x = 2
- Q: What is the maximum value of f(x) = x^4 - 4x^3 + 4 on [0, 4]?
  Options: A) 4  B) -23  C) 0  D) 260   Answer: A) 4
- Q: Find the minimum value of f(x) = x^2 - 4x + 4.
  Options: A) 0  B) 2  C) 4  D) -4   Answer: A) 0
- Q: What is the rate of change of f(x) = x^2 at x = 3?
  Options: A) 3  B) 6  C) 9  D) 12   Answer: B) 6
- Q: Find the derivative of f(x) = x^2 sin(x).
  Options: A) 2x sin(x)  B) x^2 cos(x)  C) 2x sin(x) + x^2 cos(x)  D) 2x cos(x) - x^2 sin(x)   Answer: C) 2x sin(x) + x^2 cos(x)
- Q: What is the slope of the tangent line to y = ln(x) at x = 1?
  Options: A) 0  B) 1  C) e  D) undefined   Answer: B) 1
- Q: Find the critical points of f(x) = x^3 - 6x^2 + 11x - 6.
  Options: A) x = 1, 2, 3  B) x = (6 +/- sqrt(3))/3  C) x = 2 only  D) x = 3 +/- sqrt(2)   Answer: B) x = (6 +/- sqrt(3))/3

---

## 4D. Expansion Quiz — Precalculus (A-coded, 19 Qs)

<!-- tags: id:QZ-EA-01, course:precalc, area:algebra, type:quiz, code:A1, subtopic:domain-range -->
### QZ-EA-01 · A1. Domain & Range (2 Qs)
- Q: What is the domain of f(x) = sqrt(x - 2)?
  Options: A) [2, inf)  B) (2, inf)  C) (-inf, 2]  D) All reals   Answer: A) [2, inf)
- Q: What is the range of f(x) = x^2?
  Options: A) All reals  B) [0, inf)  C) (0, inf)  D) (-inf, 0]   Answer: B) [0, inf)

<!-- tags: id:QZ-EA-02, course:precalc, area:precalc-general, type:quiz, code:A2, subtopic:rates-of-change -->
### QZ-EA-02 · A2. Rates of Change (2 Qs)
- Q: If f(x) = x^2 - 4x, what is the average rate of change on [1, 3]?
  Options: A) 0  B) -2  C) 2  D) 4   Answer: A) 0
- Q: A function that is concave down has what shape?
  Options: A) Frown (cap)  B) Smile (cup)  C) Straight line  D) Vertical   Answer: A) Frown (cap)

<!-- tags: id:QZ-EA-03, course:precalc, area:algebra, type:quiz, code:A3, subtopic:function-composition -->
### QZ-EA-03 · A3. Composition (2 Qs)
- Q: If f(x) = 2x + 1 and g(x) = x^2, what is (f o g)(3)?
  Options: A) 49  B) 19  C) 7  D) 13   Answer: B) 19
- Q: f(g(x)) is the same as g(f(x)). True or false?
  Options: A) True  B) False   Answer: B) False

<!-- tags: id:QZ-EA-04, course:precalc, area:algebra, type:quiz, code:A4, subtopic:linear-functions -->
### QZ-EA-04 · A4. Linear Functions (1 Q)
- Q: What is the slope of a line passing through (-1, 4) and (5, 2)?
  Options: A) -1/3  B) 1/3  C) -3  D) 3   Answer: A) -1/3

<!-- tags: id:QZ-EA-05, course:precalc, area:algebra, type:quiz, code:A5, subtopic:polynomials-deep -->
### QZ-EA-05 · A5. Polynomials Deep (2 Qs)
- Q: What is the end behavior of f(x) = -2x^5 + 3x^2 - 1?
  Options: A) Both ends up  B) Both ends down  C) Left up, right down  D) Left down, right up   Answer: C) Left up, right down
- Q: At a zero of multiplicity 3, the graph:
  Options: A) Bounces  B) Crosses linearly  C) Crosses with flattening  D) Has a vertical asymptote   Answer: C) Crosses with flattening

<!-- tags: id:QZ-EA-06, course:precalc, area:algebra, type:quiz, code:A6, subtopic:quadratics-expanded -->
### QZ-EA-06 · A6. Quadratics Expanded (1 Q)
- Q: What is the vertex of f(x) = -x^2 + 6x - 5?
  Options: A) (3, 4)  B) (-3, -4)  C) (3, -4)  D) (-3, 4)   Answer: A) (3, 4)

<!-- tags: id:QZ-EA-07, course:precalc, area:algebra, type:quiz, code:A7, subtopic:factor-remainder -->
### QZ-EA-07 · A7. Factor & Remainder (2 Qs)
- Q: If p(x) = x^3 - 4x^2 + 5x - 14, what is the remainder when divided by (x - 2)?
  Options: A) 0  B) -12  C) -16  D) 2   Answer: B) -12
- Q: If p(3) = 0 for polynomial p(x), which is true?
  Options: A) (x + 3) is a factor  B) (x - 3) is a factor  C) x = -3 is a zero  D) None of these   Answer: B) (x - 3) is a factor

<!-- tags: id:QZ-EA-08, course:precalc, area:algebra, type:quiz, code:A8, subtopic:real-zeros -->
### QZ-EA-08 · A8. Real Zeros (1 Q)
- Q: What are the possible rational zeros of f(x) = 3x^3 - x^2 + 2?
  Options: A) +/-{1, 2, 1/3, 2/3}  B) +/-{1, 3}  C) +/-{1, 2}  D) +/-{2, 3}   Answer: A) +/-{1, 2, 1/3, 2/3}

<!-- tags: id:QZ-EA-09, course:precalc, area:algebra, type:quiz, code:A9, subtopic:complex-zeros -->
### QZ-EA-09 · A9. Complex Zeros (2 Qs)
- Q: What are the zeros of f(x) = x^2 + 4?
  Options: A) +/-2  B) +/-2i  C) +/-4i  D) No zeros   Answer: B) +/-2i
- Q: How many complex zeros does a degree-5 polynomial have?
  Options: A) At most 5  B) Exactly 5  C) At least 1  D) Both B and C   Answer: D) Both B and C

<!-- tags: id:QZ-EA-10, course:precalc, area:algebra, type:quiz, code:A10, subtopic:rational-functions-deep -->
### QZ-EA-10 · A10. Rational Functions Deep (1 Q)
- Q: f(x) = (x - 2)/((x - 2)(x + 3)) has:
  Options: A) VA at x=2 and x=-3  B) Hole at x=2, VA at x=-3  C) VA at x=-3 only  D) Both B and C   Answer: B) Hole at x=2, VA at x=-3

<!-- tags: id:QZ-EA-11, course:precalc, area:algebra, type:quiz, code:A11, subtopic:inverses-radicals -->
### QZ-EA-11 · A11. Inverses & Radicals (1 Q)
- Q: Solve sqrt(x + 3) = 5.
  Options: A) x = 22  B) x = 28  C) x = 8  D) x = 2   Answer: A) x = 22

<!-- tags: id:QZ-EA-12, course:precalc, area:algebra, type:quiz, code:A12, subtopic:exponential-models -->
### QZ-EA-12 · A12. Exponential Models (1 Q)
- Q: An investment of $1000 at 5% compounded continuously is worth how much after 10 years?
  Options: A) $1,628.89  B) $1,500  C) $1,648.72  D) $1,050   Answer: C) $1,648.72

<!-- tags: id:QZ-EA-13, course:precalc, area:algebra, type:quiz, code:A13, subtopic:logarithmic-models -->
### QZ-EA-13 · A13. Logarithmic Models (1 Q)
- Q: Solve: log_3(x + 1) = 2
  Options: A) x = 8  B) x = 7  C) x = 9  D) x = 5   Answer: A) x = 8

---

## 4E. Expansion Quiz — Trigonometry (B-coded, 20 Qs)

<!-- tags: id:QZ-EB-01, course:precalc, area:trig, type:quiz, code:B1, subtopic:angles-measure -->
### QZ-EB-01 · B1. Angles & Measure (2 Qs)
- Q: What is the arc length of a circle with radius 10 and central angle 2 radians?
  Options: A) 20  B) 5  C) 10  D) 40   Answer: A) 20
- Q: Which angle is coterminal with 450 deg?
  Options: A) 90 deg  B) 180 deg  C) 270 deg  D) 360 deg   Answer: A) 90 deg

<!-- tags: id:QZ-EB-02, course:precalc, area:trig, type:quiz, code:B2, subtopic:six-functions-identities -->
### QZ-EB-02 · B2. Six Trig Functions (2 Qs)
- Q: If tan(theta) = 3 and theta is in QIII, what is sin(theta)?
  Options: A) 3/sqrt(10)  B) -3/sqrt(10)  C) -1/sqrt(10)  D) 1/sqrt(10)   Answer: B) -3/sqrt(10)
- Q: sec(theta) is the reciprocal of:
  Options: A) sin(theta)  B) cos(theta)  C) tan(theta)  D) cot(theta)   Answer: B) cos(theta)

<!-- tags: id:QZ-EB-03, course:precalc, area:trig, type:quiz, code:B3, subtopic:trig-identities-proofs -->
### QZ-EB-03 · B3. Trig Identities Proofs (2 Qs)
- Q: What is sin(2theta) equal to?
  Options: A) 2sin(theta)  B) sin^2(theta)  C) 2sin(theta)*cos(theta)  D) cos^2(theta) - sin^2(theta)   Answer: C) 2sin(theta)*cos(theta)
- Q: cos(A - B) =
  Options: A) cosA*cosB + sinA*sinB  B) cosA*cosB - sinA*sinB  C) sinA*cosB - cosA*sinB  D) sinA*cosB + cosA*sinB   Answer: A) cosA*cosB + sinA*sinB

<!-- tags: id:QZ-EB-04, course:precalc, area:trig, type:quiz, code:B4, subtopic:trig-graphs -->
### QZ-EB-04 · B4. Trig Graphs (1 Q)
- Q: The period of y = sec(3x) is:
  Options: A) 2pi  B) 2pi/3  C) pi/3  D) 3pi   Answer: B) 2pi/3

<!-- tags: id:QZ-EB-05, course:precalc, area:trig, type:quiz, code:B5, subtopic:inverse-trig -->
### QZ-EB-05 · B5. Inverse Trig (2 Qs)
- Q: arctan(1) = ?
  Options: A) pi/6  B) pi/4  C) pi/3  D) pi/2   Answer: B) pi/4
- Q: The domain of arcsin(x) is:
  Options: A) All reals  B) [-1, 1]  C) [0, 1]  D) (-pi/2, pi/2)   Answer: B) [-1, 1]

<!-- tags: id:QZ-EB-06, course:precalc, area:trig, type:quiz, code:B6, subtopic:trig-equations -->
### QZ-EB-06 · B6. Trig Equations (2 Qs)
- Q: How many solutions does sin(x) = 1/2 have in [0, 2pi)?
  Options: A) 1  B) 2  C) 3  D) Infinite   Answer: B) 2
- Q: The general solution to tan(x) = 1 is:
  Options: A) x = pi/4 + 2pi*k  B) x = pi/4 + pi*k  C) x = pi/4 only  D) x = 3pi/4 + pi*k   Answer: B) x = pi/4 + pi*k

<!-- tags: id:QZ-EB-07, course:precalc, area:trig, type:quiz, code:B7, subtopic:law-of-sines -->
### QZ-EB-07 · B7. Law of Sines (1 Q)
- Q: The Law of Sines is useful when you know:
  Options: A) SSS  B) SAS  C) AAS  D) All of these   Answer: C) AAS

<!-- tags: id:QZ-EB-08, course:precalc, area:trig, type:quiz, code:B8, subtopic:law-of-cosines -->
### QZ-EB-08 · B8. Law of Cosines (1 Q)
- Q: Given a = 8, b = 6, c = 10, find angle C.
  Options: A) 90 deg  B) 60 deg  C) 120 deg  D) 45 deg   Answer: A) 90 deg

<!-- tags: id:QZ-EB-09, course:precalc, area:trig, type:quiz, code:B9, subtopic:polar-coordinates -->
### QZ-EB-09 · B9. Polar Coordinates (1 Q)
- Q: The Cartesian coordinates of the polar point (4, pi/3) are:
  Options: A) (2, 2*sqrt(3))  B) (2*sqrt(3), 2)  C) (4, 4)  D) (2, 2)   Answer: A) (2, 2*sqrt(3))

<!-- tags: id:QZ-EB-10, course:precalc, area:trig, type:quiz, code:B10, subtopic:vectors -->
### QZ-EB-10 · B10. Vectors (2 Qs)
- Q: What is the dot product of <1, 2> and <-2, 1>?
  Options: A) 0  B) 4  C) -4  D) 2   Answer: A) 0
- Q: The work done by a force F = 10 lbs at 30 deg over 50 ft is:
  Options: A) 250*sqrt(3)  B) 500  C) 250  D) 125*sqrt(3)   Answer: A) 250*sqrt(3)

<!-- tags: id:QZ-EB-11, course:precalc, area:trig, type:quiz, code:B11, subtopic:parametric-equations -->
### QZ-EB-11 · B11. Parametric Equations (1 Q)
- Q: The parametric equations x = 3cos(t), y = 3sin(t) trace out:
  Options: A) A line  B) A parabola  C) A circle of radius 3  D) An ellipse   Answer: C) A circle of radius 3

<!-- tags: id:QZ-EB-12, course:precalc, area:trig, type:quiz, code:B12, subtopic:polar-complex -->
### QZ-EB-12 · B12. Polar Complex (1 Q)
- Q: The modulus of z = 3 + 4i is:
  Options: A) 5  B) 7  C) sqrt(7)  D) 25   Answer: A) 5

<!-- tags: id:QZ-EB-13, course:precalc, area:trig, type:quiz, code:B13, subtopic:harmonic-motion -->
### QZ-EB-13 · B13. Harmonic Motion (1 Q)
- Q: The period of S(t) = 5sin(pi*t/3) is:
  Options: A) 6  B) 3  C) pi/3  D) 2pi/3   Answer: A) 6

<!-- tags: id:QZ-EB-14, course:precalc, area:trig, type:quiz, code:B14, subtopic:polar-conics-rotation -->
### QZ-EB-14 · B14. Polar Conics (1 Q)
- Q: A conic with eccentricity e = 0.5 is:
  Options: A) Circle  B) Ellipse  C) Parabola  D) Hyperbola   Answer: B) Ellipse

---
---

# PART 5 — CONTENT TOTALS & FEATURES
# ====================================

## Content Totals

| Category | Original | Expansion | Total |
| --- | --- | --- | --- |
| Review Cards | ~25 sections | 27 topics | ~52 sections |
| Flashcards | 45 cards | 76 cards | ~121 cards |
| Quiz Questions | 50 (15 precalc + 35 calculus) | 39 questions | 89 questions |

## Features
- Topic navigation dropdown in Review tab with smooth scroll and highlight
- Topic filter dropdowns in Flashcards and Quiz tabs
- Cross-tab sync: selecting an expansion topic in Review auto-sets flashcard/quiz filters
- Priority tier badges: Tier 1 (Essential), Tier 2 (Important), Tier 3 (Advanced)
- Sidebar navigation with grouped expansion topics
- Quiz history with localStorage persistence and CSV export
- Yu-Gi-Oh! crossover sections on 10 expansion topics (collapsible)

---

# APPENDIX — TAG INDEX (for programmatic lookup)
# ================================================
#
# To filter by course:
#   grep "course:precalc" this_file.md
#   grep "course:calculus" this_file.md
#
# To filter by area:
#   grep "area:algebra" this_file.md
#   grep "area:trig" this_file.md
#   grep "area:calculus" this_file.md
#   grep "area:precalc-general" this_file.md
#
# To filter by type:
#   grep "type:review-card" this_file.md
#   grep "type:expansion-review" this_file.md
#   grep "type:flashcard" this_file.md
#   grep "type:quiz" this_file.md
#
# To filter by tier:
#   grep "tier:1-essential" this_file.md
#   grep "tier:2-important" this_file.md
#   grep "tier:3-advanced" this_file.md
#
# To filter by expansion code:
#   grep "code:A1" this_file.md
#   grep "code:B13" this_file.md
#
# To get all items with Yu-Gi-Oh! crossover:
#   grep "yugioh:yes" this_file.md
