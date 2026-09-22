<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $X$ having rows $x_i^T=(1,g_i,m_i)$ and $\mu_i(\beta)=e^{x_i^T\beta}$, the [quasi-score equation](../../../../../../quasi-score-equation.md) is

$$
X^T\{Y-\mu(\beta)\}=0.
$$

It is the same coefficient equation as for Poisson maximum likelihood, explaining why the two models have identical coefficient estimates.

Let $W=\operatorname{diag}(\widehat\mu_1,\ldots,\widehat\mu_n)$ and let coordinate $2$ denote gender. The model-based [standard error](../../../../../../standard-error.md) is

$$
\boxed{\operatorname{se}(\widehat\beta_1)
=\sqrt{\widehat\phi\,[(X^TWX)^{-1}]_{22}},
\qquad
\widehat\phi=\frac{X_P^2}{n-3}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
