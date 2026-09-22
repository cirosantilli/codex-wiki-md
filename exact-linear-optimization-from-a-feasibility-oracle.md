# Exact linear optimization from a feasibility oracle

↑ **Parent:** [Ellipsoid method](ellipsoid-method.md)

A [polynomial-time algorithm](polynomial-time-algorithm.md) for integer linear feasibility gives exact rational [linear programming](linear-programming.md) optimization. Rational vertex bounds give a polynomial-bit bound on every finite optimal value and its denominator. An objective threshold below that bound detects unboundedness after feasibility is established. Binary search with the additional inequality $c^Tx\leq t$ localizes the finite optimum to an interval containing a unique rational of bounded denominator; [continued fractions](continued-fraction.md) recover it exactly. A feasible optimizer can then be found by successive coordinate minimizations on a bounded optimal face. These produce faces of one fixed rational polytope, so one uniform vertex-denominator bound works throughout, avoiding exponential growth of precision requirements.

## ↑ Ancestors (6)

1. [Ellipsoid method](ellipsoid-method.md)
2. [Linear programming](linear-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/2/solution.md)
