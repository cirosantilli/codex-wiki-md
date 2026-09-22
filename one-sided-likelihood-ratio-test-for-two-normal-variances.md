# One-sided likelihood-ratio test for two normal variances

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For independent samples from [normal distributions](normal-distribution.md) with separate unknown means, test equal variances against $\sigma_X^2>\sigma_Y^2$. Profiling the means gives sample means. Under the null the variance maximum is $(S_X+S_Y)/(n_X+n_Y)$; the separate maxima are $S_X/n_X$ and $S_Y/n_Y$. If the latter obey the proposed order, their likelihood quotient is

$$
\Lambda=\frac{(S_X/n_X)^{n_X/2}(S_Y/n_Y)^{n_Y/2}}{[(S_X+S_Y)/(n_X+n_Y)]^{(n_X+n_Y)/2}}.
$$

It decreases strictly as $(S_X/n_X)/(S_Y/n_Y)>1$ increases. Otherwise the ordered alternative maximum lies on the equal-variance boundary and the quotient is one. Under the null, [Cochran's theorem](cochran-s-theorem.md) gives independent chi-squared residual sums with degrees $n_X-1,n_Y-1$, so rejection is in the upper tail of the displayed [F-distribution](f-distribution.md) statistic, calibrated at the desired significance level.

## ↑ Ancestors (8)

1. [Likelihood-ratio test](likelihood-ratio-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/12h/solution.md)
