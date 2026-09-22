<h1 id="section-d/d12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [chi-squared test](../../../../../../chi-squared-test.md) compares discrepancies with their expected random size. For independent Gaussian observations with known [standard deviations](../../../../../../standard-deviation.md), a fitted model gives

$$
\chi^2=\sum_{i=1}^n\frac{[y_i-f(x_i;\widehat\theta)]^2}{\sigma_i^2}.
$$

Under a correct regular model with $p$ fitted parameters, its reference [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) are usually $\nu=n-p$. Correlated errors instead require $\chi^2=\mathbf r^TC^{-1}\mathbf r$ with the correct [covariance matrix](../../../../../../covariance-matrix.md). The reduced statistic has mean about one and [standard deviation](../../../../../../standard-deviation.md) $\sqrt{2/\nu}$, so it should not be forced to equal exactly one.

For binned counts, Pearson's statistic is $\sum_i(O_i-E_i)^2/E_i$. With a fixed total and $k$ populated categories, fitting $p$ distribution parameters generally gives $\nu=k-1-p$. The approximation needs adequately populated expected bins and the appropriate dependence assumptions. Sparse data may require a Poisson [likelihood](../../../../../../likelihood-function.md), exact calculation or simulated reference distribution rather than a casual chi-squared approximation.

The upper-tail [probability](../../../../../../probability.md) $p_{\rm value}=P(\chi^2_\nu\geq\chi^2_{\rm obs})$ measures how unusual the discrepancy would be under the null model; it is not the [probability](../../../../../../probability.md) that the model is true. A large statistic can indicate a wrong model, underestimated noise or unmodelled systematic effects; an unusually small one can indicate overestimated errors or correlations. Residual plots and checks of the noise model are needed alongside the numerical test.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
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
