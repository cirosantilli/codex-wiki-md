<h1 id="section-d/d12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For independent Gaussian measurements with correctly specified [standard deviations](../../../../../../standard-deviation.md), model residuals give the [chi-squared test](../../../../../../chi-squared-test.md) statistic

$$
X^2=\sum_{i=1}^n\frac{[y_i-f_i(\widehat\theta)]^2}{\sigma_i^2}.
$$

For a linear fit of $p$ identifiable parameters under the null model, it has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $\nu=n-p$ [degrees of freedom](../../../../../../degree-of-freedom.md). The upper-tail [p-value](../../../../../../p-value.md) $P(\chi_\nu^2\geq X_{\rm obs}^2)$ tests unusually large residuals; a nonlinear fit generally uses this distribution only approximately. Correlated Gaussian errors instead require $X^2=\mathbf r^{\mathsf T}\Sigma^{-1}\mathbf r$.

For counts, [Pearson's chi-squared test](../../../../../../pearson-s-chi-squared-test.md) uses $X^2=\sum_j(O_j-E_j)^2/E_j$, with $E_j$ calculated under the [null hypothesis](../../../../../../null-hypothesis.md). For $k$ multinomial categories and $p$ fitted parameters the usual asymptotic [degrees of freedom](../../../../../../degree-of-freedom.md) are $k-1-p$; the subtraction of one reflects the fixed total count. Sparse expected counts can invalidate this approximation, requiring a suitable exact or simulation-based test. Contingency-table independence gives $(r-1)(c-1)$ [degrees of freedom](../../../../../../degree-of-freedom.md).

**A small [p-value](../../../../../../p-value.md) indicates tension with the specified model and error assumptions; it is not the [probability](../../../../../../probability.md) that the null is true.** Excessive $X^2$ may reflect a wrong model, underestimated errors, correlations or outliers. An implausibly small value may suggest overestimated errors or hidden constraints. For an adequate fitted model $X^2/\nu$ is typically near one, with fluctuations, rather than required to equal one.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2010](../../../../split.md)
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
