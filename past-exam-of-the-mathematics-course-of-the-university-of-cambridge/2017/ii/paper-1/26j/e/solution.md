<h1 id="26j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [set](../../../../../../set-split.md) of finitely disagreeing pairs is $\bigcup_{N\ge0}F_N$, where $F_N$ consists of pairs whose digits agree at every position beyond $N$. For $M>N$, requiring agreement just at positions $N+1,\ldots,M$ defines a union of dyadic rectangles of total area $2^{-(M-N)}$: among the $2^{2M}$ pairs of length-$M$ prefixes, exactly $2^{M+N}$ meet these $M-N$ matching constraints, each rectangle having area $2^{-2M}$.

Since $F_N$ is contained in each of these finite-prefix agreement [sets](../../../../../../set-split.md), its measure is at most $2^{-(M-N)}$ for every $M$, hence zero. [Countable subadditivity](../../../../../../countable-subadditivity-of-a-measure.md) now gives

$$
\boxed{\lambda^2\bigl(f^{-1}([0,\infty))\bigr)=0}.
$$

Thus almost every pair disagrees in infinitely many digits. Dyadic endpoints, treated with the stipulated expansion convention, do not change any rectangle measure.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26J](../../26j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
