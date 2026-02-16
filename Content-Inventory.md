# Precalc Review Master Content Inventory

Source: Study-Buddy_App.html

## Review Cards (Review Tab)

### Algebra

**Functions and Notation**
- f(x) means "plug x into the expression".
- f(3) = replace every x with 3.
- f(a + h) = replace x with (a + h).
- Domain: all valid x-values (watch for division by zero, sqrt of negatives, log issues).
- Range: all possible y-values.

**Factoring Patterns**
- Difference of squares: a^2 - b^2 = (a + b)(a - b)
- Perfect square: a^2 +/- 2ab + b^2 = (a +/- b)^2
- Sum/difference of cubes: a^3 +/- b^3 = (a +/- b)(a^2 -/+ ab + b^2)

**Solving Quadratics**
- Quadratic formula: x = (-b +/- sqrt(b^2 - 4ac)) / (2a)
- Discriminant: Delta = b^2 - 4ac
  - Delta > 0: two real solutions
  - Delta = 0: one solution
  - Delta < 0: no real solutions

**More Algebra Skills**
- Completing the square:
  - x^2 + bx -> x^2 + bx + (b/2)^2 - (b/2)^2 = (x + b/2)^2 - (b/2)^2
  - Example: x^2 + 6x + 1 = 0 -> (x + 3)^2 = 8 -> x = -3 +/- 2*sqrt(2)
- Rationalizing denominators:
  - 1/sqrt(a) -> multiply by sqrt(a)/sqrt(a)
  - 1/(a + sqrt(b)) -> multiply by (a - sqrt(b))/(a - sqrt(b))
  - Use the conjugate to eliminate radicals in the denominator.

**Rational Functions**
- Vertical asymptotes: set denominator = 0.
- Horizontal asymptotes:
  - deg(P) < deg(Q) -> y = 0
  - deg(P) = deg(Q) -> y = leading coefficient ratio
  - deg(P) > deg(Q) -> none

**Inverse Functions**
- Steps:
  1. Write y = f(x)
  2. Swap x and y
  3. Solve for y
  4. Write f^-1(x)
- Graphs are reflections across y = x.

**Lines and Slopes**
- Slope: m = (y2 - y1) / (x2 - x1)
- Forms of linear equations:
  - Slope-intercept: y = mx + b
  - Point-slope: y - y1 = m(x - x1)
  - Standard: Ax + By = C
- Parallel lines: same slope (m1 = m2)
- Perpendicular lines: negative reciprocal slopes (m1 * m2 = -1)

**Absolute Value and Piecewise**
- |x| = x if x >= 0, and -x if x < 0
- Solving |expression| = k:
  - expression = k OR expression = -k
- Absolute value inequalities:
  - |expr| < k -> -k < expr < k
  - |expr| > k -> expr < -k OR expr > k
- Piecewise functions: choose the rule based on the domain condition.

**Function Transformations**
- y = a * f(b(x - h)) + k
  - k: vertical shift
  - h: horizontal shift
  - a: vertical stretch/compress
  - b: horizontal compress/stretch
- Reflections:
  - -f(x): reflect over x-axis
  - f(-x): reflect over y-axis
- Inside changes affect x (opposite direction); outside changes affect y (same direction).

**Inequalities**
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

### Exponentials and Logs

**Exponentials and Logs**
- Core relationship: a^x = y <-> log_a(y) = x
- Natural base: e^x = y <-> ln(y) = x
- Exponentials and logs are inverse operations.

**Log Properties**
- Product: log(MN) = log(M) + log(N)
- Quotient: log(M/N) = log(M) - log(N)
- Power: log(M^k) = k * log(M)
- Wrong rule: ln(a + b) != ln(a) + ln(b)

### Trigonometry

**The Unit Circle (Review Tab)**
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

**Quick Trig Reference**

| Angle | sin | cos | tan |
| --- | --- | --- | --- |
| 0 / pi/2 | 0 / 1 | 1 / 0 | 0 / undef |
| pi/6 (30) | 1/2 | sqrt(3)/2 | sqrt(3)/3 |
| pi/4 (45) | sqrt(2)/2 | sqrt(2)/2 | 1 |
| pi/3 (60) | sqrt(3)/2 | 1/2 | sqrt(3) |

