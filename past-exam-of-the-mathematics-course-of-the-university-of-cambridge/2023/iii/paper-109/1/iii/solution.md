<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $k=k_1+\cdots+k_s$ be an [integer partition](../../../../../../integer-partition.md). Partition $[2k]$ into blocks $X_j$ of sizes $2k_j$. For every $x\in X_j$, include

$$
A_{j,x}=X_j\setminus\{x\}.
$$

There are $2k=n$ sets. Each has odd size; two sets from the same block meet in $2k_j-2$ points, and sets from different blocks are disjoint. Thus every pairwise intersection has even size.

The partition can be recovered from the bipartite [incidence graph](../../../../../../incidence-graph.md) between the sets and ground points. A block with $k_j\geq2$ gives one connected component containing $2k_j$ set-vertices and $2k_j$ point-vertices, while a block with $k_j=1$ gives two isolated edges. Therefore isomorphic families yield the same multiset $(k_1,\ldots,k_s)$. Distinct integer partitions give non-isomorphic families, so there are at least $p(k)$ of them.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
