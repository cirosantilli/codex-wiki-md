<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the distinct [interpolation nodes](../../../../interpolation-node.md), define the [Lagrange cardinal polynomials](../../../../lagrange-cardinal-polynomial.md)

$$
L_i(x)=\prod_{\substack{0\leq j\leq n\\j\ne i}}
\frac{x-x_j}{x_i-x_j},\qquad i=0,\ldots,n.
$$

Every denominator is nonzero, each $L_i$ has [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$, and $L_i(x_j)=\delta_{ij}$. Hence the [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md)

$$
\boxed{p_n(x)=\sum_{i=0}^n f_iL_i(x)}
$$

belongs to $\Pi_n$ and has $p_n(x_j)=f_j$. This proves existence.

If $p_n$ and $\widetilde p_n$ both fit the data, their difference has [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$ but vanishes at the $n+1$ distinct [interpolation nodes](../../../../interpolation-node.md). Repeated application of the [factor theorem](../../../../factor-theorem.md) implies that $\prod_{j=0}^n(x-x_j)$ divides that difference. A nonzero [polynomial](../../../../polynomial-split.md) of degree at most $n$ cannot have such a divisor of degree $n+1$. Thus $p_n-\widetilde p_n=0$, proving uniqueness. When $n=0$, the empty product defining $L_0$ is $1$, so the argument includes the constant case.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
