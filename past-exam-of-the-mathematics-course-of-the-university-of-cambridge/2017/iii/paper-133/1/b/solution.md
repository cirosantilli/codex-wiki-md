<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The surviving conclusion is a [quasi-isometry](../../../../../../quasi-isometry.md) from a [word metric](../../../../../../word-metric.md) for a possibly infinite [generating set of a group](../../../../../../generating-set-of-a-group.md). Finite generation cannot be asserted. Choose $x\in X$ and $R\geq0$ so that $Gx$ is $R$-dense; the [cobounded group action](../../../../../../cobounded-group-action.md) hypothesis provides such a choice. Put

$$
S=\{g\in G\setminus\{1\}:d_X(x,gx)\leq2R+1\}.
$$

This set is symmetric because $d_X(x,g^{-1}x)=d_X(gx,x)$. The [metric geodesic](../../../../../../metric-geodesic.md) subdivision argument in the next part gives

$$
\boxed{|g|_S\leq d_X(x,gx)+1,\qquad d_X(x,gx)\leq(2R+1)|g|_S.}
$$

In particular $S$ generates $G$. Apply the same estimates to $g^{-1}h$ to obtain the two-sided bounds for the [orbit map](../../../../../../orbit-map.md); its image is $R$-dense. Thus **a cobounded isometric action on a [metric geodesic](../../../../../../metric-geodesic.md) space admits an orbit [quasi-isometry](../../../../../../quasi-isometry.md) for a suitable, possibly infinite, generating set**. This is the [cobounded orbit map lemma](../../../../../../cobounded-orbit-map-lemma.md).

Infinite stabilizers cause no obstruction to these bounds: all their nonidentity elements belong to $S$ and have length one, although their orbit displacement is zero. The additive constant permits precisely this collapse. For example, every group acts coboundedly on a point; its complete [Cayley graph](../../../../../../cayley-graph.md) for $S=G\setminus\{1\}$ is bounded, but the group need not be finitely generated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
