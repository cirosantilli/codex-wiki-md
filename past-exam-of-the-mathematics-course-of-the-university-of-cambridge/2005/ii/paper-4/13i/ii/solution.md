<h1 id="13i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $t_i=\beta^Tx_i=1/\mu_i>0$. Up to constants independent of $\beta$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta)=\nu\sum_i[\log t_i-Y_it_i].
$$

The [score function](../../../../../../informant-function.md) and its [derivative](../../../../../../derivative.md) are

$$
U(\beta)=\nu\sum_i x_i(\mu_i-Y_i),\qquad
\ell''(\beta)=-\nu\sum_i\mu_i^2x_ix_i^T.
$$

Thus an interior [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) solves

$$
\boxed{\sum_i x_i[(\widehat\beta^Tx_i)^{-1}-Y_i]=0}.
$$

For a full-rank design the Hessian is negative definite on the parameter region, so there is at most one interior solution and it is the maximum. A [Newton method](../../../../../../newton-s-method-in-optimization.md), also [Fisher scoring](../../../../../../scoring-algorithm.md) here because the observed Hessian equals its expectation, is

$$
\beta_{\rm new}=\beta+
\left(\sum_i\mu_i^2x_ix_i^T\right)^{-1}\sum_i x_i(\mu_i-Y_i).
$$

Recompute the means at every step and use a line search if necessary to keep all $t_i>0$ and increase the [log-likelihood](../../../../../../log-likelihood.md). Existence, [identifiability](../../../../../../identifiability.md) and nonsingularity are regularity conditions, not consequences of the density alone.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13I](../../13i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
