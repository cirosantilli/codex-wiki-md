<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual [clinical trial](../../../../../../clinical-trial.md) sampling assumption that all patients' responses are independent, with fixed positive arm sizes and positive known variances. Marginal [normal distributions](../../../../../../normal-distribution.md) alone would not specify the variance of a treatment contrast without this assumption. Put $\overline Y_i=n_i^{-1}\sum_jY_{ij}$, $v_i=\sigma_i^2/n_i$, and $s_i=\sqrt{v_i+v_0}$. The [sample mean](../../../../../../sample-mean.md) contrast estimates $\delta_i$ and has [standard error](../../../../../../standard-error.md) $s_i$. Thus **the one-sided Wald statistics** are

$$
\boxed{W_i=\frac{\overline Y_i-\overline Y_0}{\sqrt{\sigma_i^2/n_i+\sigma_0^2/n_0}},\qquad i=1,2.}
$$

Large positive values of these [Wald test](../../../../../../wald-test.md) statistics provide evidence against the respective [null hypotheses](../../../../../../null-hypothesis.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