**Key Identities**
- sin^2(x) + cos^2(x) = 1
- tan(x) = sin(x) / cos(x)
- sin(2x) = 2 sin(x) cos(x)
- Even/odd:
  - sin(-x) = -sin(x)
  - cos(-x) = cos(x)

**Sinusoidal Models**
- y = A sin(bx + c) + D
  - A = amplitude
  - b = 2pi / period
  - D = vertical shift (midline)

### Sequences and Series
- Arithmetic sequence (constant difference d):
  - an = a1 + (n - 1)d
  - Sum: Sn = n(a1 + an)/2
- Geometric sequence (constant ratio r):
  - an = a1 * r^(n-1)
  - Sum: Sn = a1(1 - r^n) / (1 - r)
- Infinite geometric series converges when |r| < 1:
  - S = a1 / (1 - r)

### Limits (Calculus Preview)
- Core idea: what value does f(x) approach as x -> c?
- Strategy:
  1. Try direct substitution
  2. If 0/0, factor/cancel/rationalize
  3. For limits at infinity, divide by highest power of x
- Key facts:
  - lim(x->0) sin(x)/x = 1
  - lim(x->inf) 1/x^n = 0 for n > 0
  - lim(x->a) [polynomial] = substitute a

### Common Mistakes to Avoid
- ln(a + b) != ln(a) + ln(b)
- (a + b)^2 != a^2 + b^2 -> a^2 + 2ab + b^2
- sqrt(a^2 + b^2) != a + b
- 1/(a + b) != 1/a + 1/b
- Also watch out for:
  - forgetting to flip inequality sign when multiplying/dividing by a negative
  - ignoring domain restrictions (division by 0, sqrt of negatives, log of <= 0)
  - dropping parentheses: -3^2 = -9 but (-3)^2 = 9

### Calculator Skills
- Essential buttons: sin, cos, tan, sin^-1, cos^-1, tan^-1, ln, log, e^x, 10^x, x^2, sqrt, pi, ^
- Always check degree vs radian mode (use radian for calculus).
- Change of base: log_a(M) = ln(M) / ln(a)
- Parentheses matter: -3^2 = -9 vs (-3)^2 = 9

### Calculus Preview Topics

**What Is a Function?**
- Relationship between domain (inputs) and codomain (outputs), one output per input.
- Vertical line test.
- Descriptions: algebraic, graphical, numerical, verbal.
- Types: polynomial, rational, exponential, logarithmic, trigonometric.
- Example: f(x) = 2x + 3 (linear, slope 2, y-intercept 3).

**What Is a Limit?**
- lim(x->a) f(x) = L.
- Two-sided and one-sided limits.
- Techniques: direct substitution, factoring, rationalizing.
- Example: lim(x->1) (x^2 - 1)/(x - 1) = 2.

**What Is a Derivative?**
- f'(x) = lim(h->0) [f(x+h) - f(x)] / h
- Interpretations: tangent slope, instantaneous rate of change.
- Rules: power, product, quotient, chain.
- Example: f(x) = x^2 -> f'(x) = 2x, slope at x=2 is 4.

**What Is an Integral?**
- Integral from a to b is area under the curve.
- Definite vs indefinite integrals.
- Techniques: antiderivatives, substitution, integration by parts, partial fractions.
- Example: int_0^1 x^2 dx = 1/3.

**What Is Continuity?**
- Conditions at x = a:
  1. f(a) defined
  2. lim(x->a) f(x) exists
  3. lim(x->a) f(x) = f(a)
- Discontinuities: removable, jump, infinite.
- Intermediate Value Theorem (IVT).

### Calculus Topics

**Quick Reference Chart**

| Term | Meaning |
| --- | --- |
| Critical point | f'(x) = 0 or undefined |
| Increasing interval | f'(x) > 0 |
| Decreasing interval | f'(x) < 0 |
| Inflection point | f''(x) = 0 with sign change |
| Concave up | f''(x) > 0 |
| Concave down | f''(x) < 0 |

**Graph Reference Key**

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

**Definitions**

| Term | Condition | Meaning |
| --- | --- | --- |
| Critical point | f'(x) = 0 | Horizontal tangent (max/min) |
| Increasing | f'(x) > 0 | Function rising |
| Decreasing | f'(x) < 0 | Function falling |
| Inflection point | f''(x) = 0 (sign change) | Concavity changes |
| Concave up | f''(x) > 0 | Curves upward |
| Concave down | f''(x) < 0 | Curves downward |

