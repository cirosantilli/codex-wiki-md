<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At any [vertex](../../../../../../vertex-graph-theory.md), each [complete bipartite graph](../../../../../../complete-bipartite-graph.md) $K_{k,k}$ containing it contributes exactly $k$ incident [edges](../../../../../../edge-of-a-graph.md). Since the copies partition all incident [edges](../../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../../complete-graph.md), $n-1$ is a multiple of $k$. In particular $\gcd(n,k)=1$.

If there are $b$ copies, counting their [edges](../../../../../../edge-of-a-graph.md) gives

$$
\frac{n(n-1)}2=bk^2,\qquad n(n-1)=2bk^2.
$$

Thus $k^2\mid n(n-1)$. Since $n$ is coprime to $k^2$, it can be cancelled in this divisibility, yielding

$$
\boxed{k^2\mid n-1.}
$$

If $n=1$, the empty partition is consistent with the same conclusion, since every positive [integer](../../../../../../integer.md) divides zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
