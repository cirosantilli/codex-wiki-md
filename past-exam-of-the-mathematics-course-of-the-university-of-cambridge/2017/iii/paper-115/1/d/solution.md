<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the standard [smooth manifold](../../../../../../smooth-manifold.md) hypotheses, the first answer is **yes**, although the isomorphism requires a choice. A [partition of unity](../../../../../../partition-of-unity.md) combines Euclidean [inner products](../../../../../../inner-product.md) in [manifold charts](../../../../../../manifold-chart.md) to produce a [Riemannian metric](../../../../../../riemannian-metric.md) $g$. Nonnegative local weights summing to one preserve positivity, and local finiteness preserves smoothness. The [musical isomorphism](../../../../../../musical-isomorphism.md) is

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g(v,\cdot).}
$$

It is smooth and fiberwise invertible, with inverse having local [matrix](../../../../../../matrix.md) $(g_{ij})^{-1}$. It is therefore a [vector bundle isomorphism](../../../../../../vector-bundle-isomorphism.md). There is no preferred such map before a metric or equivalent additional structure is chosen.

The second answer is **no**. On $S^1=\mathbb R/2\pi\mathbb Z$, compare the [trivial vector bundle](../../../../../../trivial-vector-bundle.md) $S^1\times\mathbb R$ with the [Möbius line bundle](../../../../../../mobius-line-bundle.md)

$$
L=(\mathbb R\times\mathbb R)/((t+2\pi,a)\sim(t,-a)).
$$

Both have rank one. A [continuous](../../../../../../continuous-function.md) [section of a vector bundle](../../../../../../section-of-a-vector-bundle.md) of $L$ is represented on $[0,2\pi]$ by a [continuous](../../../../../../continuous-function.md) function $s$ satisfying $s(2\pi)=-s(0)$. If it were nowhere zero, the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) would prevent its endpoint signs from being opposite. Thus $L$ has no [nowhere-zero section](../../../../../../nowhere-zero-section.md). The trivial bundle has the section $1$, and a bundle isomorphism would carry that section to a nowhere-zero section of $L$, a contradiction. Hence

$$
\boxed{L\not\cong S^1\times\mathbb R.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