**Rolle's Theorem**
- Conditions:
  1. f continuous on [a, b]
  2. f differentiable on (a, b)
  3. f(a) = f(b)
- If all 3 hold, there exists c in (a, b) with f'(c) = 0.

**Mean Value Theorem (MVT)**
- Conditions:
  1. f continuous on [a, b]
  2. f differentiable on (a, b)
- There exists c in (a, b) with f'(c) = (f(b) - f(a)) / (b - a).

**Corollaries**
- If f'(x) = 0 for all x in I, then f(x) is constant on I.
- If f'(x) = g'(x) for all x in I, then f(x) = g(x) + C.
- If f'(x) > 0 on (a, b), f increases on [a, b]. If f'(x) < 0 on (a, b), f decreases on [a, b].

**First Derivative Test**
- f' changes + -> - at c: local maximum
- f' changes - -> + at c: local minimum
- f' same sign on both sides: neither

**Second Derivative Test**
- Steps:
  1. Find critical points from f'(x) = 0
  2. Compute f''(x)
  3. Evaluate f''(c)
- f''(c) > 0 -> local minimum
- f''(c) < 0 -> local maximum
- f''(c) = 0 -> inconclusive (use first derivative test)

**Graphing with Derivatives**
- Step 1: Find f'(x); locate critical points and increasing/decreasing intervals.
- Step 2: Find f''(x); locate inflection points and concavity.
- Step 3: Analyze sign charts for f'(x), f''(x).
- Step 4: Identify key points (local max/min, inflection).
- Step 5: Sketch using behavior info.

**Integration Formulas**

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

## Unit Circle Tab (Trigonometry Deep Dive)

**Understanding the Unit Circle**
- Unit circle: radius 1 centered at (0, 0). Every point is (cos(theta), sin(theta)).
- Key insight: x-coordinate = cos(theta), y-coordinate = sin(theta).
- Conversion formulas:
  - Radians to degrees: degrees = (180/pi) * radians
  - Degrees to radians: radians = (pi/180) * degrees
- Key angles to memorize: 0, 30 (pi/6), 45 (pi/4), 60 (pi/3), 90 (pi/2).

**Complete Unit Circle Reference Table**

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

**Quadrant Patterns**
- Quadrant I: all trig functions positive.
- Quadrant II: sin positive, cos and tan negative.
- Quadrant III: tan positive, sin and cos negative.
- Quadrant IV: cos positive, sin and tan negative.
- Study tip: master Quadrant I first, then use reference angles and sign patterns.

## Flashcards

### Precalc Flashcards

**Functions (4)**
- Q: What does f(a + h) mean?
  A: Replace every x in the function rule with (a + h). Example: if f(x) = x^2, then f(a + h) = (a + h)^2 = a^2 + 2ah + h^2.
- Q: What three things restrict the domain of a function?
  A: Division by zero (denominator != 0), even roots of negatives (radicand >= 0), logarithms of non-positives (argument > 0).
- Q: How do you evaluate the composition (f o g)(x)?
  A: (f o g)(x) = f(g(x)). Evaluate g(x) first, then plug into f. Domain: x in domain of g with g(x) in domain of f.
- Q: What is the difference between domain and range?
  A: Domain = all valid input values. Range = all possible outputs.

**Exponentials (4)**
- Q: State the core relationship between exponentials and logarithms.
  A: a^x = y <-> log_a(y) = x. They are inverse operations.
- Q: State all three logarithm properties (product, quotient, power).
  A: log(MN) = log(M) + log(N); log(M/N) = log(M) - log(N); log(M^k) = k * log(M).
- Q: What is the change of base formula?
  A: log_a(M) = ln(M) / ln(a).
- Q: State three key log/exp values you must memorize.
  A: ln(1) = 0, ln(e) = 1, e^(ln(x)) = x. Also log_a(1) = 0 and log_a(a) = 1.

**Trigonometry (4)**
- Q: State the Pythagorean identity.
  A: sin^2(x) + cos^2(x) = 1.
- Q: State both double-angle formulas for sin(2x) and cos(2x).
  A: sin(2x) = 2 sin(x) cos(x). cos(2x) = cos^2(x) - sin^2(x) = 2 cos^2(x) - 1 = 1 - 2 sin^2(x).
