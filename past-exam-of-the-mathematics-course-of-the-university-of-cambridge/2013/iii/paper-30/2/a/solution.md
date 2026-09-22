<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $m_i=\mu+\alpha_i$. Apart from a constant, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell=-\frac{IJ}{2}\log\sigma^2-\frac{1}{2\sigma^2}\sum_{i=1}^I\sum_{j=1}^J(Y_{ij}-m_i)^2.
$$

For each group,

$$
\sum_j(Y_{ij}-m_i)^2=\sum_j(Y_{ij}-\overline Y_i)^2+J(\overline Y_i-m_i)^2,
\qquad \overline Y_i=J^{-1}\sum_jY_{ij}.
$$

Thus [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) sets $\widehat m_i=\overline Y_i$. The [corner-point constraint](../../../../../../corner-point-constraint.md) $\alpha_1=0$ identifies $m_1=\mu$, giving

$$
\boxed{\widehat\mu=\overline Y_1,\qquad
\widehat\alpha_i=\overline Y_i-\overline Y_1\quad(i=2,\ldots,I).}
$$

The baseline mean is the first group mean, rather than the grand mean, because of the chosen [identifiability](../../../../../../identifiability.md) constraint.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
