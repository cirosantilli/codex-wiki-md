<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If no complete [matching](../../../../../matching-graph-theory-split.md) exists, Hall's theorem gives a nonempty $S\subseteq V_1$, of size $k$, with $|N(S)|\le k-1$. The pairs between $S$ and $V_2\setminus N(S)$ must be nonedges, so there are at least

$$
k(n-k+1)=n+(k-1)(n-k)\ge n
$$

missing edges. Hence $e(G)\le n^2-n$, contradicting the strict edge bound. Therefore **a complete [matching](../../../../../matching-graph-theory-split.md) exists**.

The strictness is necessary: isolate one vertex of $V_1$ and put all edges between the remaining $n-1$ left vertices and all $n$ right vertices. There are exactly $n(n-1)$ edges and no [matching](../../../../../matching-graph-theory-split.md) can cover the isolated vertex. This also handles $n=1$.

## ↑ Ancestors (13)

1. [B](../b.md)
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
