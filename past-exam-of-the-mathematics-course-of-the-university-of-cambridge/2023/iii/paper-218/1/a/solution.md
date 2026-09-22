<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For individual $i$, let $Y_i$ be the reported count, $g_i\in\{0,1\}$ the gender indicator, and $m_i\in\{0,1\}$ the minority indicator. The fitted [Poisson regression](../../../../../../poisson-regression.md) is

$$
Y_i\mathrel{\perp\!\!\!\perp}Y_j,
\qquad
Y_i\sim\operatorname{Poisson}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1g_i+\beta_2m_i.
$$

Its [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta)=\sum_{i=1}^{1308}
\{Y_i x_i^T\beta-e^{x_i^T\beta}-\log(Y_i!)\},
\qquad x_i=(1,g_i,m_i)^T.
$$

The [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
(\widehat\beta_0,\widehat\beta_1,\widehat\beta_2)
=(-2.2959,-0.1916,1.7293).
$$

Holding minority status fixed, changing the gender indicator from zero to one multiplies the fitted [conditional expected value](../../../../../../conditional-expectation.md) by $e^{-0.1916}=0.826$. Thus the fitted mean count for men is about $17.4\%$ lower than that for women with the same minority status.

## ↑ Ancestors (11)

1. [A](../a.md)
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
