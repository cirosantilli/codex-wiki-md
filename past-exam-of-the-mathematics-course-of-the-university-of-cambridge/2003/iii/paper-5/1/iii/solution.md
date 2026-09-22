<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $F$ be the [free group](../../../../../../free-group.md) on a set $A$. Form the rose $R_A$, a [topological graph](../../../../../../graph-topology.md) with one vertex and one oriented loop for each generator. Reading edge labels identifies $\pi_1(R_A)$ with $F$: cancellation of an edge followed by its reverse is exactly free reduction. This also applies to an infinite generating set, using the graph's CW topology rather than an accumulation topology.

Apply the subgroup-covering construction to obtain a connected [covering graph](../../../../../../covering-graph.md) $Y\to R_A$ with $\pi_1(Y)\cong H$. Choose a [spanning tree](../../../../../../spanning-tree.md) $T\subseteq Y$ and a base vertex $v_0$. For every edge $e\notin T$, choose one orientation and form the loop consisting of the unique tree [path](../../../../../../continuous-path.md) from $v_0$ to the initial vertex of $e$, the edge $e$, and the unique tree [path](../../../../../../continuous-path.md) back from its terminal vertex.

These loops generate $\pi_1(Y)$. Indeed, in any edge loop insert the tree [paths](../../../../../../continuous-path.md) to and from the base vertex between consecutive edges. A tree edge contributes a contractible loop; a non-tree edge contributes the chosen loop or its inverse. They are freely independent as well: reducing an edge [path](../../../../../../continuous-path.md) cancels backtracking, and, after suppressing the tree portions, a nonempty freely reduced word in the oriented non-tree edges cannot disappear. Equivalently, collapsing the tree gives a rose whose petals are precisely the non-tree edges, and the same edge-path reduction identifies its [fundamental group](../../../../../../fundamental-group.md) with the [free group](../../../../../../free-group.md) on those petals.

Thus $\pi_1(Y)$ is free, and its isomorphism with $H$ proves the [Nielsen–Schreier theorem](../../../../../../nielsen-schreier-theorem.md):

$$
\boxed{H\le F\quad\Longrightarrow\quad H\text{ is a free group}.}
$$

The non-tree edges may be infinite in number; the argument does not require $H$ to have finite index or be finitely generated.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