- Q: Which trig functions are even and which are odd?
  A: Even: cos(-x) = cos(x), sec(-x) = sec(x). Odd: sin(-x) = -sin(x), tan(-x) = -tan(x), csc(-x) = -csc(x), cot(-x) = -cot(x).
- Q: Express tan(x) and the two other Pythagorean identities.
  A: tan(x) = sin(x)/cos(x); 1 + tan^2(x) = sec^2(x); 1 + cot^2(x) = csc^2(x).

**Unit Circle (4)**
- Q: What are cos(pi/6) and sin(pi/6)?
  A: cos(pi/6) = sqrt(3)/2 and sin(pi/6) = 1/2.
- Q: What are cos(pi/4) and sin(pi/4)?
  A: cos(pi/4) = sqrt(2)/2 and sin(pi/4) = sqrt(2)/2.
- Q: Which trig functions are positive in each quadrant?
  A: QI: all positive. QII: sin, csc. QIII: tan, cot. QIV: cos, sec. Mnemonic: All Students Take Calculus.
- Q: How do you convert between degrees and radians?
  A: Degrees -> radians: multiply by pi/180. Radians -> degrees: multiply by 180/pi. Example: 60 deg * (pi/180) = pi/3.

**Sinusoidal (3)**
- Q: In y = A sin(bx + c) + D, what does each parameter control?
  A: A = amplitude, b = frequency with period 2pi/b, c = phase constant with phase shift -c/b, D = vertical shift (midline y = D).
- Q: How do you find the period of y = 3 sin(2x) - 5?
  A: Period = 2pi/b = 2pi/2 = pi.
- Q: How do you find amplitude from a graph showing max and min values?
  A: Amplitude = (max - min)/2. Midline D = (max + min)/2.

**Polynomials (3)**
- Q: How does the degree and leading coefficient determine end behavior?
  A: Even degree, positive lead -> both ends +inf. Even degree, negative lead -> both ends -inf. Odd degree, positive lead -> left -inf, right +inf. Odd degree, negative lead -> left +inf, right -inf.
- Q: How do you find the horizontal asymptote of a rational function P(x)/Q(x)?
  A: Compare degrees: deg(P) < deg(Q) -> y = 0; deg(P) = deg(Q) -> ratio of leading coefficients; deg(P) > deg(Q) -> no horizontal asymptote.
- Q: How do you find vertical asymptotes of a rational function?
  A: Set denominator = 0. x = a is a vertical asymptote only if the numerator is not also 0 at x = a.

**Algebra Skills (4)**
- Q: State the difference of squares and sum/difference of cubes patterns.
  A: a^2 - b^2 = (a + b)(a - b); a^3 + b^3 = (a + b)(a^2 - ab + b^2); a^3 - b^3 = (a - b)(a^2 + ab + b^2).
- Q: State the quadratic formula and explain the discriminant.
  A: x = (-b +/- sqrt(b^2 - 4ac)) / (2a). Delta > 0 two distinct real roots; Delta = 0 one repeated real root; Delta < 0 no real roots.
- Q: What are the steps to complete the square for x^2 + bx?
  A: Take half of b, square it, add and subtract: x^2 + bx = (x + b/2)^2 - (b/2)^2. Example: x^2 + 6x = (x + 3)^2 - 9.
- Q: How do you rationalize a denominator with a binomial radical like 1/(sqrt(a) + b)?
  A: Multiply numerator and denominator by the conjugate (sqrt(a) - b).

**Lines (3)**
- Q: State the slope formula and the three main forms of a line.
  A: m = (y2 - y1)/(x2 - x1). Forms: y = mx + b, y - y1 = m(x - x1), Ax + By = C.
- Q: What is the relationship between slopes of parallel and perpendicular lines?
  A: Parallel: same slope. Perpendicular: negative reciprocal slopes (m1 * m2 = -1).
- Q: What does a slope of zero vs. an undefined slope look like?
  A: Slope 0 -> horizontal line. Undefined slope -> vertical line (not a function).

**Absolute Value and Piecewise (3)**
- Q: State the formal definition of |x|.
  A: |x| = x if x >= 0, and -x if x < 0.
- Q: How do you solve |expression| = k?
  A: If k > 0: expression = k or expression = -k. If k = 0: expression = 0. If k < 0: no solution.
- Q: How do you solve |expression| < k (k > 0)?
  A: -k < expression < k. For |expression| > k: expression < -k or expression > k.

