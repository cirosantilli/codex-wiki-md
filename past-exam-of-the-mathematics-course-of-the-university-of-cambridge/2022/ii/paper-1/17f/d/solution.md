<h1 id="17f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [edge chromatic number](../../../../../../edge-chromatic-number.md) $\chi'(G)$ is the least number of colors in a proper coloring of edges, where incident edges receive distinct colors. [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) says a bipartite graph has a matching saturating one side exactly when $|N(S)|\geq|S|$ for every subset $S$ of that side.

In a 4-regular bipartite graph, the $4|S|$ edges leaving $S$ all enter $N(S)$, whose vertices can receive at most $4|N(S)|$ such edges. Hence Hall's condition holds and there is a perfect matching. Remove it and repeat in the resulting 3-, 2-, and 1-regular bipartite graphs. The four perfect matchings give a four-edge-coloring, while every vertex requires four distinct colors. Therefore

$$
\boxed{\chi'(G)=4}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
