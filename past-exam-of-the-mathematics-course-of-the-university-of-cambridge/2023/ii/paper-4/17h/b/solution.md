<h1 id="17h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) says that a [bipartite graph](../../../../../../bipartite-graph.md) with classes $A,B$ has a [matching](../../../../../../matching-graph-theory.md) saturating $A$ if and only if

$$
|N(S)|\geq|S|
\qquad\text{for every }S\subseteq A,
$$

where $N(S)$ is the [graph neighbourhood](../../../../../../graph-neighbourhood.md) of $S$. Necessity follows because the matching sends the vertices of $S$ to distinct vertices of $N(S)$.

For sufficiency, add vertices $x,y$, join $x$ to every vertex of $A$, and join every vertex of $B$ to $y$. Let $W$ be an $x$-$y$ vertex separator, and write $W_A=W\cap A$ and $W_B=W\cap B$. If an edge joined a vertex of $A\setminus W_A$ to a vertex of $B\setminus W_B$, it would give an $x$-$y$ path avoiding $W$. Hence

$$
N(A\setminus W_A)\subseteq W_B.
$$

Hall's condition gives

$$
|W_B|\geq|N(A\setminus W_A)|
\geq|A\setminus W_A|,
$$

and therefore $|W|\geq|A|$. By [Menger theorem](../../../../../../menger-theorem.md), there are $|A|$ internally vertex-disjoint $x$-$y$ paths. Each has the form $xaby$ with $a\in A$ and $b\in B$; disjointness makes all the $a$ and all the $b$ distinct. Their middle edges form a matching saturating $A$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
