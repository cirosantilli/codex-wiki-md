<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

For a connected cellular embedding on the sphere, the [Euler formula for a connected planar graph](../../../../../euler-formula-for-a-connected-planar-graph.md) is

$$
\boxed{V-E+F=2}.
$$

The boundary graph of a convex polyhedron has such an embedding. Counting edge ends at vertices and edge sides at faces gives $\sum_{m\ge3}mV_m=2E=\sum_{n\ge3}nF_n$. Therefore

$$
\begin{aligned}
\sum_{n\ge3}(6-n)F_n&=6F-2E\\
&=6(2-V+E)-2E\\
&=12+\sum_{m\ge3}(2m-6)V_m\ge12.
\end{aligned}
$$

Faces of size six contribute zero, and larger faces contribute negatively. The contribution of each triangle, quadrilateral or pentagon is at most three, so

$$
12\le3F_3+2F_4+F_5\le3(F_3+F_4+F_5).
$$

Thus the [small faces of a spherical polyhedral graph](../../../../../small-faces-of-a-spherical-polyhedral-graph.md) bound is

$$
\boxed{F_3+F_4+F_5\ge4}.
$$

The tetrahedron shows that four is attainable. Connectedness and cellular faces are the standard hypotheses in this Euler formula; an arbitrary disconnected embedded graph has a different count.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
