<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A proper $k$-coloring assigns one of $k$ colors to each vertex so adjacent vertices receive different colors. The [chromatic number](../../../../../../chromatic-number.md) $\chi(G)$ is the least such $k$. Order the vertices arbitrarily and color greedily. At most $\Delta(G)$ colors are forbidden by previously colored neighbors, so

$$
\boxed{\chi(G)\leq\Delta(G)+1}.
$$

Equality occurs for every possible maximum degree: use $K_1$ for $\Delta=0$, $K_2$ for $\Delta=1$, an odd cycle for $\Delta=2$, and $K_{\Delta+1}$ for every $\Delta\geq3$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
