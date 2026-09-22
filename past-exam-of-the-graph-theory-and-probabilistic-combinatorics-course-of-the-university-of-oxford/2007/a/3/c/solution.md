<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $s,t\ge2$, split $(s-1)(t-1)$ vertices into $s-1$ classes of size $t-1$, coloring edges between classes red and edges inside classes blue. The red [graph](../../../../../graph-split.md) has no $K_s$, and every blue component is too small for the [connected](../../../../../connected-space.md) [tree](../../../../../tree-graph-theory-split.md). This proves the lower bound.

For the upper bound let $N=(s-1)(t-1)+1$ and suppose the blue [graph](../../../../../graph-split.md) contains no copy of the [tree](../../../../../tree-graph-theory-split.md). By the permitted chromatic-number statement, its [chromatic number](../../../../../chromatic-number.md) is at most $t-1$. A [graph](../../../../../graph-split.md) of larger [chromatic number](../../../../../chromatic-number.md) would have a subgraph of [chromatic number](../../../../../chromatic-number.md) exactly $t$, obtained by deleting vertices until that number is reached. A proper blue coloring with at most $t-1$ classes puts no blue edges within any class, so each class is a red [clique](../../../../../clique-graph-theory.md). If there is no red $K_s$, each class has at most $s-1$ vertices, contradicting $N>(s-1)(t-1)$. Therefore

$$
\boxed{R(K_s,T)=(s-1)(t-1)+1}.
$$

The one-vertex boundary cases give one directly.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
