<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [coordinate chart](../../../../../../manifold-chart.md) $x:U\to x(U)$ and either [orientation](../../../../../../orientation-of-a-simplex.md) sheet over $U$, take the chart $x\circ\pi$ on that sheet. On a nonempty overlap, its transition to $y\circ\pi$ is exactly $y\circ x^{-1}$, restricted to the open agreement set from part (a). It is smooth with smooth inverse. These charts therefore define a smooth structure for which $\pi$ is locally a [diffeomorphism](../../../../../../diffeomorphism.md).

The topology is [Hausdorff](../../../../../../hausdorff-space.md): points with distinct base points are separated by inverse images of disjoint base neighborhoods; two points over the same base point are separated by the two disjoint sheets over one coordinate neighborhood. A countable coordinate cover of $M$ gives a countable collection of two-sheeted charts, whose Euclidean chart bases show [second countability](../../../../../../second-countable-space.md). Thus the cover is a genuine [smooth manifold](../../../../../../smooth-manifold.md), not just a collection of compatible charts. The construction using all base charts makes the smooth structure independent of the chosen atlas. It also makes $\pi:\widehat U_\omega\to U$ a [diffeomorphism](../../../../../../diffeomorphism.md) for every oriented open $U$, since it is a bijective local [diffeomorphism](../../../../../../diffeomorphism.md).

At $\widehat p=(p,o_p)$, the derivative $d\pi_{\widehat p}:T_{\widehat p}\widehat M\to T_pM$ is a linear isomorphism. Define the [orientation](../../../../../../orientation-of-a-simplex.md) of $T_{\widehat p}\widehat M$ to be the one mapped to $o_p$. On $\widehat U_\omega$ it is represented by $\pi^*\omega$. Where two sheets overlap, their base [orientation](../../../../../../orientation-of-a-simplex.md) forms differ by a positive function, so their pullbacks determine the same [orientation](../../../../../../orientation-of-a-simplex.md). This proves the **canonical [orientation](../../../../../../orientation-of-a-simplex.md) of the cover**:

$$
\boxed{o_{\widehat p}=(d\pi_{\widehat p})^{-1}o_p.}
$$

The deck involution $(p,o_p)\mapsto(p,-o_p)$ reverses this [canonical orientation of the orientation double cover](../../../../../../canonical-orientation-of-the-orientation-double-cover.md). No global [orientation](../../../../../../orientation-of-a-simplex.md) of the base was used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
