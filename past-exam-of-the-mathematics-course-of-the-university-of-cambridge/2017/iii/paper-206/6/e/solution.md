<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $X$ have rows $(1,y_i)$ and let $\Sigma_\vartheta$ be the spatial [covariance matrix](../../../../../../covariance-matrix.md) with $\vartheta=(\tau^2,\sigma^2,a)$. Conditional on chosen [covariance](../../../../../../covariance.md) parameters, the [best linear unbiased estimator](../../../../../../best-linear-unbiased-estimator.md) of the drift coefficients is the [generalized least squares](../../../../../../generalized-least-squares.md) estimator

$$
\boxed{\widehat\beta(\vartheta)=(X^T\Sigma_\vartheta^{-1}X)^{-1}X^T\Sigma_\vartheta^{-1}z.}
$$

The printed procedure first estimates the linear drift from `depth ~ y`, constructs a binned residual [empirical semivariogram](../../../../../../empirical-semivariogram.md), fits a Gaussian [semivariogram](../../../../../../semivariogram.md) to it, and then uses the fitted [covariance](../../../../../../covariance.md) in [generalized least squares](../../../../../../generalized-least-squares.md) trend estimation and [universal kriging](../../../../../../universal-kriging.md). The missing fit could be supplied as
```
gauss.model2 <- fit.variogram(smvg2, vgm(0.5, "Gau", 1, 0))
```
where those arguments are initial values, not the reported final estimates. Such [semivariogram](../../../../../../semivariogram.md) fitting typically minimizes a weighted sum of squared discrepancies between binned empirical values and model values; it is not automatically a joint Gaussian likelihood maximization. One can iterate: form residuals using the current drift, refit the [covariance](../../../../../../covariance.md) model, recompute the [generalized least squares](../../../../../../generalized-least-squares.md) drift, and repeat until changes are small. The displayed commands themselves show a single sequence, not evidence that such iteration occurred.

A likelihood-based alternative estimates the two blocks coherently from

$$
\ell(\beta,\vartheta)=-\frac12\{n\log(2\pi)+\log\det\Sigma_\vartheta+(z-X\beta)^T\Sigma_\vartheta^{-1}(z-X\beta)\}.
$$

Substitute $\widehat\beta(\vartheta)$ to obtain a profile [log-likelihood](../../../../../../log-likelihood.md), maximize over $\tau^2,\sigma^2\ge0$ and $a>0$ with a [positive-definite matrix](../../../../../../positive-definite-matrix.md) $\Sigma_\vartheta$, and recover the drift coefficients from the optimizing [covariance](../../../../../../covariance.md). [Restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md) adds the design determinant term $\log\det(X^T\Sigma_\vartheta^{-1}X)$ and uses $n-2$ in place of $n$ in the normalizing term, up to a fixed-design constant. It can reduce [bias](../../../../../../bias-of-an-estimator.md) from estimating the drift before the [covariance](../../../../../../covariance.md). A zero fitted nugget is a legitimate boundary estimate, not proof that measurement error is absent. **Estimate drift using covariance-weighted regression, and spatial dependence from drift-adjusted variation, with the two stages or likelihood explicitly distinguished.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
