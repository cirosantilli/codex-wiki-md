<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Hall's theorem states that a finite [bipartite graph](../../../../../bipartite-graph-split.md) with classes $L,R$ has a [matching](../../../../../matching-graph-theory-split.md) covering $L$ exactly when $|N(S)|\ge|S|$ for every $S\subseteq L$. Necessity follows because the distinct matched partners of $S$ belong to $N(S)$.

For sufficiency take a maximum [matching](../../../../../matching-graph-theory-split.md). If it leaves $x\in L$ unmatched, explore alternating paths starting at $x$, traversing unmatched edges from left to right and matched edges back to the left. No reached right vertex can be unmatched, since flipping the edges of such an alternating path would augment the [matching](../../../../../matching-graph-theory-split.md). Let $S,T$ be the reached left and right sets. Every neighbour of $S$ lies in $T$: unmatched edges are explored, and a matched edge from a reached left vertex leads to its already reached predecessor. Conversely every member of $T$ is a neighbour of $S$. Their matched partners are exactly $S\setminus\{x\}$, so $|N(S)|=|T|=|S|-1$, contradicting the hypothesis. Thus a [matching](../../../../../matching-graph-theory-split.md) covering $L$ exists.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
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
