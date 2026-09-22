<h1 id="r/1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

If the printed $K_{33}$ means an ordinary $K_{3,3}$ subgraph, the claim is false. Any two distinct hypercube vertices have exactly two common neighbors when their Hamming distance is two, and no common neighbors otherwise. Three common neighbors, required by any pair of vertices on one side of $K_{3,3}$, are therefore impossible.

The valid intended statement is a [graph subdivision](../../../../../graph-subdivision.md) of $K_{3,3}$. An explicit one in $Q_4$ has branch sets $A=\{0000,0011,1100\}$ and $B=\{0001,0010,0100\}$. Six of the nine branch-to-branch connections are direct edges: $0000$ joins all three vertices of $B$, $0011$ joins $0001,0010$, and $1100$ joins $0100$. The other three paths are

$$
\begin{aligned}
0011&\to0111\to0110\to0100,\\
1100&\to1101\to0101\to0001,\\
1100&\to1110\to1010\to0010.
\end{aligned}
$$

Every step changes one bit and the six internal vertices are distinct and are not branch vertices. Thus these paths and direct edges form the required topological subgraph. For $k>4$, append $k-4$ zeros to every label, embedding the construction in $Q_k$.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [1](../../1.md)
3. [R](../../../r.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
