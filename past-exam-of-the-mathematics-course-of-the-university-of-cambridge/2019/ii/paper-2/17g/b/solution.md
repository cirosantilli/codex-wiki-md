<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the two-colour [matching Ramsey number](../../../../../../matching-ramsey-number.md)

$$
R(rK_2,sK_2)=2r+s-1
\qquad(r\geq s).
$$

Its upper bound follows by induction on $s$. If there is a blue edge, remove its endpoints and apply the induction hypothesis to the remaining $K_{2r+s-3}$: it contains either a red $r$-edge matching or a blue $(s-1)$-edge matching, and in the latter case the removed edge completes a blue $s$-edge matching. If there is no blue edge, the graph itself contains a red $r$-edge matching. For $r=s=t$, this gives the required monochromatic matching in $K_{3t-1}$.

The result never remains true for $K_{3t-2}$, including $t=1$. Partition its vertices into $A$ and $B$ with $|A|=2t-1$ and $|B|=t-1$. Colour edges within $A$ blue and every other edge yellow. A blue matching has at most $t-1$ edges, while every yellow edge meets $B$, so a yellow matching also has at most $t-1$ edges.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
