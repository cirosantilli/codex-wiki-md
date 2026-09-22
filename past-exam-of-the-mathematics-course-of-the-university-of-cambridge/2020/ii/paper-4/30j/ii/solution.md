<h1 id="30j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $I_s$ independently and uniformly from $\{1,\ldots,n\}$. Starting from any $\beta_1\in C$, the [projected stochastic gradient descent](../../../../../../projected-stochastic-gradient-descent.md) iteration is

$$
G_s=-\frac{y_{I_s}x_{I_s}}{\log(2)[1+\exp(y_{I_s}x_{I_s}^T\beta_s)]},
\qquad
\beta_{s+1}=\pi_C(\beta_s-\eta_sG_s).
$$

Conditional on $\beta_s$, $\mathbb E[G_s\mid\beta_s]=\nabla f(\beta_s)$, so $G_s$ is an [unbiased stochastic gradient](../../../../../../unbiased-stochastic-gradient.md). The [metric projection onto a closed convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) keeps every iterate in $C$. For a fixed step size, return the [Cesaro average](../../../../../../cesaro-mean.md) $\bar\beta=k^{-1}\sum_{s=1}^k\beta_s$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
