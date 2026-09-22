<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The plug-in estimate is

$$
\boxed{\widehat\theta=\widehat\beta_1\widehat\beta_2.}
$$

For a concrete [bootstrap](../../../../../../bootstrapping-statistics.md) construction, suppose the rows $(x_i,y_i)$ are [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md), $\mathbb E(e_i\mid x_i)=0$, the design moment matrix is nonsingular, and the required moments exist. Use a [paired bootstrap](../../../../../../paired-bootstrap.md): sample $n$ rows with replacement, form $X^*,Y^*$, refit by [ordinary least squares](../../../../../../ordinary-least-squares.md), and compute $\widehat\theta^*=\widehat\beta_1^*\widehat\beta_2^*$. Repeat many times. Singular resampled designs require a suitable rank-preserving implementation or replacement replicate; with a regular continuous design their frequency vanishes asymptotically.

The [bootstrap-t confidence interval](../../../../../../bootstrap-t-confidence-interval.md) method also needs a [standard error](../../../../../../standard-error.md) in the original sample and every replicate. One asymptotically valid heteroscedasticity-robust [covariance](../../../../../../covariance.md) estimate is

$$
\widehat V=(X^\top X)^{-1}\left(\sum_i x_ix_i^\top\widehat e_i^2\right)(X^\top X)^{-1}.
$$

The [delta method](../../../../../../delta-method.md) for the coefficient product gives

$$
d=(\widehat\beta_2,\widehat\beta_1)^\top,\qquad
\boxed{\widehat s=(d^\top\widehat Vd)^{1/2}.}
$$

Recompute $\widehat V^*,d^*,\widehat s^*$ in each paired replicate. This is [bootstrap inference for a product of regression coefficients](../../../../../../bootstrap-inference-for-a-product-of-regression-coefficients.md).

With fixed rather than random design, resample centered residuals if errors are identically distributed with [homoskedasticity](../../../../../../homoskedasticity.md), or use a properly specified [wild bootstrap](../../../../../../wild-bootstrap.md) for heteroscedastic errors, keeping $X$ fixed and refitting after generating $Y^*$. The printed assumption $\mathbb E e_i=0$ alone does not establish [independent](../../../../../../independent-random-variables.md) observations or validity of a [bootstrap confidence interval](../../../../../../bootstrap-confidence-interval.md). The formulas below give asymptotic 95% coverage under the stated regularity conditions, not an exact finite-sample guarantee. In particular the ordinary first-order studentization needs $(\beta_1,\beta_2)\ne(0,0)$ and a nonzero asymptotic [variance](../../../../../../variance-split.md); when both coefficients vanish the product has nonstandard behavior.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