**Inverses (3)**
- Q: What is the definition of an inverse function?
  A: f and g are inverses if f(g(x)) = x and g(f(x)) = x. Domain and range swap.
- Q: What are the steps to find an inverse function algebraically?
  A: 1) y = f(x). 2) Swap x and y. 3) Solve for y. 4) Write f^-1(x). 5) Verify f(f^-1(x)) = x.
- Q: How are the graphs of f and f^-1 related?
  A: f^-1 is the reflection of f across y = x.

**Transformations (4)**
- Q: What does y = f(x) + k do to the graph? What about y = f(x + h)?
  A: y = f(x) + k shifts up by k (down if k < 0). y = f(x + h) shifts left by h (right if h < 0).
- Q: How do vertical and horizontal stretches/compressions work?
  A: y = a f(x) stretches vertically by |a| if |a| > 1 (compress if 0 < |a| < 1). y = f(bx) compresses horizontally by 1/|b| if |b| > 1 (stretch if 0 < |b| < 1).
- Q: What do y = -f(x) and y = f(-x) do?
  A: -f(x) reflects across the x-axis. f(-x) reflects across the y-axis.
- Q: In what order should you apply multiple transformations?
  A: 1) Horizontal stretch/compress and reflection (inside). 2) Horizontal shift. 3) Vertical stretch/compress and reflection. 4) Vertical shift (outside).

**Inequalities (3)**
- Q: What critical rule must you remember when solving inequalities?
  A: Multiply/divide by a negative -> flip the inequality sign.
- Q: How does the sign chart method work for polynomial/rational inequalities?
  A: Move to one side, factor, find zeros/undefined points, test signs in intervals, choose intervals that satisfy the inequality.
- Q: How do you write solutions in interval notation?
  A: Use ( ) for strict and [ ] for inclusive. Use parentheses with inf. Example: -3 <= x < 5 is [-3, 5). Use union for disjoint intervals.

**Sequences (4)**
- Q: State the formulas for the nth term and sum of an arithmetic sequence.
  A: an = a1 + (n - 1)d; Sn = n(a1 + an)/2.
- Q: State the formulas for the nth term and sum of a geometric sequence.
  A: an = a1 * r^(n-1); Sn = a1(1 - r^n)/(1 - r).
- Q: What is the formula for an infinite geometric series, and when does it converge?
  A: S = a1/(1 - r), valid only when |r| < 1.
- Q: How do you determine if a sequence is arithmetic vs. geometric?
  A: Arithmetic has constant difference; geometric has constant ratio.

**Limits (3)**
- Q: What does lim(x->a) f(x) = L mean intuitively?
  A: As x approaches a, f(x) approaches L. f(a) does not need to exist.
- Q: What are the common indeterminate forms, and what do you do about 0/0?
  A: Common: 0/0 and inf/inf. For 0/0: factor, rationalize, or simplify to cancel, then substitute.
- Q: How do you find the limit of a polynomial as x -> c?
  A: Substitute x = c (polynomials are continuous).

**Common Mistakes (3)**
- Q: Why is ln(a + b) != ln(a) + ln(b)?
  A: Log product rule requires multiplication inside, not addition.
- Q: What is the correct expansion of (a + b)^2?
  A: a^2 + 2ab + b^2.
- Q: Is sqrt(a^2 + b^2) equal to a + b?
  A: No. sqrt does not distribute over addition.

**Calculator (3)**
- Q: When should your calculator be in radian mode vs degree mode?
  A: Use radian mode for calculus and most precalc problems (especially with pi). Use degree mode only when angles are given in degrees.
- Q: How do you compute log base 5 of 20 on a calculator that only has ln?
  A: log_5(20) = ln(20) / ln(5) approx 1.861.
- Q: What is a common calculator pitfall with negative numbers and exponents?
  A: -3^2 = -9 (exponent first). Use parentheses: (-3)^2 = 9.

### Calculus Flashcards

**Calc Limits (7)**
- Q: What is the limit of f(x) = 3x^2 - 2x + 1 as x approaches 2?
  A: 9.
- Q: What is the value of lim(x->0) sin(x)/x?
  A: 1.
- Q: What is the limit of (x^2 - 4)/(x - 2) as x approaches 2?
  A: 4.
- Q: What is the value of lim(x->inf) (2x^2 + 3x)/(x^2 + 1)?
  A: 2.
- Q: What is the limit of 1/x as x approaches infinity?
  A: 0.
