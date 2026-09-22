<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

The [ordinary least squares](../../../../../ordinary-least-squares.md) estimate, which is also the [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) in this [normal linear model](../../../../../normal-linear-model.md), gives the [hat matrix](../../../../../hat-matrix.md)

$$
\boxed{P=X(X^TX)^{-1}X^T.}
$$

It is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the column space of $X$, so $P^T=P$, $P^2=P$ and $\operatorname{rank}P=p$. Since $(I-P)X=0$, the vector of [regression residuals](../../../../../regression-residual.md) is $\widehat\epsilon=(I-P)\epsilon$, with [multivariate normal distribution](../../../../../multivariate-normal-distribution.md)

$$
\boxed{\widehat\epsilon\sim N_n\bigl(0,\sigma^2(I-P)\bigr).}
$$

For $i\ne j$, its [covariance](../../../../../covariance.md) is $-\sigma^2p_{ij}$, which is generally nonzero. Therefore the [regression residuals](../../../../../regression-residual.md) are generally dependent, even though the original errors are [independent random variables](../../../../../independent-random-variables.md).

Fit the model in R, compute its [internally studentized residuals](../../../../../standardized-regression-residual.md) with `rstandard(fit)`, and examine a [normal Q-Q plot](../../../../../normal-q-q-plot.md) with `qqnorm(rstandard(fit))` and `qqline(rstandard(fit))`. A plot of these [regression residuals](../../../../../regression-residual.md) against the [fitted values](../../../../../fitted-values.md) helps detect a curved mean pattern or nonconstant [variance](../../../../../variance-split.md). Approximate agreement with a straight line in the [Q-Q plot](../../../../../q-q-plot.md), with no systematic residual pattern, supports the assumed error model.

Here $p\ll n$. The average [leverage](../../../../../regression-leverage.md) is $\operatorname{tr}P/n=p/n$, and $\sum_{ij}p_{ij}^2=\operatorname{tr}(P^2)=p$. Thus most diagonal corrections and most off-diagonal dependences are small when only a few directions have been removed from a large sample. Also $\widetilde\sigma^2$ estimates $\sigma^2$ accurately when $n-p$ is large. These facts make the visual independent-normal approximation reasonable, though exceptional high-[leverage](../../../../../regression-leverage.md) observations still deserve attention.

The approximation is not an exact distributional statement: the [distribution of an internally studentized Gaussian residual](../../../../../distribution-of-an-internally-studentized-gaussian-residual.md) has $\widehat\eta_i^2/(n-p)\sim\operatorname{Beta}(1/2,(n-p-1)/2)$ when $n-p\geq2$ and $p_{ii}<1$. In particular these residuals are bounded, rather than exactly distributed according to [Student's t-distribution](../../../../../student-s-t-distribution.md). Formal goodness-of-fit calibration should account for fitting and dependence.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
