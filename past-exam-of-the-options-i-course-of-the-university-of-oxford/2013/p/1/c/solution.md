<h1 id="p/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrate the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) and exchange the [integral](../../../../../integral-split.md) with the finite sum:

$$
\int_a^bp(x)dx=\sum_{j=0}^nf(x_j)\int_a^b\ell_j(x)dx.
$$

Therefore the [interpolatory quadrature](../../../../../interpolatory-quadrature.md) weights are

$$
\boxed{w_j=\int_a^b\ell_j(x)dx=\int_a^b\prod_{k\ne j}\frac{x-x_k}{x_j-x_k}\,dx.}
$$

The resulting [quadrature rule](../../../../../quadrature-rule.md) is exact for every [polynomial](../../../../../polynomial-split.md) of degree at most $n$, since its interpolant is itself. For a general continuous $f$, replacing $f$ by its interpolant supplies the approximation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [P](../../../p.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
