# Root selection by bisection with multiple roots in the initial bracket

↑ **Parent:** [Bisection method](bisection-method.md)

The [bisection method](bisection-method.md) preserves some root in a sign-changing bracket but does not select a fixed root when several are present. For the displayed [polynomial](polynomial-split.md), endpoint and midpoint roots are returned immediately. If $2<b<3$, the first midpoint lies in $(1/2,1)$ with negative function value, so the retained bracket contains only zero. If $b=3$, the first midpoint is exactly one. If $3<b\leq4$, that midpoint lies in $(1,3/2]$ with positive function value, so the retained bracket contains only two. At $b=2$ the right endpoint itself is the root two.

Thus arbitrarily small changes of the initial endpoint across $b=3$ change the limiting root from zero to two, with one selected exactly at the transition. The guarantee concerns distance to a root inside the retained interval, rather than continuous dependence of that root's identity on the starting data.

## ↑ Ancestors (7)

1. [Bisection method](bisection-method.md)
2. [Bracketing method](bracketing-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/u/1/c/solution.md)
