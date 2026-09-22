<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [factor analysis](../../../../../../factor-analysis.md), the independent [multivariate normal distributions](../../../../../../multivariate-normal-distribution.md) of $Z_i$ and $\xi_i$ imply that their linear combination is also multivariate normal. Its [expected value](../../../../../../expected-value.md) is zero and its [covariance matrix](../../../../../../covariance-matrix.md) is

$$
\operatorname{Cov}(Y_i)=\Lambda\operatorname{Cov}(Z_i)\Lambda^T+\operatorname{Cov}(\xi_i)
=\Lambda\Lambda^T+\sigma^2I_p.
$$

Therefore

$$
\boxed{Y_i\sim N_p(0,\Lambda\Lambda^T+\sigma^2I_p),\quad i=1,\ldots,n,\text{ independently}.}
$$

The noise variance is assumed positive. The factor contribution is positive semidefinite and has rank at most $k$, while the noise makes the marginal covariance nonsingular.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