- Q: What is the value of lim(x->3) (x^2 - 9)/(x - 3)?
  A: 6.
- Q: What is the limit of e^x as x approaches negative infinity?
  A: 0.

**Calc Derivatives (10)**
- Q: What is the derivative of f(x) = x^3?
  A: 3x^2.
- Q: What is the derivative of f(x) = sin(x)?
  A: cos(x).
- Q: What is the derivative of f(x) = e^x?
  A: e^x.
- Q: What is the derivative of f(x) = ln(x)?
  A: 1/x.
- Q: What is the derivative of f(x) = x^2 + 3x - 4?
  A: 2x + 3.
- Q: What is the derivative of f(x) = cos(x)?
  A: -sin(x).
- Q: What is the derivative of f(x) = tan(x)?
  A: sec^2(x).
- Q: What is the derivative of f(x) = x sin(x)?
  A: sin(x) + x cos(x).
- Q: What is the derivative of f(x) = 1/x?
  A: -1/x^2.
- Q: What is the derivative of f(x) = x^4 - 2x^3 + 5x^2 - 3x + 1?
  A: 4x^3 - 6x^2 + 10x - 3.

**Calc Integrals (10)**
- Q: What is the integral of f(x) = x^2?
  A: x^3/3 + C.
- Q: What is the value of int e^x dx?
  A: e^x + C.
- Q: What is the integral of f(x) = sin(x)?
  A: -cos(x) + C.
- Q: What is the value of int (1/x) dx?
  A: ln|x| + C.
- Q: What is the integral of f(x) = cos(x)?
  A: sin(x) + C.
- Q: What is the value of int x^3 dx?
  A: x^4/4 + C.
- Q: What is the integral of f(x) = 1/x^2?
  A: -1/x + C.
- Q: What is the value of int (2x + 3) dx?
  A: x^2 + 3x + C.
- Q: What is the integral of f(x) = tan(x)?
  A: -ln|cos(x)| + C (equivalently ln|sec(x)| + C).
- Q: What is the value of int sqrt(x) dx?
  A: (2/3)x^(3/2) + C.

**Calc Applications (8)**
- Q: What is the slope of the tangent line to y = x^2 at x = 2?
  A: 4.
- Q: What are the critical points of f(x) = x^3 - 3x^2?
  A: x = 0 and x = 2.
- Q: What is the maximum value of f(x) = x^4 - 4x^3 + 4 on [0, 4]?
  A: 4 (at x = 0 and x = 4).
- Q: What is the minimum value of f(x) = x^2 - 4x + 4?
  A: 0 (at x = 2).
- Q: What is the rate of change of f(x) = x^2 at x = 3?
  A: 6.
- Q: What is the derivative of f(x) = x^2 sin(x)?
  A: 2x sin(x) + x^2 cos(x).
- Q: What is the slope of the tangent line to y = ln(x) at x = 1?
  A: 1.
- Q: What are the critical points of f(x) = x^3 - 6x^2 + 11x - 6?
  A: x = (6 +/- sqrt(3)) / 3.

## Quiz Questions

### Precalc Quiz (15)

**Functions and Algebra**
- Q: If f(x) = x^2 - 3x + 2, what is f(2)?
  Options: A) 0 B) 2 C) 4 D) 6
  Answer: A) 0
- Q: Factor: x^2 - 9
  Options: A) (x - 3)^2 B) (x + 3)^2 C) (x - 3)(x + 3) D) (x - 3)(x - 3)
  Answer: C) (x - 3)(x + 3)
- Q: Solve: x^2 - 5x + 6 = 0
  Options: A) 1, 6 B) 2, 3 C) -2, -3 D) 2, -3
  Answer: B) 2, 3

**Exponentials and Logs**
- Q: Solve: 2^x = 16
  Options: A) 2 B) 3 C) 4 D) 8
  Answer: C) 4
- Q: Which is equivalent to ln(e^5)?
  Options: A) 1 B) e C) 5 D) e^5
  Answer: C) 5
- Q: Expand: log(x^2 y / z)
  Options: A) 2log(x) + log(y) - log(z) B) log(x) + log(y) - log(z) C) 2log(x) - log(y) - log(z) D) log(2x) + log(y) - log(z)
  Answer: A) 2log(x) + log(y) - log(z)
- Q: What is ln(1)?
  Options: A) 0 B) 1 C) undefined D) e
  Answer: A) 0

