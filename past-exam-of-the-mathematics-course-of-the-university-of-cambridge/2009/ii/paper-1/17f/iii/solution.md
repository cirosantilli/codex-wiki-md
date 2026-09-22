<h1 id="17f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take a maximal [matching in a graph](../../../../../../matching-graph-theory.md) with $m$ edges and let $S$ be its $2m$ endpoints. Maximality makes its complement an [independent set](../../../../../../independent-set-graph-theory.md), since an edge wholly outside $S$ could be added. Every vertex outside $S$ therefore sends all its $k$ edges into $S$, giving $k(n-2m)$ crossing edges. Every vertex in $S$ already uses at least one incident edge inside $S$, its matched edge, so it sends at most $k-1$ outside. Hence

$$
k(n-2m)\leq2m(k-1),\qquad
\boxed{m\geq\frac{kn}{4k-2}.}
$$

The maximum [matching in a graph](../../../../../../matching-graph-theory.md) is at least this large. For $k=2$, take any disjoint union of $r$ triangles. It is 2-regular, has $n=3r$ vertices and matching number $r=n/3$, since each triangle contributes exactly one edge. As $r$ varies this gives infinitely many equality examples.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
