<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Young lattice](../../../../../../young-s-lattice.md), or Young poset, has one vertex for each [partition of an integer](../../../../../../partition-of-an-integer.md), including the empty partition, ordered by inclusion of their [Young diagrams](../../../../../../young-diagram.md). A diagram covers another exactly when it adds one box. The [Young branching graph](../../../../../../young-branching-graph.md) is its graded graph: vertices at level $i$ are the partitions of $i$, and edges join diagrams differing by one box.

A descending path from $\lambda\vdash n$ to $(1)$ determines a [standard Young tableau](../../../../../../standard-young-tableau.md): label the successive removed boxes $n,n-1,\ldots,2$, then label the remaining box $1$. Every removed box is a [Removable node of a Young diagram](../../../../../../removable-node-of-a-young-diagram.md), so the resulting labels increase along rows and columns. Conversely, deleting boxes in decreasing label order from a [standard Young tableau](../../../../../../standard-young-tableau.md) gives the path. Extending by the unique edge from $(1)$ to the empty diagram yields the usual path-to-tableau correspondence.

For the operator identity, compare the coefficients of each $\mu\vdash i$ in $DU(\lambda)$ and $UD(\lambda)$. If $\mu\ne\lambda$, a common upper cover exists exactly when a common lower cover exists, and each is then unique: the two diagrams differ by exchanging one box, their union is the upper cover and their intersection the lower cover. Since unions and intersections of partition diagrams are again partition diagrams, these off-diagonal coefficients agree.

The coefficient of $\lambda$ in $DU(\lambda)$ is the number of [addable nodes of a Young diagram](../../../../../../addable-node-of-a-young-diagram.md); its coefficient in $UD(\lambda)$ counts the choices of a [Removable node of a Young diagram](../../../../../../removable-node-of-a-young-diagram.md). Along the diagram's boundary the two types of corners alternate, beginning and ending with addable corners. Hence there is exactly one more addable than removable corner. For the empty partition the counts are $1$ and $0$.

Therefore **the up and down operators satisfy**

$$
\boxed{DU-UD=I},
$$

or $D_{i+1}U_i-U_{i-1}D_i=I_i$ at level $i$. At level zero, interpret $D_0$ and the lowering contribution as zero. This makes the [Young lattice](../../../../../../young-s-lattice.md) a [differential poset](../../../../../../differential-poset.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
