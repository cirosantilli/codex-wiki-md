<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $X_1$ is the sum of two independent centered Gaussian innovations,

$$
\boxed{X_1\sim N(0,\sigma^2(1+\theta^2)).}
$$

For any nonzero $a\in\mathbb R^n$,

$$
a^T\Sigma a
=\operatorname{Var}\left(\sum_{t=1}^na_tX_t\right).
$$

Expanding each $X_t=\varepsilon_t+\theta\varepsilon_{t-1}$ expresses this as $\sigma^2$ times a sum of squared innovation coefficients. If all coefficients vanished, the coefficient of the latest innovation gives $a_n=0$, and backward induction gives every $a_t=0$, a contradiction. Hence $a^T\Sigma a>0$ and the covariance matrix is positive definite.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
