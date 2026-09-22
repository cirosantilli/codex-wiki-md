<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes, the two real smooth [vector bundles](../../../../../../vector-bundle.md) are isomorphic, although the choice is not canonical.** A standard [smooth manifold](../../../../../../smooth-manifold.md) is [Hausdorff](../../../../../../hausdorff-space.md) and second countable, hence admits a smooth locally finite [partition of unity](../../../../../../partition-of-unity.md). Choose Euclidean [Riemannian metrics](../../../../../../riemannian-metric.md) on coordinate neighborhoods and take their partition-of-unity sum. At each point at least one positive coefficient occurs, so the resulting smooth symmetric tensor $g$ is positive definite.

The resulting [musical isomorphism](../../../../../../musical-isomorphism.md) is

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g_p(v,\cdot).}
$$

It covers the identity of $M$ and is linear on every fibre. In coordinates it is $(x,v)\mapsto(x,G(x)v)$, where $G=(g_{ij})$ is a smooth positive-definite [matrix](../../../../../../matrix.md). Its inverse uses the smooth inverse [matrix](../../../../../../matrix.md) $G^{-1}$, giving the map $\sharp_g$. Thus it is a smooth [vector bundle isomorphism](../../../../../../vector-bundle-isomorphism.md).

The [Riemannian metric](../../../../../../riemannian-metric.md) supplies the extra choice: no positive-dimensional real [vector space](../../../../../../vector-space-split.md) has a linear identification with its dual invariant under all changes of [basis](../../../../../../basis.md). Indeed a scalar change $tI$ acts by $t$ on vectors and $t^{-1}$ on [covectors](../../../../../../covector.md), so an equivariant map $L$ would satisfy $tL(v)=t^{-1}L(v)$ for every $t>0$, forcing $L=0$. An isomorphism therefore exists without being a metric-free canonical one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
