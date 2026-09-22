<h1 id="17f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Hall's marriage theorem](../../../../../../hall-s-marriage-theorem.md) states that a finite [bipartite graph](../../../../../../bipartite-graph.md) with parts $A,B$ has a [matching in a graph](../../../../../../matching-graph-theory.md) saturating $A$ exactly when $|N(S)|\geq|S|$ for every $S\subseteq A$. Necessity follows because the matched neighbours of $S$ are distinct.

For sufficiency use induction on $|A|$. The empty case is immediate. If a nonempty proper subset $S$ has $|N(S)|=|S|$, the induced graph on $S,N(S)$ satisfies Hall's condition and has a saturating [matching in a graph](../../../../../../matching-graph-theory.md) by induction. The remaining graph on $A\setminus S,B\setminus N(S)$ also satisfies it: for $T\subseteq A\setminus S$,

$$
|N(T)\setminus N(S)|=|N(T\cup S)|-|N(S)|\geq|T|.
$$

Apply induction again and unite the two [matchings in a graph](../../../../../../matching-graph-theory.md). If there is no such tight proper subset, every nonempty proper $S$ has $|N(S)|\geq|S|+1$. Choose a vertex $a$ and a neighbour $b$, which exists by Hall's condition. Delete both. Every remaining subset loses at most one neighbour and still satisfies Hall's condition. Induction supplies a [matching in a graph](../../../../../../matching-graph-theory.md) of the remainder; add $ab$. For $|A|=1$ this last step directly proves the assertion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
