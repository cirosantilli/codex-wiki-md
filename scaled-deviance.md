# Scaled deviance

↑ **Parent:** [Exponential-family deviance](exponential-family-deviance.md)

For an [exponential dispersion family](exponential-dispersion-model.md) with a common [dispersion parameter](dispersion-parameter.md) $\phi$, scaled deviance compares a fitted model with the [saturated statistical model](saturated-statistical-model.md) at the same dispersion:

$$
D^*=2\{\ell(\widetilde\theta;\phi)-\ell(\widehat\theta;\phi)\}=\frac D\phi,
\qquad
D=2\sum_i\{y_i(\widetilde\theta_i-\widehat\theta_i)-b(\widetilde\theta_i)+b(\widehat\theta_i)\}.
$$

For a [normal distribution](normal-distribution.md) with variance $\sigma^2$, unscaled [deviance](exponential-family-deviance.md) is the [residual sum of squares](residual-sum-of-squares.md) and scaled deviance is that sum divided by $\sigma^2$. For the [binomial distribution](binomial-distribution.md), $\phi=1$ and the two coincide. Unknown Gaussian dispersion requires variance estimation; raw deviance differences should not be treated as chi-squared statistics without the scale.

## ↑ Ancestors (8)

1. [Exponential-family deviance](exponential-family-deviance.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/3/i/solution.md)
