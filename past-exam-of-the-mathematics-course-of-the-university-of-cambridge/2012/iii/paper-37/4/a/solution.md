<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Poisson regression](../../../../../../poisson-regression.md), the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta)=\sum_{i=1}^n\left[Y_ix_i^T\beta-e^{x_i^T\beta}-\log(Y_i!)\right].
$$

Since $\mu_i=e^{x_i^T\beta}$, the [score function](../../../../../../informant-function.md) and its derivative are

$$
U(\beta)=\sum_i x_i(Y_i-\mu_i)=X^T(Y-\mu),\qquad
\frac{\partial U}{\partial\beta^T}=-X^TWX,\quad W=\operatorname{diag}(\mu_i).
$$

Consequently a finite [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) satisfies

$$
\boxed{X^T(Y-\widehat\mu)=0,\qquad\widehat\mu_i=e^{x_i^T\widehat\beta}.}
$$

These nonlinear equations are normally solved by [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). If $X$ has full column rank, the Hessian is negative definite and any finite solution is the unique maximizer. Full rank does not by itself rule out a boundary solution at infinite coefficients for every conceivable data set. The Poisson [generalized linear model](../../../../../../generalized-linear-model.md) has dispersion one, so there is no separate scale parameter in this likelihood.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
