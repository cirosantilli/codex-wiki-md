<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N=C d^{2d}k$ and red-blue colour $K_N$. Split its vertices into two classes of comparable size. At least half the cross-edges have one colour, say red. The [bounded-degree bipartite Ramsey bound](../../../../../../bounded-degree-bipartite-ramsey-bound.md), proved by [dependent random choice](../../../../../../dependent-random-choice.md), gives a set $U$ in one class such that every subset of at most $d$ vertices of $U$ has at least $k$ common red neighbours in the other class.

Let $H=X\sqcup Y$ be a bipartition. Embed $X$ injectively into $U$. List the vertices of $Y$ and embed them one at a time. Each vertex of $Y$ has at most $d$ already embedded neighbours, whose common red neighbourhood has at least $k$ vertices; fewer than $k$ host vertices have yet been used, so a fresh choice is available. This greedily constructs a red copy of $H$. Thus

$$
\boxed{R(H)\leq C d^{2d}k=O(d^{2d}k).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
