<h1 id="section-d/d12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [chi-squared test](../../../../../../chi-squared-test.md) compares residuals with the random scatter predicted by a model. For independent measurements $y_i$ with known Gaussian [standard deviations](../../../../../../standard-deviation.md) $\sigma_i$ and predictions $\mu_i(\theta)$, form

$$
Q=\sum_{i=1}^{N}\frac{[y_i-\mu_i(\widehat\theta)]^2}{\sigma_i^2}.
$$

If the mean model and error assumptions are correct, a full-rank linear fit of $p$ parameters gives a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $\nu=N-p$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). With a fully specified prediction and no fitted parameters, $\nu=N$. Nonlinear fits usually make this an approximation. Independent external calibration is not the same as fitting a parameter to these test data.

Under the reference distribution, the mean statistic is $\nu$ and its [variance](../../../../../../variance-split.md) is $2\nu$. The upper-tail [p-value](../../../../../../p-value.md) $\Pr(\chi_\nu^2\geq Q_{\mathrm{obs}})$ quantifies how unusual a discrepancy at least this large would be under the assumed model. A small value suggests model failure or incorrect uncertainties; it is not the [probability](../../../../../../probability.md) that the model is true. An unusually small statistic can also reveal inflated uncertainties or correlations. A rejection threshold should be specified in advance.

For independent [Poisson distribution](../../../../../../poisson-distribution.md) counts, the model [variance](../../../../../../variance-split.md) is its expected count $\mu_i$. The [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md) is $\sum(y_i-\mu_i)^2/\mu_i$. The estimated-error alternative $\sigma_i\simeq\sqrt{y_i}$ is common for large counts but can differ substantially when counts are small. In that regime the [Poisson deviance](../../../../../../poisson-deviance.md) or a direct [likelihood](../../../../../../likelihood-function.md) calculation is preferable, with simulation if an accurately calibrated goodness-of-fit [probability](../../../../../../probability.md) is required.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
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
