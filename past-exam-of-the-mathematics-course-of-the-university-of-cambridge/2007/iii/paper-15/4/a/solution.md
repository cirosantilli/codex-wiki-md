<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every oriented open set $U$ and nowhere-vanishing [orientation](../../../../../../orientation-of-a-simplex.md) form $\omega$, let $\widehat U_\omega$ contain the points $(p,o_p)$ for which $o_p$ is the [orientation](../../../../../../orientation-of-a-simplex.md) determined by $\omega_p$. These sets form a [basis of a topology](../../../../../../basis-of-a-topology.md) for the desired topology on the [orientation double cover](../../../../../../orientation-double-cover.md).

They cover the set of all pairs: every point has an oriented [coordinate chart](../../../../../../manifold-chart.md), and changing the sign of its [orientation](../../../../../../orientation-of-a-simplex.md) form gives the other [orientation](../../../../../../orientation-of-a-simplex.md). To check the basis intersection axiom, consider $\widehat U_\omega$ and $\widehat V_\eta$. On $U\cap V$ there is a unique smooth nonzero function $h$ with $\eta=h\omega$. Their intersection is the sheet over

$$
W=\{p\in U\cap V:h(p)>0\}.
$$

Since $W$ is open, this intersection is $\widehat W_{\omega|_W}$, another basis set. Thus intersections are open without requiring the two local orientations to agree on every component of the overlap.

The restriction $\pi:\widehat U_\omega\to U$ is bijective. Its inverse sends a relatively open set $V\subset U$ to the basis set $\widehat V_{\omega|_V}$, so the inverse is continuous. Conversely the projection of the intersection of $\widehat U_\omega$ with any other basis set is an open agreement set like $W$, so the projection is continuous as well. Hence **each sheet projects homeomorphically onto its oriented open set**. In particular,

$$
\boxed{\pi^{-1}(U)=\widehat U_\omega\sqcup\widehat U_{-\omega},}
$$

with both sheets open. This establishes the two-sheeted [covering space](../../../../../../covering-space.md) structure.

## ↑ Ancestors (11)

1. [A](../a.md)
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
