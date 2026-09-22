<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [positive-semidefinite kernel](../../../../../../positive-semidefinite-kernel.md) on $\mathcal X$ is a symmetric function $k:\mathcal X^2\to\mathbb R$ such that, for every $x_1,\ldots,x_n$ and $c_1,\ldots,c_n$,

$$
\sum_{i,j=1}^nc_ic_jk(x_i,x_j)\geq0.
$$

If $k(x,x')=\langle\phi(x),\phi(x')\rangle$ for a [feature map](../../../../../../feature-map.md) into an [inner product space](../../../../../../inner-product-space.md), then

$$
\sum_{i,j}c_ic_jk(x_i,x_j)
=\left\|\sum_ic_i\phi(x_i)\right\|^2\geq0.
$$

Thus every feature-map inner product is a kernel. If $\alpha_1,\alpha_2\geq0$, then each finite quadratic form for $\alpha_1k_1+\alpha_2k_2$ is the corresponding nonnegative linear combination, so **nonnegative linear combinations of kernels are kernels**.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
