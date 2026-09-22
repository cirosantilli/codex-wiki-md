<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write a nonterminating parity series as $y=x^r\sum_{j\geq0}b_jx^{2j}$, where $r=0$ or $1$. Its [recurrence relation](../../../../../recurrence-relation.md) is

$$
\frac{b_{j+1}}{b_j}=\frac{(2j+r)^2-m^2}{(2j+r+2)(2j+r+1)}.
$$

The [ratio test](../../../../../ratio-test.md) applied to its nonzero successive terms has limiting absolute ratio $|x|^2$. Hence the series converges absolutely for $|x|<1$ and diverges for $|x|>1$, with

$$
\boxed{R=1\quad\text{for every nonterminating parity series}.}
$$

At $x=\pm1$, the limiting ratio is one, so the basic [ratio test](../../../../../ratio-test.md) alone is inconclusive. Retain the next term of the ratio instead:

$$
\left|\frac{b_{j+1}}{b_j}\right|=1-\frac{3}{2j}+O(j^{-2}).
$$

For large $j$ the ratio is positive. Taking logarithms and summing gives $\log|b_j|=-\tfrac32\log j+O(1)$; the $O(j^{-2})$ remainders have a finite sum. Thus $|b_j|\leq Cj^{-3/2}$ eventually. Comparison with the convergent [p-series](../../../../../p-series.md) proves [absolute convergence](../../../../../absolute-convergence.md) at both endpoints as well:

$$
\boxed{\text{The nonpolynomial solutions' power series converge throughout }[-1,1].}
$$

The [radius of convergence](../../../../../radius-of-convergence.md) one is the distance from the expansion point to the nearest [singular points of a differential equation](../../../../../singular-point-of-a-differential-equation.md), $x=\pm1$. Convergence of function values at those points does not make the solutions analytic there; endpoint [derivatives](../../../../../derivative.md) can diverge. The terminating [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) is an exception with infinite [radius of convergence](../../../../../radius-of-convergence.md). For example, at $m=0$ the other solution is $\arcsin x$, whose endpoint values are finite while its first [derivative](../../../../../derivative.md) diverges.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
