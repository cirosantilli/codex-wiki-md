<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Grassmann graph](../../../../../../grassmann-graph.md) is connected, and its distance can be determined directly. Put $C=A\cap B$, $r=\dim C$, and $s=k-r$. Choose [vectors](../../../../../../vector.md) so that

$$
A=C\oplus\langle a_1,\ldots,a_s\rangle,\qquad
B=C\oplus\langle b_1,\ldots,b_s\rangle.
$$

The [vectors](../../../../../../vector.md) of a [basis](../../../../../../basis.md) of $C$, followed by all the $a_i$ and $b_i$, are independent: a relation would identify a [vector](../../../../../../vector.md) in the two chosen complements modulo $C$, contradicting $A\cap B=C$. For $0\le j\le s$ define

$$
A_j=C\oplus\langle b_1,\ldots,b_j,a_{j+1},\ldots,a_s\rangle.
$$

Each successive pair has an intersection of [dimension](../../../../../../dimension-vector-space.md) $k-1$. Thus $A_0=A$ and $A_s=B$ are joined by a path of length $s$.

For the lower bound, if two vertices $U,V$ are adjacent, their common [vector subspace](../../../../../../vector-subspace.md) $D$ has codimension one in each. Both $\dim(U\cap B)$ and $\dim(V\cap B)$ lie between $\dim(D\cap B)$ and $\dim(D\cap B)+1$. Thus one edge can change the [dimension](../../../../../../dimension-vector-space.md) of the intersection with $B$ by at most one. It must change from $r$ to $k$ along a path from $A$ to $B$, requiring at least $k-r$ edges. Therefore

$$
\boxed{d(A,B)=k-\dim(A\cap B).}
$$

If two ordered pairs have equal distance, their intersections have equal [dimension](../../../../../../dimension-vector-space.md). Construct adapted [bases](../../../../../../basis.md) for each pair as above and extend both to [bases](../../../../../../basis.md) of the ambient [vector space](../../../../../../vector-space-split.md). The invertible [linear map](../../../../../../linear-map.md) between them sends the first ordered pair to the second. It preserves intersection [dimensions](../../../../../../dimension-vector-space.md), so it is a [graph automorphism](../../../../../../graph-automorphism.md). This proves that the [Grassmann graph](../../../../../../grassmann-graph.md) is [distance-transitive](../../../../../../distance-transitive-graph.md), with the required simultaneous images. Its diameter is $k$, because $2k\le n$ permits two disjoint $k$-dimensional [vector subspaces](../../../../../../vector-subspace.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
