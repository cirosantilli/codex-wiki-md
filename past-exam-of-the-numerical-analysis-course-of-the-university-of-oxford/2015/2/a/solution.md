<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [polynomial](../../../../polynomial-split.md) $p_n$ interpolates $f$ at the [interpolation nodes](../../../../interpolation-node.md) when

$$
p_n(x_i)=f(x_i)\qquad(0\leq i\leq n).
$$

For distinct [interpolation nodes](../../../../interpolation-node.md), define the [Lagrange cardinal polynomials](../../../../lagrange-cardinal-polynomial.md)

$$
\ell_i(x)=\prod_{j\ne i}\frac{x-x_j}{x_i-x_j}.
$$

The denominators are nonzero, each [polynomial degree](../../../../degree-of-a-polynomial.md) is at most $n$, and $\ell_i(x_j)=\delta_{ij}$, with $\delta_{ij}$ the [Kronecker delta](../../../../kronecker-delta.md). Therefore

$$
\boxed{p_n(x)=\sum_{i=0}^nf(x_i)\ell_i(x)}
$$

is a [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md) belonging to the [vector space of univariate polynomials](../../../../vector-space-of-univariate-polynomials.md) $\Pi_n$, and it has all the required sampled values.

If $r_n\in\Pi_n$ also works, $p_n-r_n$ has $n+1$ distinct [roots of a polynomial](../../../../root-of-a-polynomial.md) while its [polynomial degree](../../../../degree-of-a-polynomial.md) is at most $n$. The [root bound for a polynomial](../../../../lagrange-root-bound-over-a-field.md) forces it to be the [zero polynomial](../../../../zero-polynomial.md), proving uniqueness. The phrase “degree $n$” denotes the allowed maximum; the actual [polynomial degree](../../../../degree-of-a-polynomial.md) may be smaller. No [continuity](../../../../continuous-function.md) assumption is needed merely to construct the [interpolation polynomial](../../../../interpolation-polynomial.md) from these finitely many values.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
