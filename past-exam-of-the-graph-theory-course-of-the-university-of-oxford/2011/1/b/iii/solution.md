<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) says that a [bipartite graph](../../../../../bipartite-graph-split.md) with parts $L,R$ has a [matching](../../../../../matching-graph-theory-split.md) saturating $L$ if and only if

$$
\boxed{|N(S)|\geq|S|\qquad\text{for every }S\subseteq L.}
$$

Necessity follows because the matched [neighbours](../../../../../neighbour-of-a-vertex.md) of [vertices](../../../../../vertex-graph-theory.md) of $S$ are distinct and belong to $N(S)$.

For sufficiency, assume these [inequalities](../../../../../inequality-mathematics.md). Let $K=U\cup W$ be any [vertex cover](../../../../../vertex-cover.md), with $U\subseteq L$ and $W\subseteq R$. Every [neighbour](../../../../../neighbour-of-a-vertex.md) of $S=L\setminus U$ must belong to $W$, since otherwise its [edge](../../../../../edge-of-a-graph.md) from $S$ is uncovered. Therefore $|W|\geq|N(S)|\geq|S|$, and $|K|\geq|U|+|S|=|L|$. The whole part $L$ is itself a [vertex cover](../../../../../vertex-cover.md) of size $|L|$. Part (ii) now gives a [matching](../../../../../matching-graph-theory-split.md) of size exactly $|L|$, so it saturates $L$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
