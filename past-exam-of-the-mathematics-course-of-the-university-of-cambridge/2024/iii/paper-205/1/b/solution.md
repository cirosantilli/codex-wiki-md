<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose a [feature map](../../../../../../feature-map.md) $\phi:\mathbb R^d\to\mathbb R^p$ represented the [Gaussian kernel](../../../../../../gaussian-kernel.md). Choose $n>p$, a unit vector $e$, and points $x_i=iae$ for $i=0,\ldots,n-1$. Their [kernel matrix](../../../../../../kernel-matrix.md) is

$$
K_{ij}=\exp\!\left(-\frac{a^2(i-j)^2}{2\sigma^2}\right)=r^{(i-j)^2},
\qquad r=e^{-a^2/(2\sigma^2)}.
$$

For sufficiently large $a$, hence sufficiently small $r$, every row satisfies

$$
\sum_{j\ne i}|K_{ij}|\leq2\sum_{m\geq1}r^{m^2}<1=K_{ii}.
$$

Thus $K$ is a symmetric [strictly diagonally dominant matrix](../../../../../../strictly-diagonally-dominant-matrix.md) with positive diagonal and is therefore a [positive-definite matrix](../../../../../../positive-definite-matrix.md), so $\operatorname{rank}K=n$.

On the other hand, if $\Phi$ is the $n\times p$ matrix whose $i$th row is $\phi(x_i)^T$, then $K=\Phi\Phi^T$ and $\operatorname{rank}K\leq p<n$, a contradiction. Hence every feature-space realization of the Gaussian kernel requires an [infinite-dimensional vector space](../../../../../../infinite-dimensional-vector-space.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
