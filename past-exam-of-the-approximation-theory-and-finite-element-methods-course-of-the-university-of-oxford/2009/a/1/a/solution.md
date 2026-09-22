<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [Lagrange cardinal polynomials](../../../../../lagrange-cardinal-polynomial.md)

$$
\ell_r(x)=\frac{\pi_{n,r}(x)}{\pi_{n,r}(x_r)}
=\prod_{s\ne r}\frac{x-x_s}{x_r-x_s}.
$$

Distinct nodes make every denominator nonzero. At $x_s$ these polynomials satisfy $\ell_r(x_s)=\delta_{rs}$, so the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) is

$$
\boxed{p_n(x)=\sum_{r=0}^nu_r\ell_r(x).}
$$

It has degree at most $n$ and takes the prescribed data values. If two such polynomials existed, their difference would have $n+1$ distinct roots but degree at most $n$, forcing that difference to be zero. This also proves uniqueness.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
