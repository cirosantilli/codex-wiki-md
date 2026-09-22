<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $s=\sigma/\sqrt n$, $\mu=\delta/s$, and let $Z_1,Z_2$ be independent [standard normal random variables](../../../../../../standard-normal-random-variable.md) obtained by centering and scaling the separate stage means. Then

$$
W_1=\mu+Z_1,\qquad W_2=\sqrt2\mu+\frac{Z_1+Z_2}{\sqrt2}.
$$

The second statistic uses all patients, so the statistics are correlated even though the stages' new observations are independent. Their [covariance](../../../../../../covariance.md) is $1/\sqrt2$ and each [variance](../../../../../../variance-split.md) is one. This gives the exact [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md)

$$
\boxed{\begin{pmatrix}W_1\\W_2\end{pmatrix}\sim N_2\left[\begin{pmatrix}\mu\\\sqrt2\mu\end{pmatrix},\begin{pmatrix}1&1/\sqrt2\\1/\sqrt2&1\end{pmatrix}\right].}
$$

Under the [null hypothesis](../../../../../../null-hypothesis.md) both means are zero. At $\delta=\delta^*$ replace $\mu$ by $\sqrt n\delta^*/\sigma$; the mean vector is $(\sqrt n\delta^*/\sigma,\sqrt{2n}\delta^*/\sigma)^T$. In this [group sequential design](../../../../../../group-sequential-design.md) the full-sample statistic may be viewed as a potential statistic from the underlying sequence of outcomes, even on paths where recruitment stops.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
