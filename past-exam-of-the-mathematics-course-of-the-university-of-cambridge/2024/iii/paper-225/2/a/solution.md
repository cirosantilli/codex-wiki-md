<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [test statistic](../../../../../../test-statistic.md)

$$
T_n=n\lVert\overline X_n\rVert^2,
\qquad
\overline X_n=\frac1n\sum_{i=1}^nX_i.
$$

Under the [null hypothesis](../../../../../../null-hypothesis.md), the [Hilbert-space central limit theorem](../../../../../../hilbert-space-central-limit-theorem.md) gives $\sqrt n\,\overline X_n\xrightarrow dG$, where $G$ is centered Gaussian with covariance $C_X$. If $C_X\phi_j=\lambda_j\phi_j$, its [Karhunen–Loève expansion](../../../../../../karhunen-loeve-expansion.md) and the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) give

$$
T_n\xrightarrow d\lVert G\rVert^2
=\sum_{j\geq1}\lambda_jZ_j^2,
$$

for independent $Z_j\sim N(0,1)$. Reject for $T_n$ above the $(1-\alpha)$ quantile of this weighted chi-squared law; replacing the $\lambda_j$ by empirical covariance eigenvalues gives a [plug-in estimator](../../../../../../plug-in-estimator.md) of the critical value.

Under every [fixed alternative](../../../../../../fixed-alternative.md) $\mu\ne0$, the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $\overline X_n\xrightarrow p\mu$, so $T_n/n\xrightarrow p\lVert\mu\rVert^2$ and the test is consistent. Under a [local alternative](../../../../../../local-alternative.md) $\mu_n=n^{-1/2}\delta$, the limit is $\lVert G+\delta\rVert^2$, which describes its local power.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
