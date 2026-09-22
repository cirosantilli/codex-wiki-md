<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [local isometry](../../../../../../local-isometry.md) here is a local diffeomorphism whose pullback metric is the source metric. Use the usual convention that a [covering map](../../../../../../covering-space.md) is surjective. Assume the target is connected and the source is nonempty; this is the connected-manifold setting of the intended assertion. For a disconnected target the precise result is a covering of the union of target components met by the map. For example, inclusion $\mathbb R\hookrightarrow\mathbb R\sqcup\mathbb R$ is a [local isometry](../../../../../../local-isometry.md) from a complete manifold but is not a surjective covering of the whole target.

The correct [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md) says that on a connected finite-dimensional [Riemannian manifold](../../../../../../riemannian-manifold.md), completeness for the induced distance is equivalent to [geodesic completeness](../../../../../../geodesic-completeness.md), and to compactness of every closed bounded subset. These conditions imply that every two points are joined by a [minimizing geodesic](../../../../../../minimizing-geodesic.md). The last property by itself does not imply completeness: an open Euclidean ball has minimizing segments between every pair but is incomplete.

A [local isometry](../../../../../../local-isometry.md) preserves the [Levi-Civita connection](../../../../../../levi-civita-connection.md), by uniqueness of the torsion-free metric connection on each [local isometry](../../../../../../local-isometry.md) chart. Hence it preserves affinely parametrized [geodesics](../../../../../../geodesic.md), and

$$
f(\exp_x v)=\exp_{f(x)}(df_xv)
$$

whenever the source [geodesic](../../../../../../geodesic.md) is defined. This is [geodesic preservation by a local isometry](../../../../../../geodesic-preservation-by-a-local-isometry.md).

Suppose $M$ is complete. Given $y\in N$, join $f(x)$ to $y$ by a minimizing target [geodesic](../../../../../../geodesic.md) using target completeness. The source [geodesic](../../../../../../geodesic.md) whose initial velocity is its inverse image under $df_x$ exists for its full parameter interval by source completeness; its image is the target [geodesic](../../../../../../geodesic.md) by uniqueness. Thus $f$ is onto.

Choose a normal ball $U=\exp_y(B_r(0))$ with $\exp_y$ a diffeomorphism on $B_r(0)\subset T_yN$. For every $x\in f^{-1}(y)$ put $U_x=\exp_x(B_r(0))$. Source completeness defines these exponential maps throughout the tangent balls. The displayed exponential identity makes $f:U_x\to U$ a diffeomorphism: injectivity follows from injectivity of the target [exponential map](../../../../../../exponential-map-riemannian-geometry.md), and differentiating the identity shows the source exponential has invertible derivative on the ball, so its image is open.

These sheets are disjoint. If $z$ lay in two, lift the reversed radial target [geodesic](../../../../../../geodesic.md) from $f(z)$ to $y$, starting at $z$. Its initial velocity is uniquely fixed by $df_z$; uniqueness of the source [geodesic](../../../../../../geodesic.md) forces the two sheet centres to be equal. They exhaust $f^{-1}(U)$: for any point over $U$, lift that reversed radial [geodesic](../../../../../../geodesic.md) using source completeness, obtaining a centre over $y$, and then reverse it. Thus $U$ is evenly covered. This proves the [complete local isometry is a covering](../../../../../../complete-local-isometry-is-a-covering.md) assertion.

Conversely suppose $f$ is a covering. Given any initial tangent vector in $M$, the corresponding target [geodesic](../../../../../../geodesic.md) extends over all $\mathbb R$ by target completeness. The [path lifting theorem](../../../../../../path-lifting-theorem.md) for coverings lifts it over every compact time interval, with uniqueness gluing the lifts to a curve on $\mathbb R$. In local covering charts the lift is a [geodesic](../../../../../../geodesic.md), because the charts are [local isometries](../../../../../../local-isometry.md). It extends the source initial-value [geodesic](../../../../../../geodesic.md). Therefore $M$ is geodesically complete, and Hopf-Rinow yields metric completeness on each source component. In the stated connected-target setting,

$$
\boxed{M\text{ is complete}\iff f\text{ is a covering map}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
