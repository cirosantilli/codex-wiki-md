<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each [interpolation node](../../../../interpolation-node.md) define the [Lagrange cardinal polynomial](../../../../lagrange-cardinal-polynomial.md)

$$
\ell_j(x)=\prod_{\substack{0\leq k\leq n\\k\ne j}}\frac{x-x_k}{x_j-x_k},\qquad 0\leq j\leq n.
$$

All denominators are nonzero because the [interpolation nodes](../../../../interpolation-node.md) are distinct. Each [polynomial](../../../../polynomial-split.md) has [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$, and $\ell_j(x_i)=\delta_{ij}$, where $\delta_{ij}$ is the [Kronecker delta](../../../../kronecker-delta.md). Consequently the [linear combination](../../../../linear-combination.md)

$$
p_n(x)=\sum_{j=0}^n f_j\ell_j(x)
$$

belongs to the [vector space of univariate polynomials](../../../../vector-space-of-univariate-polynomials.md) $\Pi_n$ and has the required values. This proves existence of the [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md).

For uniqueness, suppose $p_n$ and $r_n$ both work. Their difference is a [polynomial](../../../../polynomial-split.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$ with $n+1$ distinct [roots of a polynomial](../../../../root-of-a-polynomial.md). The [root bound for a polynomial](../../../../lagrange-root-bound-over-a-field.md) forces $p_n-r_n$ to be the [zero polynomial](../../../../zero-polynomial.md).

The seven supplied values follow $f_i=i^2+1$. The [quadratic polynomial](../../../../quadratic-polynomial.md) $x^2+1$ belongs to $\Pi_6$ and takes all seven values, so uniqueness gives

$$
\boxed{p_6(x)=x^2+1.}
$$

The subscript bounds the [polynomial degree](../../../../degree-of-a-polynomial.md); it does not require [polynomial degree](../../../../degree-of-a-polynomial.md) exactly six.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
