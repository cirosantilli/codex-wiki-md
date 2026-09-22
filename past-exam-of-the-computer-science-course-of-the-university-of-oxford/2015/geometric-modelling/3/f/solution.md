<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With $i$ processed [points](../../../../../point-geometry.md), a triangulated three-dimensional [convex hull](../../../../../convex-hull.md) has $O(i)$ faces and edges. For a sphere-like triangular boundary, the [Euler characteristic](../../../../../euler-characteristic.md) and $3F=2E$ give $F=2V-4$ and $E=3V-6$, with $V\le i$. The complete face scan, horizon construction and adjacency update in the implementation of part (e) therefore cost $O(i)$ per insertion. Consequently,

$$
\boxed{T(n)=O\!\left(\sum_{i=4}^{n-1}i\right)=O(n^2),\qquad\text{working storage }O(n).}
$$

The quadratic worst case really occurs for this implementation. Choose all input [points](../../../../../point-geometry.md) in strictly [convex](../../../../../convex-function.md) position, for example distinct [points](../../../../../point-geometry.md) $(t,t^2,t^3)$ on the three-dimensional [moment curve](../../../../../moment-curve.md). Each processed [point](../../../../../point-geometry.md) remains a hull [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md), so the hull has $2i-4$ triangular faces after $i$ insertions. Scanning every face at every next insertion takes $\Theta(n^2)$ sign tests. This argument does not require every insertion to delete most faces: the repeated global scans already force the bound. More elaborate [convex hull](../../../../../convex-hull.md) algorithms with different search machinery are not the implementation being analysed here.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
