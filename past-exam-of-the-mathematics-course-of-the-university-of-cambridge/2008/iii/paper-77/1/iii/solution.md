<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Store a [bounding volume hierarchy](../../../../../../bounding-volume-hierarchy.md) for each object, using [axis-aligned bounding boxes](../../../../../../axis-aligned-bounding-box.md) or tighter enclosing volumes. A leaf contains one [triangle](../../../../../../triangle.md) or a small group; every internal node encloses all its descendants. Start with the two roots. If their [bounding volumes](../../../../../../bounding-volume.md) are disjoint, discard that pair. Otherwise descend into children of one or both nodes, usually splitting the larger node, until overlapping leaf pairs are reached. Apply the exact [triangle-triangle intersection algorithm](../../../../../../triangle-triangle-intersection-algorithm.md) only at these leaves, and stop at the first hit if only a yes/no answer is required. The pruning is sound because disjoint enclosing volumes imply disjoint enclosed [triangles](../../../../../../triangle.md).

A balanced [bounding volume hierarchy](../../../../../../bounding-volume-hierarchy.md) typically takes $O(n\log n)$ work to construct and $O(n)$ storage. It can be reused for repeated queries and refitted when vertex positions move; a rigid transformation can also be handled in a common coordinate frame. Spatial grids or octrees provide another broad-phase strategy: place [triangles](../../../../../../triangle.md) in every cell they meet and test only pairs from common cells, suppressing duplicates. A box test is especially valuable because the small randomly distributed [triangles](../../../../../../triangle.md) almost always fail it.

For $n,m$ of order $10^5$, the naive method has about $10^{10}$ candidate pairs. Hierarchical pruning replaces this by the number of overlapping node pairs and actual candidate leaf pairs. No universal subquadratic worst-case bound follows: interpenetrating or very poorly separated meshes can still generate $nm$ candidates. If “intersection of objects” means overlap of solid volumes rather than intersection of their boundaries, add a point-in-solid containment test when no surface intersections are found; one closed object can lie wholly inside the other. **Use spatial enclosure to prune pairs before exact triangle tests.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
