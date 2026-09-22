<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The triangular-grid form is [Sperner's lemma](../../../../../sperner-s-lemma.md): subdivide a triangle into small triangles meeting edge to edge, label its vertices $1,2,3$, and forbid label $i$ on the side opposite corner $i$. The corner labels are thereby forced. **An odd number of small triangles, in particular at least one, carry all three labels.**

Here is the parity proof. Count incidences of a small triangle with an edge whose endpoint labels are $1,2$. On the outer boundary these edges occur only on the side joining corners $1,2$; traversing that side begins with label one and ends with label two, so the number of changes of label is odd. Interior edges contribute twice to the incidence count. A small triangle with all three labels contributes once; a triangle having only labels one and two contributes twice if it has both, and all other triangles contribute zero. Reduction modulo two therefore proves the assertion.

To obtain the continuous [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) on the triangle, use barycentric coordinates and a continuous map $F$ from the triangle to itself. If a grid vertex is not already fixed, label it by an index $i$ with $x_i>F_i(x)$, which exists since both coordinate sums are one. A point on the side $x_i=0$ cannot receive label $i$, so the discrete lemma applies. On successively finer grids take a fully labelled small triangle. Compactness gives a subsequence converging to one point $x$; all three vertices converge to it because the mesh tends to zero. Passing to the limit in the three label inequalities gives $x_i\ge F_i(x)$ for every $i$. Equal coordinate sums force equality throughout, hence $F(x)=x$.

A closed disk is homeomorphic to a triangle: radial coordinates from an interior point, scaled by the distance to the boundary in each direction, give such a [homeomorphism](../../../../../homeomorphism.md). Conjugation therefore gives the same fixed-point assertion on the disk. If $r$ were a continuous [retraction](../../../../../retraction.md) from the unit disk to its boundary, define $F(x)=-r(x)$. A [fixed point](../../../../../fixed-point.md) would have $|x|=1$, hence $r(x)=x$ and $x=-x$, impossible on the unit circle. Thus **no continuous disk-to-boundary [retraction](../../../../../retraction.md) exists**. The continuous conclusion has been deduced from the grid parity argument, not used to prove it.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
