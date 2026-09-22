<h1 id="p/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

As explained by [admissible polynomials for a singular inverse-linear weight](../../../../../admissible-polynomials-for-a-singular-inverse-linear-weight.md), there is a domain issue: the constant [polynomial](../../../../../polynomial-split.md) does not belong to the weighted space, because $\int_0^1x^{-1}dx=\infty$. Hence the full space $\Pi_{n-1}$ is not a subspace of $V$, and the preceding inner-product projection theorem cannot be applied to it as stated.

Nevertheless a meaningful finite-error [best approximation](../../../../../best-approximation-in-a-normed-space.md) does exist after restricting to admissible [polynomials](../../../../../polynomial-split.md). The target $x^n$ lies in $V$ for every $n\ge1$, since its squared integrand near zero is $x^{2n-1}$. A [polynomial](../../../../../polynomial-split.md) $p\in\Pi_{n-1}$ has finite error exactly when $p(0)=0$: otherwise the residual tends to a nonzero constant and its weighted squared integral diverges; if $p(0)=0$, it has at least a simple zero and is [integrable](../../../../../integrability.md) in the required norm. Thus the admissible approximation space is

$$
\boxed{\Pi_{n-1}\cap V=\operatorname{span}\{x,x^2,\ldots,x^{n-1}\}.}
$$

For $n=1$ it is $\{0\}$, giving [best approximation](../../../../../best-approximation-in-a-normed-space.md) zero. For $n\ge2$ it is a finite-dimensional inner-product subspace with positive definite [Gram matrix](../../../../../gram-matrix.md), so it has a unique [orthogonal projection](../../../../../orthogonal-projection.md) of $x^n$. Therefore **the full [polynomial](../../../../../polynomial-split.md)-space formulation is not defined inside $V$, but the finite-error interpretation has a unique [best approximation](../../../../../best-approximation-in-a-normed-space.md)**. Declaring that no [best approximation](../../../../../best-approximation-in-a-normed-space.md) can exist under any interpretation would miss this admissible subspace.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [P](../../../p.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
