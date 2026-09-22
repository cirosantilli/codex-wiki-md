<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the normalized [eigenfunctions](../../../../../eigenfunction.md) with the stated [weighted inner product](../../../../../weighted-inner-product.md). [Orthogonality](../../../../../orthogonal-vectors.md) gives $G[\hat y]=\sum_n|c_n|^2$. The corrected [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) and the vanishing boundary term give

$$
F[\hat y]=\int_a^b\overline{\hat y}\,\mathcal L\hat y\,dx=\sum_n\lambda_n|c_n|^2.
$$

For a complex trial the numerator means $\int(p|\hat y'|^2+q|\hat y|^2)dx$, agreeing with the given formula for real trials. Therefore

$$
\boxed{\Lambda[\hat y]=\frac{\sum_n\lambda_n|c_n|^2}{\sum_n|c_n|^2}\geq\lambda_0.}
$$

It is a [convex combination](../../../../../convex-combination.md) of the [eigenvalues](../../../../../eigenvalue.md), with equality only for a trial proportional to the lowest [eigenfunction](../../../../../eigenfunction.md). The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) consequently estimates $\lambda_0$ by choosing a nonzero admissible trial family and minimizing this quotient over its parameters:

$$
\boxed{\lambda_0\leq\min_{\text{trial parameters}}\Lambda[\hat y].}
$$

The result is an upper bound. A more flexible trial space can lower it, while equality requires that the exact lowest [eigenfunction](../../../../../eigenfunction.md) belong to the trial space. One need not know the expansion coefficients to calculate the quotient directly from the trial function.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
