<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A $d$-dimensional [embedded submanifold](../../../../../embedded-submanifold.md) $F\subseteq M^m$ has the subspace topology and, near each of its points, a [manifold chart](../../../../../manifold-chart.md) identifying it with a coordinate slice $\mathbb R^d\times\{0\}$. These [slice charts for an embedded submanifold](../../../../../slice-chart-for-an-embedded-submanifold.md) give its smooth structure, and its inclusion is a [smooth embedding](../../../../../smooth-embedding.md).

A [regular value](../../../../../regular-value.md) $q\in N^n$ of a [smooth map](../../../../../smooth-map-between-manifolds.md) $f:M^m\to N^n$ is one for which $df_p:T_pM\to T_qN$ is [surjective](../../../../../surjective-function.md) at every $p\in f^{-1}(q)$. If the preimage is nonempty this forces $m\geq n$.

The [inverse function theorem](../../../../../inverse-function-theorem.md) used here says that if $G:U\subseteq\mathbb R^m\to\mathbb R^m$ is smooth and $DG_p$ is an [invertible matrix](../../../../../invertible-matrix.md), then its restriction to a suitable neighbourhood of $p$ is a [diffeomorphism](../../../../../diffeomorphism.md) onto an open neighbourhood of $G(p)$, with smooth inverse.

To prove the [regular level set theorem](../../../../../regular-level-set-theorem.md), fix $p\in f^{-1}(q)$ and choose coordinates centred at $p,q$. The coordinate representative $\widetilde f$ has a rank-$n$ [Jacobian matrix](../../../../../jacobian-matrix.md). After permuting domain coordinates, its first $n$ columns form an [invertible matrix](../../../../../invertible-matrix.md). Define

$$
G(x)=\bigl(\widetilde f^1(x),\ldots,\widetilde f^n(x),x^{n+1},\ldots,x^m\bigr).
$$

Its [Jacobian matrix](../../../../../jacobian-matrix.md) is block triangular with invertible diagonal blocks, so the [inverse function theorem](../../../../../inverse-function-theorem.md) makes $G$ a local coordinate change. In these coordinates, $f^{-1}(q)$ is precisely the slice with first $n$ coordinates zero. Thus it is an [embedded submanifold](../../../../../embedded-submanifold.md) of dimension $m-n$, with

$$
\boxed{T_p f^{-1}(q)=\ker df_p}.
$$

An empty preimage is harmless; the local assertion is then vacuous.

Three [equivalent formulations of orientability of a smooth manifold](../../../../../equivalent-formulations-of-orientability-of-a-smooth-manifold.md) are: an [oriented atlas](../../../../../oriented-atlas.md) whose transition [Jacobian determinants](../../../../../jacobian-determinant.md) are positive; a smoothly varying [orientation of a vector space](../../../../../orientation-of-a-vector-space.md) on each [tangent space](../../../../../tangent-space.md); and a nowhere-vanishing smooth top-degree [differential form](../../../../../differential-form-split.md). An oriented atlas gives compatible oriented coordinate frames. A [partition of unity](../../../../../partition-of-unity.md) glues their positive local top forms, and a nonzero top form declares a frame positive precisely when it evaluates positively on that frame. These constructions prove the equivalence.

For the [orientability of a regular fibre](../../../../../orientability-of-a-regular-fibre.md), write $F=f^{-1}(q)$. The derivative gives a [short exact sequence](../../../../../short-exact-sequence.md) of [vector bundles](../../../../../vector-bundle.md)

$$
0\longrightarrow TF\longrightarrow TM|_F
\xrightarrow{df}F\times T_qN\longrightarrow0.
$$

This is the reason the [normal bundle of a regular fibre is trivial](../../../../../normal-bundle-of-a-regular-fibre-is-trivial.md). Choose any fixed positive basis $b_1,\ldots,b_n$ of $T_qN$ and an ambient orientation on $M$. Declare a frame $v_1,\ldots,v_{m-n}$ of $T_pF$ positive when

$$
\widetilde b_1,\ldots,\widetilde b_n,v_1,\ldots,v_{m-n}
$$

is positive in $T_pM$, where $df_p(\widetilde b_i)=b_i$. Changing a lift adds a tangent vector and leaves the [determinant](../../../../../determinant.md) sign unchanged. Local smooth lifts exist because $df$ is surjective, so this rule varies smoothly and agrees on overlaps. It gives a global orientation on $F$. Only an orientation of the single vector space $T_qN$ was chosen; $N$ itself need not be orientable.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
