<h1 id="6/viii/solution">Solution</h1>

↑ **Parent:** [Viii](../viii.md)

For a regular iid model with a fixed-dimensional interior parameter $\theta_0$, identifiability, sufficient differentiability and moment domination, and nonsingular per-observation [Fisher information](../../../../../../fisher-information-matrix.md) $I(\theta_0)$, a consistent [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) solves the [score equation](../../../../../../score-equation.md). Expanding it gives

$$
\sqrt n(\widehat\theta-\theta_0)=I(\theta_0)^{-1}\frac1{\sqrt n}\sum_i s_{\theta_0}(Y_i)+o_p(1)
\Rightarrow N_p(0,I(\theta_0)^{-1}),
$$

where $s_\theta=\partial_\theta\log f_\theta$. The score has mean zero and [covariance](../../../../../../covariance.md) $I$ under the regularity assumptions. This proves the usual large-sample information bound and asymptotic efficiency within regular parametric inference. The observed curvature $j(\widehat\theta)/n$ and the empirical score [covariance](../../../../../../covariance.md) consistently estimate $I$ when the model is correctly specified.

For $r$ smooth constraints $h(\theta)=0$ with full-row-rank derivative $H$, the [Wald test](../../../../../../wald-test.md) uses

$$
W=n\,h(\widehat\theta)^T[H I^{-1}H^T]^{-1}h(\widehat\theta)\Rightarrow\chi_r^2.
$$

The [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) and [score test](../../../../../../score-test.md), evaluated using the constrained fit and nuisance-adjusted efficient information, have the same first-order chi-square law. A quadratic local [likelihood](../../../../../../likelihood-function.md) expansion explains their asymptotic equivalence. [Profile likelihood](../../../../../../profile-likelihood.md) supplies inference about a parameter of interest with fitted [nuisance parameters](../../../../../../nuisance-parameter.md), and the corresponding chi-square cutoffs give approximate confidence regions.

These conclusions depend on the stated regularity: parameters at a boundary, nonidentifiability, singular information, changing dimension, or parameter-dependent support can give different rates and limits. Under misspecification, the fitted parameter generally approaches a pseudo-true value and its [variance](../../../../../../variance-split.md) is a [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md), not simply inverse [Fisher information](../../../../../../fisher-information-matrix.md).

## ↑ Ancestors (11)

1. [Viii](../viii.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
