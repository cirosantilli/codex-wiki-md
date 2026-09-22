<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with real [vector bundles](../../../../../../vector-bundle.md); for complex bundles replace the [inner products](../../../../../../inner-product.md) below by [positive-definite](../../../../../../positive-definite-bilinear-form.md) [Hermitian forms](../../../../../../hermitian-form.md). A smooth rank-$r$ [vector bundle](../../../../../../vector-bundle.md) is a smooth total space $E$ with a smooth projection $\pi:E\to M$, a real [vector space](../../../../../../vector-space-split.md) structure on each [fiber](../../../../../../fiber-of-a-function.md) $E_p$, and an [open cover](../../../../../../open-cover.md) with [vector bundle trivializations](../../../../../../vector-bundle-trivialization.md)

$$
\Phi_i:\pi^{-1}(U_i)\longrightarrow U_i\times\mathbb R^r.
$$

Each $\Phi_i$ is a [diffeomorphism](../../../../../../diffeomorphism.md) over $U_i$ and is linear on [fibers](../../../../../../fiber-of-a-function.md). The overlap maps have the form $(p,v)\mapsto(p,A_{ji}(p)v)$, where $A_{ji}:U_i\cap U_j\to GL_r(\mathbb R)$ is smooth. The [rank of a vector bundle](../../../../../../rank-of-a-vector-bundle.md) may be specified separately on each [connected component](../../../../../../connected-component.md).

A smooth [fiber metric](../../../../../../fiber-metric.md) is a [positive-definite](../../../../../../positive-definite-bilinear-form.md) [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) $h_p$ on each [fiber](../../../../../../fiber-of-a-function.md), with smoothly varying coefficients in every [local frame](../../../../../../frame-of-a-vector-bundle.md). Equivalently it is a smooth section of $\operatorname{Sym}^2E^*$ which is positive definite at every point. Each trivialization supplies a local [fiber metric](../../../../../../fiber-metric.md) $h_i$ by pulling back the Euclidean [inner product](../../../../../../inner-product.md).

A [smooth manifold](../../../../../../smooth-manifold.md) is Hausdorff and second-countable, hence [paracompact](../../../../../../paracompact-space.md). Choose a smooth, locally finite [partition of unity](../../../../../../partition-of-unity.md) $\{\phi_i\}$ subordinate to a trivializing cover, with $\phi_i\ge0$, $\operatorname{supp}\phi_i\subset U_i$, and $\sum_i\phi_i=1$. Define

$$
\boxed{h=\sum_i\phi_i h_i.}
$$

Extend each weighted term by zero outside its trivializing set; its support lies inside that set, so the extension is smooth. Local finiteness makes the sum smooth. At a point $p$ and for $0\ne v\in E_p$, every nonzero term $\phi_i(p)h_i(v,v)$ is positive and at least one such term occurs. Thus $h_p(v,v)>0$. This proves that **every smooth [vector bundle](../../../../../../vector-bundle.md) admits a smooth [fiber metric](../../../../../../fiber-metric.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
