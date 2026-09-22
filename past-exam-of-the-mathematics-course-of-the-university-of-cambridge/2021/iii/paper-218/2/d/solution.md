<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The beta-binomial regression is

$$
P_j\sim\operatorname{Beta}(\mu_j,\theta),\qquad
C_j\mid P_j\sim\operatorname{Bin}(m_j,P_j),
\qquad
\operatorname{logit}(\mu_j)=z_j^T\beta,
$$

where the beta distribution is parameterized by mean $\mu_j$ and variance parameter $\theta$. Marginally,

$$
\operatorname{Var}(C_j/m_j)
=\frac{\mu_j(1-\mu_j)}{m_j}
\left\{1+(m_j-1)\frac{\theta}{1+\theta}\right\}.
$$

It matches part c when $\rho=\theta/(1+\theta)$, so it is appropriate at the mean-variance level for a common nonnegative intraclass correlation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
