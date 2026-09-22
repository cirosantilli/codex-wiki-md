<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $z_i=\log Y_i$. The [Weighted graph Laplacian](../../../../../../weighted-graph-laplacian.md) $L_J$ of the tree is defined by

$$
\beta^TL_J\beta
=\sum_{i\ne v_0}J_i(\beta_i-\beta_{a(i)})^2.
$$

Multiplication of the [Gaussian likelihood](../../../../../../gaussian-likelihood.md) by the prior shows that, conditionally on the [precision parameter](../../../../../../precision-parameter.md) $\tau$,

$$
\pi(\beta\mid Y,\tau)
\propto\exp\left\{-\frac12\beta^TM\beta
+\tau z^T\beta\right\},
\qquad
M=\tau I+2L_J+2cI.
$$

Completing the square therefore gives

$$
\beta\mid Y,\tau\sim N(M^{-1}\tau z,M^{-1}).
$$

As a function of $\tau$, the posterior density is

$$
\tau^{n/2}\exp\left\{-\tau\left(1+\frac12\lVert z-\beta\rVert^2\right)\right\},
$$

so, in shape-rate notation,

$$
\tau\mid Y,\beta\sim
\operatorname{Gamma}\left(\frac n2+1,
1+\frac12\lVert z-\beta\rVert^2\right).
$$

The [precision matrix](../../../../../../precision-matrix.md) $M$ has the [sparsity pattern](../../../../../../sparse-matrix.md) of a [tree](../../../../../../tree-graph-theory.md). A sparse [Cholesky decomposition](../../../../../../cholesky-decomposition.md) and its triangular solves have $O(n)$ cost and storage on this graph, while the gamma update also costs $O(n)$. Hence each systematic-scan [Gibbs sampler](../../../../../../gibbs-sampler.md) iteration costs $O(n)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
