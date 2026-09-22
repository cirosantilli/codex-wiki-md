<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $L$ be the maximum perimeter of a two-cell of $X$, taking $L=0$ if there are none. Compactness of the combinatorial complex makes $L$ finite. We show that the vertex-endpoint [metric geodesic](../../../../../../metric-geodesic.md) $\gamma$ stays within $L/2$ of $\widetilde Y^{(1)}$.

Fix a shortest path $\sigma$ in $\widetilde Y^{(1)}$ and choose the reduced diagram of minimum area, then minimum edge count, as in the preceding part. There is no spur in the interior of either boundary side, since both sides are reduced [metric geodesic](../../../../../../metric-geodesic.md) paths in their respective graphs.

There can be no shell with its entire exterior arc $Q$ on $\gamma$: the [Greendlinger lemma](../../../../../../greendlinger-lemma.md) gives a complementary path $P$ shorter than $Q$, contradicting the ambient [metric geodesic](../../../../../../metric-geodesic.md) property. There can be no such shell with $Q$ entirely on $\sigma$ either. If its image cell $R$ belongs to $\widetilde Y$, the shorter complementary path belongs to $\widetilde Y^{(1)}$ and contradicts the intrinsic [metric geodesic](../../../../../../metric-geodesic.md) property of $\sigma$. If $R$ is outside $\widetilde Y$, the given perimeter decomposition has an arc $I$ of length at least half the perimeter all of whose edges are outside $\widetilde Y$. Any contiguous boundary arc whose edges lie in $\widetilde Y$ must then be contained in the complementary arc $O$ and has length at most half the perimeter. This contradicts $|Q|>|\partial R|/2$.

Thus every shell or spur of the diagram must straddle one of the two marked boundary corners $p,q$. Distinct shell exterior arcs have disjoint interiors, so there can be at most two such exposed features. The [Greendlinger ladder theorem](../../../../../../greendlinger-ladder-theorem.md) now says that the diagram is a single cell or a ladder, apart from common edge paths and the zero-area case. Its two ends contain the marked corners; each intervening cell has one boundary arc on $\gamma$ and one on $\sigma$. Common edge paths already map into $\widetilde Y$.

For a point $z$ of the $\gamma$ arc of a cell, choose a vertex on its $\sigma$ arc. One of the two paths around that cell boundary to the chosen vertex has length at most half the perimeter. Its image is an ambient path to $\widetilde Y^{(1)}$, so

$$
\boxed{d_{\widetilde X^{(1)}}(z,\widetilde Y^{(1)})\leq\frac L2.}
$$

The same argument treats a single cell. In the zero-area case the reduced boundary sides coincide and already lie in $\widetilde Y^{(1)}$.

Finally allow endpoints in the interiors of edges of $\widetilde Y^{(1)}$. The initial and final partial edges of a graph [metric geodesic](../../../../../../metric-geodesic.md) lie in $\widetilde Y^{(1)}$; what remains is a [metric geodesic](../../../../../../metric-geodesic.md) between vertices of that [CW subcomplex](../../../../../../cw-subcomplex.md). If both endpoints are joined without reaching a vertex, the whole segment is already in its edge. Thus the same bound applies to every graph [metric geodesic](../../../../../../metric-geodesic.md), and

$$
\boxed{\widetilde Y^{(1)}\text{ is }(L/2)\text{-quasiconvex in }\widetilde X^{(1)}.}
$$

This is [quasiconvexity from no missing shells](../../../../../../quasiconvexity-from-no-missing-shells.md). The intrinsic path $\sigma$ was never assumed to be an ambient [metric geodesic](../../../../../../metric-geodesic.md), and the bound is independent of the endpoints and of its length.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
