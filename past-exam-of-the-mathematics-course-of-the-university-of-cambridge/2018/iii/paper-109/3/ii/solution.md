<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We establish [small-set edge isoperimetry in a square grid](../../../../../../small-set-edge-isoperimetry-in-a-square-grid.md) directly by counting row and column transitions. Regard the vertices of the [grid graph](../../../../../../grid-graph.md) as $[n]\times[n]$. Put $s=a-(b-1)^2$, so $1\leq s\leq b-1$. Start with the corner square $[b-1]\times[b-1]$ and add the $s$ vertices $(1,b),\ldots,(s,b)$. In this shape every occupied row and column is a proper initial interval. There are $b-1$ occupied rows and $b$ occupied columns, each contributing exactly one edge to the [edge boundary in a graph](../../../../../../edge-boundary-in-a-graph.md) in its direction. This gives $f_n(a)\leq2b-1$.

For the reverse bound take an arbitrary $a$-vertex set $A$, and let $R,C$ be its numbers of occupied rows and columns. A row or column that is occupied but not full has at least one transition between $A$ and its complement, hence at least one corresponding boundary edge.

Suppose first that no row and no column is full. Then $|\partial_eA|\geq R+C$ and $a\leq RC$. If $R+C\leq2b-2$, the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) would give

$$
a\leq RC\leq\left(\frac{R+C}{2}\right)^2\leq(b-1)^2,
$$

contrary to the stipulated size. Thus $|\partial_eA|\geq2b-1$.

If there is a full row but no full column, all $n$ columns are occupied and proper, giving at least $n>2b-1$ vertical boundary edges. The case of a full column but no full row is identical with the directions exchanged.

It remains to consider a set with both a full row and a full column. All rows and columns are now occupied. If $q$ rows and $t$ columns are full, then $qn\leq a$ and $tn\leq a$. The remaining rows and columns each contribute a boundary edge, so

$$
|\partial_eA|\geq2n-q-t\geq2n-\frac{2a}{n}.
$$

Since $a\leq b^2-b<b^2<n^2/4$, this exceeds $3n/2$, which is larger than $2b-1$. These cases exhaust all sets and prove

$$
\boxed{f_n(a)=2b-1\qquad\bigl((b-1)^2<a\leq b^2-b,\ b<n/2\bigr).}
$$

As usual, $a$ and $b$ are integers; the specified interval is nonempty only for $b\geq2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
