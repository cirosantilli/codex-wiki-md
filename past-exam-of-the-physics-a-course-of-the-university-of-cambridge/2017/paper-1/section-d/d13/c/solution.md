<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Gaussian distribution](../../../../../../normal-distribution.md) with mean $\mu$ and [standard deviation](../../../../../../standard-deviation.md) $\sigma$ has [probability density](../../../../../../probability-density.md)

$$
\boxed{p(x)=\frac1{\sqrt{2\pi}\sigma}
\exp\!\left[-\frac{(x-\mu)^2}{2\sigma^2}\right].}
$$

Its symmetry, finite [variance](../../../../../../variance-split.md) and simple behavior under linear combinations make it useful for repeated measurements. Roughly $68.3\%$, $95.4\%$ and $99.7\%$ of observations lie within one, two and three true standard deviations of the mean. These are coverage probabilities for a specified distribution, not guarantees that every experimental error is normal.

**Why it appears.** The [central limit theorem](../../../../../../central-limit-theorem.md) explains why many sums of small independent finite-variance contributions approach a Gaussian law after centering and scaling, provided no single contribution dominates. Detector [noise](../../../../../../noise-signal-processing.md), small mechanical disturbances and multiple electronic fluctuations can combine approximately this way. The theorem does not remove a common calibration bias, and it does not justify assuming normal tails for rare large disturbances or arbitrarily correlated errors. A large-mean [Poisson distribution](../../../../../../poisson-distribution.md) also approaches a Gaussian with [variance](../../../../../../variance-split.md) equal to its mean, making normal approximations useful for high-count photon or particle data; low counts require the discrete model.

A classical particle at thermal equilibrium in a one-dimensional [harmonic potential](../../../../../../harmonic-potential.md) has a Gaussian [position](../../../../../../position.md) distribution directly from the [Boltzmann distribution](../../../../../../boltzmann-distribution.md):

$$
p(x)\propto e^{-kx^2/(2k_BT)},\qquad
\langle x^2\rangle=\frac{k_BT}{k}.
$$

Thus a Gaussian law can arise from the [energy](../../../../../../energy-split.md) dependence of equilibrium [probability](../../../../../../probability.md), rather than only from an informal appeal to many independent errors.

**Precision of repeated measurements.** For $N$ independent observations with the same mean and [variance](../../../../../../variance-split.md), the [sample mean](../../../../../../sample-mean.md) has [variance](../../../../../../variance-split.md) $\sigma^2/N$. For Gaussian observations this mean is exactly Gaussian:

$$
\boxed{\sigma_{\overline x}=\frac\sigma{\sqrt N}.}
$$

Consequently quadrupling the number of independent readings halves the random [standard error](../../../../../../standard-error.md). When the true [variance](../../../../../../variance-split.md) is unknown, a small-sample [confidence interval](../../../../../../confidence-interval.md) for a normal mean uses a [Student t-distribution](../../../../../../student-s-t-distribution.md) with $N-1$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md); replacing that by a normal quantile can overstate precision. Shared [systematic errors](../../../../../../systematic-error.md) and correlations do not decrease by the same averaging rule.

**Combining results and fitting models.** Independent Gaussian estimates $x_i$ of one quantity, with known [variances](../../../../../../variance-split.md) $\sigma_i^2$, combine through the inverse-variance weighted mean

$$
\widehat\mu=\frac{\sum_i x_i/\sigma_i^2}{\sum_i1/\sigma_i^2},\qquad
\operatorname{Var}(\widehat\mu)=\frac1{\sum_i1/\sigma_i^2}.
$$

For a model $y_i=g_i(\theta)+\epsilon_i$ with independent zero-mean [Gaussian noise](../../../../../../gaussian-noise.md), maximizing the [likelihood](../../../../../../likelihood-function.md) is equivalent to minimizing the weighted least-squares statistic

$$
\chi^2(\theta)=\sum_i\frac{[y_i-g_i(\theta)]^2}{\sigma_i^2}.
$$

For a correct linear model with known independent Gaussian errors and $p$ fitted parameters of full rank, the minimized statistic has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $N-p$ degrees of freedom. Nonlinear fits only inherit that familiar approximation under additional regularity and adequate-data assumptions. Known correlated Gaussian errors require the full inverse [covariance matrix](../../../../../../covariance-matrix.md) in the quadratic form.

These properties support [confidence intervals](../../../../../../confidence-interval.md), consistency checks, calibration and error propagation. They also give practical diagnostics: inspect residuals for trends, changing spread, correlations or outliers before trusting a Gaussian fit. **Gaussian models connect physical fluctuations to quantitative uncertainty, but their assumptions must be checked rather than inferred from the shape of a convenient bell curve.**

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
