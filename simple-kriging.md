# Simple kriging

↑ **Parent:** [Kriging](kriging.md)

[Simple kriging](simple-kriging.md) assumes a known [mean](expected-value-split.md) function. If $m=(m(s_1),\ldots,m(s_n))^T$ and $m_0=m(s_0)$ are known, center the observations, predict the residual, and add back the target [mean](expected-value-split.md):

$$
\widehat Z_0=m_0+c^T\Sigma^{-1}(z-m),\qquad
s_{\mathrm{SK}}^2=v_0-c^T\Sigma^{-1}c.
$$

For known zero [mean](expected-value-split.md), these reduce to $c^T\Sigma^{-1}z$ and $v_0-c^T\Sigma^{-1}c$. Completing the [covariance](covariance.md) [quadratic form](quadratic-form-split.md) gives

$$
v_0-2w^Tc+w^T\Sigma w
=s_{\mathrm{SK}}^2+(w-\Sigma^{-1}c)^T\Sigma(w-\Sigma^{-1}c),
$$

which proves minimum error [variance](variance-split.md) among predictors of the form $m_0+w^T(Z-m)$. No sum-to-one constraint is needed: the known [mean](expected-value-split.md) already supplies the offset. In the exponential example from [ordinary kriging](ordinary-kriging.md), imposing known zero [mean](expected-value-split.md) gives weights $(0,2/5,2/5)^T$, prediction $2$, and error [variance](variance-split.md) $3/5$. The smaller error [variance](variance-split.md) uses additional knowledge of the [mean](expected-value-split.md); it is not a free improvement when the [mean](expected-value-split.md) is unknown.

If $(Z_0,Z)$ has a joint [multivariate normal distribution](multivariate-normal-distribution.md), the displayed prediction is exactly $\mathbb E[Z_0\mid Z=z]$, and $s_{\mathrm{SK}}^2$ is its conditional [variance](variance-split.md). A [conditional expectation](conditional-expectation.md) minimizes [mean squared error](mean-squared-error.md) among all square-integrable functions of the observations. Without a joint [multivariate normal distribution](multivariate-normal-distribution.md), [simple kriging](simple-kriging.md) remains the best predictor in the specified affine class, but the [conditional expectation](conditional-expectation.md) may be nonlinear and its conditional [variance](variance-split.md) may depend on $z$. Thus [Gaussian process regression](gaussian-process-regression.md) and the second-moment [kriging](kriging.md) construction agree under these assumptions, while having different starting points.[chapter 2, equations (2.23)–(2.24) and (2.38)](gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams.md)

## ↑ Ancestors (8)

1. [Kriging](kriging.md)
2. [Geostatistics](geostatistics.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Kriging](kriging.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/b/solution.md)
- [Simple kriging](simple-kriging.md)
- [Universal kriging](universal-kriging.md)
