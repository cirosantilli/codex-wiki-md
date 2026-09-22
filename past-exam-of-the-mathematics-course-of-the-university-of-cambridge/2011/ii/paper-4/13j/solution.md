<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

For $\sigma^2>0$, the [Gaussian linear model](../../../../../normal-linear-model.md) has [likelihood function](../../../../../likelihood-function.md)

$$
L(\beta,\sigma^2;y)=(2\pi\sigma^2)^{-n/2}\exp\!\left[-\frac{(y-X\beta)^T(y-X\beta)}{2\sigma^2}\right].
$$

Maximizing over $\beta$ minimizes the residual sum of squares. Full column rank makes $X^TX$ positive definite, and differentiating gives the unique [least-squares estimator](../../../../../ordinary-least-squares-estimators.md)

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Put $P=X(X^TX)^{-1}X^T$ and $R=\|(I-P)Y\|^2$. If $R>0$, differentiating the profile log-likelihood in $\sigma^2$ gives

$$
\boxed{\widehat\sigma^2=R/n.}
$$

The denominator is $n$, not the residual degrees of freedom $n-p$; the latter gives the unbiased estimator.

A linear transformation of the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) remains normal, so

$$
\boxed{\widehat\beta\sim N_p(\beta,\sigma^2(X^TX)^{-1}).}
$$

Its [covariance](../../../../../covariance.md) with the residual vector is $\sigma^2(X^TX)^{-1}X^T(I-P)=0$. Jointly Gaussian vectors with zero cross-covariance are independent, hence $\widehat\beta$ is independent of $(I-P)Y$, and therefore of $\widehat\sigma^2$, a function of that residual. Orthogonal coordinates also give $R/\sigma^2\sim\chi^2_{n-p}$.

**The allowed boundary case $p=n$ needs qualification.** Then $P=I$, $R=0$ for every observation, and the likelihood increases without bound as $\sigma^2\downarrow0$ after fitting $Y$ exactly. There is no maximum in the positive-variance model; $R/n=0$ is only a formal boundary estimate. When $n>p$, $R>0$ almost surely under a genuinely positive [variance](../../../../../variance-split.md), and the displayed MLEs apply. A zero residual in any exceptional exact-fit sample has the same nonexistence issue. The estimator $\widehat\beta$ and its [normal distribution](../../../../../normal-distribution.md) remain well-defined in the square full-rank case.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
