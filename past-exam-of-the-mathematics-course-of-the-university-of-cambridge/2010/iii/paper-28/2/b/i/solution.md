<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A real [Gaussian process](../../../../../../../gaussian-process.md) $(Z_t)_{t\in T}$ is a family of [random variables](../../../../../../../random-variable-split.md) such that every finite vector $(Z_{t_1},\ldots,Z_{t_d})$ has a [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md), allowing degenerate distributions. Equivalently every finite real linear combination is a [Gaussian random variable](../../../../../../../gaussian-random-variable.md). Its mean and [covariance kernel](../../../../../../../covariance-kernel.md) are $m(t)=\mathbb EZ_t$ and $C(s,t)=\mathbb E[(Z_s-m(s))(Z_t-m(t))]$.

For any finite set of indices, these functions give the whole mean vector and covariance matrix. The [characteristic function](../../../../../../../characteristic-function.md) of the vector is

$$
\boxed{\mathbb E\exp\!\left(i\sum_{j=1}^d u_jZ_{t_j}\right)
=\exp\!\left(i\sum_j u_jm(t_j)-\frac12\sum_{j,k}u_ju_kC(t_j,t_k)\right).}
$$

The standard uniqueness theorem for [characteristic functions](../../../../../../../characteristic-function.md) therefore determines every [finite-dimensional distribution](../../../../../../../finite-dimensional-distribution.md), including the singular cases. Cylinder events form a generating class for the [product sigma-algebra](../../../../../../../product-sigma-algebra.md) on $\mathbb R^T$ and are closed under finite intersections, so agreement on all cylinder events gives agreement of the process laws by the uniqueness theorem for [probability measures](../../../../../../../probability-measure.md). Thus the mean and covariance determine the law on this coordinate sigma-algebra even when $T$ is uncountable. This statement does not claim uniqueness on an arbitrary finer sigma-algebra of path properties.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
