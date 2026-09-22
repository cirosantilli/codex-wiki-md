<h1 id="17f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here $H$ is the [paw graph](../../../../../../../paw-graph.md), a triangle with a pendant edge.

For the lower bound, partition the vertices of $K_6$ into two triples. Colour the edges inside each triple red and all edges between the triples blue. Each red component is only a triangle, while the blue graph is the triangle-free graph $K_{3,3}$, so there is no monochromatic copy of $H$. Hence $R(H)>6$.

For the upper bound, every colouring of $K_7$ contains a monochromatic triangle because $R(3)=6$. Suppose that a triangle $T$ is red, and let $S$ be the other four vertices. If any edge from $T$ to $S$ were red, it would be a pendant edge extending $T$ to a red $H$. Thus all edges between $T$ and $S$ are blue.

If an edge $xy$ inside $S$ were blue, then for any $u\in T$ the vertices $u,x,y$ would form a blue triangle, and an edge from a second vertex of $T$ to $x$ would extend it to a blue $H$. Therefore every edge inside $S$ is red. The resulting red $K_4$ contains a red triangle and an additional incident edge, hence a red $H$. The blue-triangle case is symmetric, so the [Ramsey number of the paw graph](../../../../../../../ramsey-number-of-the-paw-graph.md) is

$$
\boxed{R(H)=7}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [17F](../../../17f.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
