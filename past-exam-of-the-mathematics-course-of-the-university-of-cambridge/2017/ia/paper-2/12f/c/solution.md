<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Couple the walk on the [cycle graph](../../../../../../cycle-graph.md) to a [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) $S_j$ on the integer line by taking $Y_j=S_j\bmod n$, using the same $\pm1$ increments. The visited integer interval has distinct residues until its length reaches $n$; an interval of exactly $n$ consecutive integers contains every residue once. Consequently the [cover time](../../../../../../cover-time.md) on the cycle is exactly $T_n$ in this coupling.

Since $T_1=0$, telescope the range-expansion times and use [linearity of expectation](../../../../../../linearity-of-expectation.md), without assuming those times are independent:

$$
\boxed{\mathbb ET=\mathbb ET_n
=\sum_{k=1}^{n-1}\mathbb E[T_{k+1}-T_k]
=\sum_{k=1}^{n-1}k=\frac{n(n-1)}2.}
$$

This is the [expected cover time of a cycle](../../../../../../expected-cover-time-of-a-cycle.md). The restriction $n\geq3$ makes the two neighbours distinct, matching the supplied transition rule.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
