<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The printed assertion is false when maximal means largest in the natural-number labelling.** Both the original PDF and the TeX have this wording. The specified operation gives the [complete graph](../../../../../../complete-graph.md), not the [Rado graph](../../../../../../rado-graph.md).

Fix any two distinct vertices $u,v\in\mathbb N$, and choose $M\geq\max\{u,v\}$. Apply the [hypergraph extension property](../../../../../../hypergraph-extension-property.md) of $G^{(3)}_{\mathrm{univ}}$ to $S=\{1,\ldots,M\}$, prescribing that the pair $\{u,v\}$ extend to a [hyperedge](../../../../../../hyperedge.md); prescribe all other pairs in $S$ arbitrarily. The resulting witness $w\notin S$ has $w>M$, so $\{u,v,w\}$ is a [hyperedge](../../../../../../hyperedge.md) whose largest vertex is $w$. Deleting that vertex produces the [edge](../../../../../../edge-of-a-graph.md) $\{u,v\}$ in $G_0$.

Since $u,v$ were arbitrary,

$$
\boxed{G_0=K_{\mathbb N}.}
$$

The [Rado graph](../../../../../../rado-graph.md) has nonedges: its [hypergraph extension property](../../../../../../hypergraph-extension-property.md) supplies a new vertex nonadjacent to any specified existing vertex. Therefore $K_{\mathbb N}$ and $G^{(2)}_{\mathrm{univ}}$ cannot be [isomorphic graphs](../../../../../../graph-isomorphism.md). This argument holds for every representative of the universal three-uniform structure labelled by $\mathbb N$, so changing its labelling does not repair the assertion. Equivalently, in an independently sampled representative each pair has infinitely many larger vertices that complete it to a triple, [almost surely](../../../../../../almost-sure-convergence.md).

A valid related construction is to fix a vertex $a$ and take its [link hypergraph](../../../../../../link-hypergraph.md): make $\{u,v\}$ an [edge](../../../../../../edge-of-a-graph.md) exactly when $\{a,u,v\}$ is a [hyperedge](../../../../../../hyperedge.md), on the remaining [vertex set](../../../../../../vertex-set.md). This is indeed the [Rado graph](../../../../../../rado-graph.md). To prove it, take any disjoint finite sets $U,W$ of vertices other than $a$, put $S=\{a\}\cup U\cup W$, and prescribe triples through the pairs $\{a,u\}$ for $u\in U$ and no triples through $\{a,w\}$ for $w\in W$. Complete all other pair prescriptions arbitrarily. The [hypergraph extension property](../../../../../../hypergraph-extension-property.md) produces a new vertex adjacent in the link to all of $U$ and none of $W$. Uniqueness from part (i), for $r=2$, now proves the claimed [hypergraph isomorphism](../../../../../../hypergraph-isomorphism.md) for this corrected operation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
