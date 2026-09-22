<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\sigma_1=\gamma,\sigma_2,\ldots$ be the [singular values](../../../../../../singular-value.md) of the [normalized adjacency operator of a bipartite graph](../../../../../../normalized-adjacency-operator-of-a-bipartite-graph.md), with the uniform [inner products](../../../../../../inner-product.md) used above. Its ordinary matrix in an [orthonormal basis](../../../../../../orthonormal-basis.md) on each side is $G/\sqrt{|X||Y|}$. Expanding the [trace](../../../../../../matrix-trace.md) of $(\theta_G\theta_G^*)^2$ proves the [box norm singular-value identity](../../../../../../box-norm-singular-value-identity.md)

$$
\|G\|_\square^4
=\mathbb E_{x,x',y,y'}G(x,y)G(x',y)G(x',y')G(x,y')
=\sum_j\sigma_j^4
=\gamma^4+\sum_{j\geq2}\sigma_j^4.
$$

Therefore (ii) immediately implies

$$
\boxed{s\leq c_2^{1/4}},
$$

which is (iii).

Conversely, the square of the [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md) of this operator is

$$
\sum_j\sigma_j^2=\mathbb E_{x,y}G(x,y)^2=\gamma,
$$

since a [graph](../../../../../../graph-split.md) [indicator function](../../../../../../indicator-function.md) takes values zero and one. Under (iii), every $\sigma_j$ with $j\geq2$ is at most $c_3$, so

$$
\sum_{j\geq2}\sigma_j^4
\leq c_3^2\sum_{j\geq2}\sigma_j^2
=c_3^2(\gamma-\gamma^2)
\leq\frac{c_3^2}{4}.
$$

Thus (iii)$\Rightarrow$(ii) with $\boxed{c_2=c_3^2/4}$. This bound also covers the empty and complete [bipartite graphs](../../../../../../bipartite-graph.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
