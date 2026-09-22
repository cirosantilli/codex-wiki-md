<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If a cubic graph has no cycle of length at most $2r+1$, the [Breadth-first search](../../../../../../breadth-first-search.md) ball of radius $r$ about a vertex is a tree and contains

$$
1+3(1+2+\cdots+2^{r-1})=3\cdot2^r-2
$$

vertices. Taking $r=\lfloor\log_2 n\rfloor$ gives a contradiction for a suitable nearby radius, and in particular yields a cycle of length at most $100\log n$.

Choose such a cycle $C$ of length $m\leq100\log n$. Removing its vertices deletes at most $3m$ edges. The remaining graph has at least $3n/2-3m$ edges on $n-m$ vertices. For all sufficiently large $n$, this exceeds $n-m-1$, so part (a) says the remainder contains a cycle. It is vertex-disjoint from $C$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
