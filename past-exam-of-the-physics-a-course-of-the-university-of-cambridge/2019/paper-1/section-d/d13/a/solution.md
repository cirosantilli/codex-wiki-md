<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [chi-squared test](../../../../../../chi-squared-test.md) compares squared deviations with the size expected from the assumed random errors. For independent observations with a [normal distribution](../../../../../../normal-distribution.md) $y_i$ with known [standard deviations](../../../../../../standard-deviation.md) $\sigma_i$ and predictions $\mu_i(\theta)$, use

$$
Q=\sum_{i=1}^{N}\frac{[y_i-\mu_i(\widehat\theta)]^2}{\sigma_i^2}.
$$

For a correct fixed model, the standardized independent residuals are unit-variance [normal distributions](../../../../../../normal-distribution.md), so $Q$ has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $\nu=N$. Fitting $p$ independent linear parameters removes $p$ residual directions, giving $\nu=N-p$. This distribution is exact for a full-rank linear model with known errors with a [normal distribution](../../../../../../normal-distribution.md); it is an approximation for many nonlinear fits. With known correlated errors with a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), replace the sum by $Q=\mathbf r^{\mathsf T}\Sigma^{-1}\mathbf r$, where $\Sigma$ is the [covariance matrix](../../../../../../covariance-matrix.md) and its rank and fitted constraints determine the available [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md).

Under the [null hypothesis](../../../../../../null-hypothesis.md), $\mathbb E Q=\nu$ and $\operatorname{Var}Q=2\nu$. The reduced statistic $Q/\nu$ should therefore be near one, with [standard deviation](../../../../../../standard-deviation.md) $\sqrt{2/\nu}$, rather than equal to one exactly. An upper-tail [p-value](../../../../../../p-value.md) is

$$
\boxed{p=\Pr(\chi_\nu^2\geq Q_{\mathrm{obs}}).}
$$

Compare it with a significance threshold chosen in advance. A small value indicates tension with the model together with its error assumptions; it can arise from a wrong mean model, underestimated uncertainties or neglected correlations. An unusually small statistic can suggest overestimated uncertainties, correlations or overfitting. A [p-value](../../../../../../p-value.md) is not the [probability](../../../../../../probability.md) that the model is true, and failure to reject is not proof of the model.

For counts in categories, the Pearson form is $Q=\sum_{j=1}^k(O_j-E_j)^2/E_j$. Its [chi-squared distribution](../../../../../../chi-squared-distribution.md) is an asymptotic approximation requiring adequate expected counts. For a fixed-total multinomial sample there is one normalization constraint, so the usual [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) are $k-1-p$ after fitting $p$ other parameters. Independent Poisson bins instead start with $k$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) before parameters are fitted. Sparse counts require an appropriate count [likelihood](../../../../../../likelihood-function.md) or a calibrated exact or simulation-based test; plugging tiny expected counts into the asymptotic formula is unreliable. The error model, binning, fitted parameters and chosen test must therefore be reported with the result.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
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
