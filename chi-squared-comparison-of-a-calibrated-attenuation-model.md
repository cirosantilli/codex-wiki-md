# Chi-squared comparison of a calibrated attenuation model

↑ **Parent:** [Chi-squared test](chi-squared-test.md)

Suppose $N_0$ is independently calibrated and counts $y_i$ have predicted means $\mu_i=t_iN_0e^{-bn_i}$ under a specified candidate $b$. For independent sufficiently large Poisson counts, the [Pearson chi-squared statistic](pearson-chi-squared-statistic.md) is $Q=\sum_i(y_i-\mu_i)^2/\mu_i$. With no parameters fitted to these test counts, its approximate reference [chi-squared distribution](chi-squared-distribution.md) has one degree of freedom per observation. Fitting a continuous $b$ to the same data instead removes one residual degree of freedom. Replacing the denominators by observed counts is a common estimated-error approximation but can behave badly at small counts.

Calibration uncertainty $\sigma_0$ also induces correlated prediction errors. First-order [propagation of uncertainty](propagation-of-uncertainty.md) gives

$$
\operatorname{Cov}(y_i-\mu_i,y_j-\mu_j)\simeq\delta_{ij}\mu_i+t_it_j e^{-b(n_i+n_j)}\sigma_0^2.
$$

A generalized quadratic form uses this [covariance matrix](covariance-matrix.md). For sparse counts use the [Poisson deviance](poisson-deviance.md) or the full count likelihood, with simulation if a calibrated goodness-of-fit probability is required. Choosing a range after inspecting residuals also affects formal test calibration; a physically specified signal-dominated range is preferable when applying a pure attenuation model.

## ↑ Ancestors (6)

1. [Chi-squared test](chi-squared-test.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-d/d12/d/solution.md)
