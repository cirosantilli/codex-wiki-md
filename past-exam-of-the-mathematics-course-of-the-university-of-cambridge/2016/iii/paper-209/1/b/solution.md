<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the same $M_n,v_i,S,\Delta$ as in part (a). The error of the [weighted realized variance](../../../../../../weighted-realized-variance.md) splits into its centered fluctuation and its deterministic [quadrature error](../../../../../../quadrature-error.md):

$$
\widehat\Lambda_n(g)-\Lambda(g)=M_n+B_n,\qquad
B_n=\sum_i\int_{t_{i-1}}^{t_i}\bigl(g(t_{i-1})-g(s)\bigr)\sigma(s)^2\,ds.
$$

The [Hölder continuity](../../../../../../holder-condition.md) of $g$ controls this [bias](../../../../../../bias-of-an-estimator.md):

$$
|B_n|\leq R\|\sigma^2\|_\infty\sum_i\frac{\delta_i^{1+\alpha}}{1+\alpha}
\leq\frac{R\|\sigma^2\|_\infty}{1+\alpha}\Delta^\alpha.
$$

Since $\mathbb E M_n=0$, the [bias-variance decomposition of mean squared error](../../../../../../bias-variance-decomposition-of-mean-squared-error.md) has no cross term. Part (a) therefore gives

$$
\mathbb E\bigl(\widehat\Lambda_n(g)-\Lambda(g)\bigr)^2
\leq2R^2S\Delta+\frac{R^2S}{(1+\alpha)^2}\Delta^{2\alpha}
\leq3R^2S\max\{\Delta,\Delta^{2\alpha}\}.
$$

Hence **$\widetilde D=3$ is a universal choice**. This argument separately controls the statistical fluctuation and the [Riemann sum](../../../../../../riemann-sum.md) approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
