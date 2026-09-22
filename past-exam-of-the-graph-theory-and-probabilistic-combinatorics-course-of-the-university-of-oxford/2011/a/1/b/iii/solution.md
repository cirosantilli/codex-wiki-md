<h1 id="a/1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Hall's marriage theorem](../../../../../../hall-s-marriage-theorem.md) says that a [bipartite graph](../../../../../../bipartite-graph-split.md) with parts $L,R$ has a [matching](../../../../../../matching-graph-theory-split.md) saturating $L$ if and only if

$$
\boxed{|N(S)|\geq|S|\qquad\text{for every }S\subseteq L.}
$$

Necessity follows because the matched [neighbours](../../../../../../neighbour-of-a-vertex.md) of [vertices](../../../../../../vertex-graph-theory.md) of $S$ are distinct and belong to $N(S)$.

For sufficiency, assume these [inequalities](../../../../../../inequality-mathematics.md). Let $K=U\cup W$ be any [vertex cover](../../../../../../vertex-cover.md), with $U\subseteq L$ and $W\subseteq R$. Every [neighbour](../../../../../../neighbour-of-a-vertex.md) of $S=L\setminus U$ must belong to $W$, since otherwise its [edge](../../../../../../edge-of-a-graph.md) from $S$ is uncovered. Therefore $|W|\geq|N(S)|\geq|S|$, and $|K|\geq|U|+|S|=|L|$. The whole part $L$ is itself a [vertex cover](../../../../../../vertex-cover.md) of size $|L|$. Part (ii) now gives a [matching](../../../../../../matching-graph-theory-split.md) of size exactly $|L|$, so it saturates $L$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
