<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Hall's theorem states that a finite [bipartite graph](../../../../../bipartite-graph-split.md) with classes $L,R$ has a [matching](../../../../../matching-graph-theory-split.md) covering $L$ if and only if $|N(U)|\ge|U|$ for every $U\subseteq L$. Here $N(U)$ is the set of vertices of $R$ adjacent to at least one member of $U$. Necessity follows because matched partners of $U$ are distinct members of $N(U)$.

For sufficiency induct on $|L|$; zero or one vertex is immediate. If a nonempty proper $U\subset L$ has $|N(U)|=|U|$, Hall's condition holds within the [graph](../../../../../graph-split.md) on $U,N(U)$. It also holds on the remaining classes: for $T\subseteq L\setminus U$,

$$
|N(T)\setminus N(U)|=|N(T\cup U)|-|N(U)|\ge|T|.
$$

Induction gives matchings in these two disjoint subgraphs, and their [union](../../../../../set-union.md) covers $L$. Otherwise every nonempty proper $U$ has $|N(U)|\ge|U|+1$. Choose any edge $lr$ and delete its two endpoints. Every nonempty subset of the remaining left class was a proper subset of $L$, so deleting $r$ leaves at least as many neighbours as vertices. Induction gives a [matching](../../../../../matching-graph-theory-split.md) there, and adjoining $lr$ completes the [matching](../../../../../matching-graph-theory-split.md). This proves sufficiency in all cases.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
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
