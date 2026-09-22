<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

For fixed $k$-element subsets $U,V$, their rectangle is empty with probability $(1-p)^{k^2}$. A [union bound](../../../../../boole-s-inequality.md) over at most $n^{2k}$ choices gives $P(A)\leq n^{2k}(1-p)^{k^2}$. For a specified vertex and a specified $(n-k)$-subset, the chance of no edges is $(1-p)^{n-k}$. There are at most $n\binom nk\leq n^{k+1}$ choices on each side, giving

$$
\boxed{P(B\cup C)\leq2n^{k+1}(1-p)^{n-k}.}
$$

For $n\geq6$, $k=\lceil\sqrt n\rceil\leq n/2$ and $k^2\geq n$. Hence $P(A\cup B\cup C)<3n^{2k}(1-p)^{n/2}$. The logarithm of this bound is $\log3+2k\log n+(n/2)\log(1-p)$, which tends to $-\infty$ because $\sqrt n\log n=o(n)$. Thus the bad-event probability tends to zero.

The printed phrase “almost surely” must mean **asymptotically almost surely as $n\to\infty$**. At any fixed $n$, the empty graph has positive probability $(1-p)^{n^2}$, so the literal probability-one assertion is false.

When no bad event occurs, verify [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md). If $0<|U|\leq k$, each vertex has more than $k$ neighbors because event $B$ is absent, so $|N(U)|\geq|U|$. If $k<|U|\leq n-k$, a failure would leave at least $k$ vertices outside $N(U)$, producing a forbidden empty $k$-square. If $|U|>n-k$, every vertex in $Y$ meets $U$ because event $C$ is absent; hence $N(U)=Y$. The empty set also satisfies Hall. Therefore the graph has a perfect matching whenever the three events are absent, proving the [random bipartite matching from empty-rectangle exclusion](../../../../../random-bipartite-matching-from-empty-rectangle-exclusion.md) result with probability tending to one.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
