<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ramsey number](../../../../../ramsey-number.md) $R(s,t)$ is the least $N$ such that every $N$-vertex [graph](../../../../../graph-split.md) contains a [clique](../../../../../clique-graph-theory.md) of size $s$ or an [independent set](../../../../../independent-set-graph-theory.md) of size $t$. Take $N=R(s-1,t)+R(s,t-1)$ and choose a vertex $v$. Among its $N-1$ other vertices, either it has at least $R(s-1,t)$ neighbours or it has at least $R(s,t-1)$ nonneighbours.

In the first case those neighbours contain an independent $t$-set or an $(s-1)$-[clique](../../../../../clique-graph-theory.md), which joins $v$ to form an $s$-[clique](../../../../../clique-graph-theory.md). In the second case the nonneighbours contain an $s$-[clique](../../../../../clique-graph-theory.md) or an independent $(t-1)$-set, which joins $v$ to form an independent $t$-set. This proves

$$
\boxed{R(s,t)\le R(s-1,t)+R(s,t-1)}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
