# Binomial goodness-of-fit with an estimated parameter

↑ **Parent:** [Pearson chi-squared goodness-of-fit test](pearson-chi-squared-goodness-of-fit-test.md)

For $N$ independent groups each containing $m$ independent [Bernoulli trials](bernoulli-trial.md) with common probability $\theta$, the group count has a [binomial distribution](binomial-distribution.md). If $O_j$ groups have count $j$, the [maximum-likelihood estimate](maximum-likelihood-estimator.md) is $\widehat\theta=\sum_jjO_j/(mN)$. Form the [Pearson chi-squared statistic](pearson-chi-squared-statistic.md) using $E_j=N\binom mj\widehat\theta^j(1-\widehat\theta)^{m-j}$. With all $m+1$ categories retained, an interior true parameter, and sufficiently large expected counts, its null limit is a [chi-squared distribution](chi-squared-distribution.md) with $m-1$ [statistical degrees of freedom](statistical-degrees-of-freedom.md): one degree is removed by the fixed total and another by fitting $\theta$. Small expected counts require care with this approximation. If categories are pooled, the fitted parameter and calibration should correspond to the pooled statistical model; simply pooling a statistic after fitting the unpooled model does not automatically give the usual chi-squared limit.

## ↑ Ancestors (9)

1. [Pearson chi-squared goodness-of-fit test](pearson-chi-squared-goodness-of-fit-test.md)
2. [Pearson's chi-squared test](pearson-s-chi-squared-test.md)
3. [Statistical hypothesis test](statistical-hypothesis-test.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/8c/solution.md)
