<h1 id="17h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
T=\{x_1,\ldots,x_k,y_1,\ldots,y_k\}
$$

be the terminal set, and let $C$ be the vertex set of the given [complete graph](../../../../../../complete-graph.md) $K_{2k}$. Any vertex set $S$ meeting every $T$-$C$ path has size at least $2k$: if $|S|<2k$, choose $t\in T\setminus S$ and $c\in C\setminus S$. Since $G$ is $2k$-connected, $G-S$ is connected, so it contains a $t$-$c$ path avoiding $S$, a contradiction.

The [Set version of Menger theorem](../../../../../../set-version-of-menger-theorem.md) therefore gives $2k$ pairwise vertex-disjoint $T$-$C$ paths. Truncate them at their first and last vertices in $T\cup C$. Since both sets have $2k$ vertices, every terminal is the endpoint of one path and the other endpoints are distinct vertices of $C$. Denote the path from a terminal $z$ to its clique endpoint by $R_z$, and call that endpoint $c_z$.

For each $i$, the clique contains the edge $c_{x_i}c_{y_i}$. Concatenating

$$
R_{x_i},\quad c_{x_i}c_{y_i},\quad R_{y_i}
$$

gives an $x_i$-$y_i$ [path in a graph](../../../../../../path-in-a-graph.md). The linkage paths are mutually vertex-disjoint, their clique endpoints are all distinct, and the joining clique edges pair those endpoints without introducing a new vertex. The resulting paths $P_1,\ldots,P_k$ are therefore mutually vertex-disjoint. In particular, under the stated clique hypothesis, the $2k$-connected graph is [$k$-linked](../../../../../../linked-graph.md) for these terminals.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
