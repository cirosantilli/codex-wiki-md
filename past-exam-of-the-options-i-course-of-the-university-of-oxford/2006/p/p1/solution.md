<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

The [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md) constructs existence explicitly:

$$
\ell_j(x)=\prod_{\substack{0\leq k\leq n\\k\ne j}}\frac{x-x_k}{x_j-x_k},\qquad p(x)=\sum_{j=0}^n f_j\ell_j(x).
$$

Distinct nodes make every denominator nonzero, and $\ell_j(x_k)=\delta_{jk}$, so $p(x_k)=f_k$ and $p$ has degree at most $n$. If two such [polynomials](../../../../polynomial-split.md) existed, their difference would have degree at most $n$ but at least $n+1$ distinct roots. The root bound for a nonzero [polynomial](../../../../polynomial-split.md) forces that difference to vanish. Thus **the interpolating [polynomial](../../../../polynomial-split.md) exists and is unique**.

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