**Trigonometry and Unit Circle**
- Q: What is cos(pi/3)?
  Options: A) 0 B) 1/2 C) sqrt(3)/2 D) 1
  Answer: B) 1/2
- Q: Solve: sin(x) = 1/2 for x in [0, 2pi)
  Options: A) pi/6, 5pi/6 B) pi/3, 2pi/3 C) pi/4, 3pi/4 D) pi/6, pi/3
  Answer: A) pi/6, 5pi/6
- Q: Simplify: sin^2(x) + cos^2(x)
  Options: A) 0 B) 1 C) sin(2x) D) tan(x)
  Answer: B) 1
- Q: Find the period of y = cos(pi x)
  Options: A) pi B) 2pi C) 2 D) 1/2
  Answer: C) 2

**Sinusoidal Models**
- Q: Find the amplitude of y = 3sin(2x) - 5
  Options: A) 2 B) 3 C) 5 D) -5
  Answer: B) 3

**Absolute Value**
- Q: Solve: |x - 3| = 5
  Options: A) 3 B) 8, -2 C) 5, -5 D) -2, 8
  Answer: D) -2, 8

**Lines**
- Q: Which are perpendicular lines?
  Options: A) m=2, m=2 B) m=2, m=-1/2 C) m=2, m=1/2 D) m=2, m=1
  Answer: B) m=2, m=-1/2

**Rational Functions**
- Q: For f(x) = 1/(x - 2), what is the vertical asymptote?
  Options: A) x=0 B) x=1 C) x=2 D) x=-2
  Answer: C) x=2

### Calculus Quiz Pool (35)

**Limits (7)**
- Q: What is the limit of f(x) = 3x^2 - 2x + 1 as x approaches 2?
  Options: A) 9 B) 5 C) 11 D) 7
  Answer: A) 9
- Q: Evaluate: lim(x->0) sin(x)/x
  Options: A) 0 B) 1 C) inf D) undefined
  Answer: B) 1
- Q: What is the limit of (x^2 - 4)/(x - 2) as x approaches 2?
  Options: A) 0 B) 2 C) 4 D) undefined
  Answer: C) 4
- Q: Evaluate: lim(x->inf) (2x^2 + 3x)/(x^2 + 1)
  Options: A) 0 B) 1 C) 2 D) 3
  Answer: C) 2
- Q: What is the limit of 1/x as x approaches infinity?
  Options: A) 0 B) 1 C) inf D) undefined
  Answer: A) 0
- Q: Evaluate: lim(x->3) (x^2 - 9)/(x - 3)
  Options: A) 0 B) 3 C) 6 D) 9
  Answer: C) 6
- Q: What is the limit of e^x as x approaches negative infinity?
  Options: A) 0 B) 1 C) -inf D) inf
  Answer: A) 0

**Derivatives (10)**
- Q: What is the derivative of f(x) = x^3?
  Options: A) x^2 B) 3x C) 3x^2 D) x^3
  Answer: C) 3x^2
- Q: Find the derivative of f(x) = sin(x).
  Options: A) cos(x) B) -cos(x) C) -sin(x) D) tan(x)
  Answer: A) cos(x)
- Q: What is the derivative of f(x) = e^x?
  Options: A) x e^(x-1) B) e^x C) e^(x-1) D) ln(x)
  Answer: B) e^x
- Q: Find the derivative of f(x) = ln(x).
  Options: A) x B) 1/x C) ln(x)/x D) e^x
  Answer: B) 1/x
- Q: What is the derivative of f(x) = x^2 + 3x - 4?
  Options: A) 2x + 3 B) x^2 + 3 C) 2x - 4 D) 2x + 3x
  Answer: A) 2x + 3
- Q: Find the derivative of f(x) = cos(x).
  Options: A) sin(x) B) -sin(x) C) -cos(x) D) tan(x)
  Answer: B) -sin(x)
- Q: What is the derivative of f(x) = tan(x)?
  Options: A) sec(x) B) cot(x) C) sec^2(x) D) -csc^2(x)
  Answer: C) sec^2(x)
- Q: Find the derivative of f(x) = x sin(x).
  Options: A) cos(x) B) x cos(x) C) sin(x) + cos(x) D) sin(x) + x cos(x)
  Answer: D) sin(x) + x cos(x)
