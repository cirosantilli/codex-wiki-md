<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the larger [normal linear model](../../../../../../normal-linear-model.md), add laboratory intercept offsets $\gamma_BI_{Bi}+\gamma_CI_{Ci}$ to the mean in part (a). The [nested-model F-test](../../../../../../nested-model-f-test.md) compares

$$
H_0:\gamma_B=\gamma_C=0
\qquad\text{against}\qquad
H_1:(\gamma_B,\gamma_C)\ne(0,0).
$$

The smaller and larger models fit four and six mean coefficients respectively. Under $H_0$, independent Gaussian errors with common [variance](../../../../../../variance-split.md) give independent quantities $(\mathrm{RSS}_1-\mathrm{RSS}_2)/\sigma^2\sim\chi^2_2$ and $\mathrm{RSS}_2/\sigma^2\sim\chi^2_{24}$. Thus the [test statistic](../../../../../../test-statistic.md) is

$$
\boxed{F=\frac{(\mathrm{RSS}_1-\mathrm{RSS}_2)/2}{\mathrm{RSS}_2/24}
=\frac{818.72/2}{5103.0/24}=1.9253,\qquad F\mid H_0\sim F_{2,24}.}
$$

The [p-value](../../../../../../p-value.md) is the upper-tail probability $\Pr(F_{2,24}\ge1.9253)=0.1677$. At the conventional 5% [significance level](../../../../../../significance-level.md), do not reject the common-intercept restriction. **Prefer the simpler model `tumour1` on this comparison.** This does not prove the intercepts coincide, nor address the curvature identified in part (b); the exact [F-test](../../../../../../f-test.md) calibration assumes the underlying error and mean assumptions. The one-decimal RSS values give $818.7$ when subtracted, whereas the table's difference uses unrounded values.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
