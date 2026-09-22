<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) says that a finite [bipartite graph](../../../../../bipartite-graph-split.md) with parts $L,R$ has a [matching](../../../../../matching-graph-theory-split.md) covering $L$ if and only if $|N(S)|\geq|S|$ for every $S\subseteq L$. Necessity follows because [matching](../../../../../matching-graph-theory-split.md) edges send the vertices of $S$ to distinct neighbours.

For sufficiency, choose a maximum [matching](../../../../../matching-graph-theory-split.md) $M$. If it misses $a\in L$, explore all alternating paths from $a$, taking unmatched edges from left to right and matched edges from right to left. Let $S\subseteq L$ and $T\subseteq R$ be the reached vertices. No vertex of $T$ can be unmatched, since flipping the edges along the resulting [augmenting path](../../../../../augmenting-path.md) would enlarge $M$.

Every neighbour of a reached left vertex is reached on the right: unmatched edges are exploration steps, and a matched edge leads back to an already reached [matching](../../../../../matching-graph-theory-split.md) partner. Thus $T=N(S)$. Each right vertex in $T$ is matched to a reached left vertex other than $a$, and every reached left vertex other than $a$ arose this way. These [matching](../../../../../matching-graph-theory-split.md) partners give a bijection $T\leftrightarrow S\setminus\{a\}$. Hence $|N(S)|=|S|-1$, contradicting the assumed inequality. Therefore the maximum [matching](../../../../../matching-graph-theory-split.md) covers $L$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