- Q: What is the derivative of f(x) = 1/x?
  Options: A) 1/x^2 B) -1/x^2 C) ln(x) D) -ln(x)
  Answer: B) -1/x^2
- Q: Find the derivative of f(x) = x^4 - 2x^3 + 5x^2 - 3x + 1.
  Options: A) 4x^3 - 6x^2 + 10x - 3 B) 4x^3 - 2x^2 + 5x - 3 C) x^3 - 6x^2 + 10x - 3 D) 4x^4 - 6x^3 + 10x^2 - 3x
  Answer: A) 4x^3 - 6x^2 + 10x - 3

**Integrals (10)**
- Q: What is the integral of f(x) = x^2?
  Options: A) x^3/3 + C B) 2x + C C) x^3 + C D) x^2/2 + C
  Answer: A) x^3/3 + C
- Q: Evaluate: int e^x dx
  Options: A) e^x + C B) x e^x + C C) e^(x+1)/(x+1) + C D) ln(x) + C
  Answer: A) e^x + C
- Q: What is the integral of f(x) = sin(x)?
  Options: A) cos(x) + C B) -cos(x) + C C) -sin(x) + C D) sin^2(x)/2 + C
  Answer: B) -cos(x) + C
- Q: Evaluate: int (1/x) dx
  Options: A) x + C B) ln(x) + C C) ln|x| + C D) -1/x^2 + C
  Answer: C) ln|x| + C
- Q: What is the integral of f(x) = cos(x)?
  Options: A) sin(x) + C B) -sin(x) + C C) cos^2(x) + C D) tan(x) + C
  Answer: A) sin(x) + C
- Q: Evaluate: int x^3 dx
  Options: A) 3x^2 + C B) x^4 + C C) x^4/4 + C D) x^3/3 + C
  Answer: C) x^4/4 + C
- Q: What is the integral of f(x) = 1/x^2?
  Options: A) -1/x + C B) 1/x + C C) ln(x^2) + C D) -2/x^3 + C
  Answer: A) -1/x + C
- Q: Evaluate: int (2x + 3) dx
  Options: A) x^2 + 3x + C B) 2x^2 + 3x + C C) x^2 + 3 + C D) 2 + C
  Answer: A) x^2 + 3x + C
- Q: What is the integral of f(x) = tan(x)?
  Options: A) sec^2(x) + C B) -ln|cos(x)| + C C) ln|sin(x)| + C D) -cot(x) + C
  Answer: B) -ln|cos(x)| + C
- Q: Evaluate: int sqrt(x) dx
  Options: A) (2/3)x^(3/2) + C B) (1/2)x^(1/2) + C C) 2 sqrt(x) + C D) (3/2)x^(1/2) + C
  Answer: A) (2/3)x^(3/2) + C

**Applications (8)**
- Q: What is the slope of the tangent line to y = x^2 at x = 2?
  Options: A) 2 B) 4 C) 8 D) 1
  Answer: B) 4
- Q: Find the critical points of f(x) = x^3 - 3x^2.
  Options: A) x = 0 only B) x = 3 only C) x = 0 and x = 2 D) x = 1 and x = 3
  Answer: C) x = 0 and x = 2
- Q: What is the maximum value of f(x) = x^4 - 4x^3 + 4 on [0, 4]?
  Options: A) 4 B) -23 C) 0 D) 260
  Answer: A) 4
- Q: Find the minimum value of f(x) = x^2 - 4x + 4.
  Options: A) 0 B) 2 C) 4 D) -4
  Answer: A) 0
- Q: What is the rate of change of f(x) = x^2 at x = 3?
  Options: A) 3 B) 6 C) 9 D) 12
  Answer: B) 6
- Q: Find the derivative of f(x) = x^2 sin(x).
  Options: A) 2x sin(x) B) x^2 cos(x) C) 2x sin(x) + x^2 cos(x) D) 2x cos(x) - x^2 sin(x)
  Answer: C) 2x sin(x) + x^2 cos(x)
- Q: What is the slope of the tangent line to y = ln(x) at x = 1?
  Options: A) 0 B) 1 C) e D) undefined
  Answer: B) 1
- Q: Find the critical points of f(x) = x^3 - 6x^2 + 11x - 6.
  Options: A) x = 1, 2, 3 B) x = (6 +/- sqrt(3))/3 C) x = 2 only D) x = 3 +/- sqrt(2)
  Answer: B) x = (6 +/- sqrt(3))/3
