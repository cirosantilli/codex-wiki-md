<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the terminology used for [positive-definite kernels](../../../../../../positive-semidefinite-kernel.md), positive definiteness means positive semidefiniteness of every finite [kernel matrix](../../../../../../kernel-matrix.md): $k$ is symmetric and, for every $m$, points $x_1,\ldots,x_m$ and real $c_1,\ldots,c_m$,

$$
\sum_{i,j=1}^mc_ic_jk(x_i,x_j)\geq0.
$$

The linear kernel is symmetric, and

$$
\boxed{\sum_{i,j=1}^mc_ic_jx_i^Tx_j=\left\lVert\sum_{i=1}^mc_ix_i\right\rVert_2^2\geq0.}
$$

Thus it is a [positive-semidefinite kernel](../../../../../../positive-semidefinite-kernel.md), with the identity as its [feature map](../../../../../../feature-map.md). It need not be strictly positive definite: a zero vector or linearly dependent points can make this quadratic form zero for nonzero $c$. This distinction is essential when interpreting the terminology.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
