<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The two pieces of a [one-tree](../../../../1-tree.md) can be optimized independently. Compute a [minimum spanning tree](../../../../minimum-spanning-tree.md) $F$ on vertices $\{2,\ldots,n\}$ and choose the two cheapest distinct edges incident to vertex one. Return their union.

Every feasible [one-tree](../../../../1-tree.md) contains such a [spanning tree](../../../../spanning-tree.md) and such a pair, so its cost is at least the sum of these two independent minima. Their union is itself feasible, attaining that [lower bound](../../../../lower-bound-in-a-partially-ordered-set.md). This proves optimality.

Use [Prim's algorithm](../../../../prim-s-algorithm.md) for $F$: repeatedly add a cheapest edge crossing from the current tree to an unvisited vertex. The [minimum spanning tree cut property](../../../../minimum-spanning-tree-cut-property.md) makes each chosen edge safe. With the dense weight [matrix](../../../../matrix.md) of a complete graph, maintain the best connection to each unvisited vertex and select the least one by a scan. There are $n-2$ iterations with $O(n)$ work apiece. A further scan finds the two cheapest incident edges. Thus the total complexity is $\boxed{O(n^2)}$, with $O(n)$ additional working storage beyond the input [matrix](../../../../matrix.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
