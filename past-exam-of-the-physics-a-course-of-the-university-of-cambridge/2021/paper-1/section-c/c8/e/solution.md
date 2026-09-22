<h1 id="section-c/c8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [chi-squared test](../../../../../../chi-squared-test.md) compares the sum of squared standardized [regression residuals](../../../../../../regression-residual.md) with the appropriate [chi-squared distribution](../../../../../../chi-squared-distribution.md). With both line parameters fitted, the data give $\chi^2=4.6537$ on $6-2=4$ degrees of freedom, with upper-tail [P-value](../../../../../../p-value.md) about $0.325$: the fitted [exponential decay](../../../../../../exponential-decay.md) model describes the data adequately.

First consider fixing the alternative lifetime at its central value $\tau_a=0.478\,\mathrm{ps}$. Its slope is $m_a=-1/\tau_a=-2.09205\,\mathrm{ps}^{-1}$. One must refit the normalization rather than retain the earlier intercept. Minimization over the intercept gives $c_a=\bar y-m_a\bar x=7.29773$, and

$$
\chi^2(\tau_a,\widehat c_a)=19.9111
$$

on $6-1=5$ degrees of freedom, with upper-tail [P-value](../../../../../../p-value.md) about $0.00130$. Thus that fixed central lifetime gives a substantially worse fit than $\widehat\tau=0.4216\,\mathrm{ps}$. Equivalently, the increase after profiling over the intercept is

$$
\Delta\chi^2=\frac{S_{xx}}{s^2}(m_a-\widehat m)^2=15.2574.
$$

This fixed-value comparison does not yet include the uncertainty of the alternative measurement.

For the [compatibility of independent lifetime measurements](../../../../../../compatibility-of-independent-lifetime-measurements.md), include both errors. Under the approximately Gaussian lifetime-error model, equality of the two true lifetimes is tested by

$$
\boxed{\chi^2_{\mathrm{compat}}
=\frac{(\widehat\tau-\tau_a)^2}{\sigma_\tau^2+\sigma_a^2}
=\frac{(0.42156-0.478)^2}{0.01274^2+0.023^2}
\simeq4.61.}
$$

This has one degree of freedom and [P-value](../../../../../../p-value.md) approximately $0.032$, equivalent to a $2.15$-[standard deviation](../../../../../../standard-deviation.md) discrepancy. The two measurements are therefore in mild tension: equality is rejected at a $5\%$ significance threshold, but not at $1\%$. There is no unique yes-or-no compatibility verdict without choosing such a threshold. Treating the alternative central value as exact would overstate the disagreement between the experiments.

The lifetime that provides the best fit to these six rates remains $\boxed{\tau=0.4216\,\mathrm{ps}}$, not $0.478\,\mathrm{ps}$. The compatibility calculation above assumes the two experiments have independent uncertainties; a shared systematic error would require its covariance.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
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
