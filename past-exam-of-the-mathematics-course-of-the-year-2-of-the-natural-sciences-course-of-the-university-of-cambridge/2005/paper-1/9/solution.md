<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Introduce a [Lagrange multiplier](../../../../lagrange-multiplier.md) for the normalization and vary $J[y]=\int_0^1[p(y')^2+qy^2-\lambda wy^2]dx$. With variation $\eta$ satisfying $\eta(1)=0$, [integration by parts](../../../../integration-by-parts.md) gives

$$
\delta J=2[py'\eta]_0^1-2\int_0^1[(py')'-qy+\lambda wy]\eta\,dx.
$$

The upper endpoint term vanishes, and the lower term vanishes because $p(0)=0$ with the stipulated regular differentiable behavior. More generally the natural endpoint condition is $py'\to0$ there. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives $(py')'-qy+\lambda wy=0$, the stated [Sturm-Liouville problem](../../../../sturm-liouville-problem.md).

The [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md) estimates the lowest eigenvalue by minimizing $R[y]=\int[p(y')^2+qy^2]dx/\int wy^2dx$ over an admissible finite-dimensional trial family. Restricting the family can only raise the minimum.

For the specific radial problem, $p=w=x$ and $q=0$. The trial $y=A(1-x^2)$ has $\int_0^1xy^2dx=A^2/6$. Normalization gives $\boxed{A=\sqrt6}$, with the negative sign an equivalent choice. The numerator is $\int_0^1x(2Ax)^2dx=A^2$, so

$$
\boxed{\lambda_1\leq R[y]=6.}
$$

This is the quadratic case of the [power-law variational bound for a circular membrane](../../../../power-law-variational-bound-for-a-circular-membrane.md). The exact first eigenvalue $5.7815$ is smaller because the polynomial trial is not the exact [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md) eigenfunction. Expanding a trial in the exact [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) expresses its [Rayleigh quotient](../../../../rayleigh-quotient.md) as a weighted average of eigenvalues, so no admissible trial can lie below the lowest one.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
