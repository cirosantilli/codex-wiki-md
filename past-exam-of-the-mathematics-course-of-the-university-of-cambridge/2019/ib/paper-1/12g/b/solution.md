<h1 id="12g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [metric space](../../../../../../metric-space.md) is [complete](../../../../../../completeness.md) when every [Cauchy sequence](../../../../../../cauchy-sequence.md) converges to a point of the space.

Let $x^{(1)},x^{(2)},\ldots$ be a Cauchy sequence in $X$, where $x^{(j)}=(x^{(j)}_1,x^{(j)}_2,\ldots)$. For each positive integer $N$, choose $J_N$ such that

$$
d(x^{(j)},x^{(k)})<2^{-N}
\qquad(j,k\geq J_N).
$$

This inequality says that the first $N$ coordinates of $x^{(j)}$ and $x^{(k)}$ agree. Consequently each coordinate $x_n^{(j)}$ is eventually constant. Let $x_n$ be its eventual value and put $x=(x_1,x_2,\ldots)\in X$.

For $j\geq J_N$, the first $N$ coordinates of $x^{(j)}$ agree with those of $x$, so

$$
d(x^{(j)},x)<2^{-N}.
$$

As $N$ is arbitrary, $x^{(j)}\to x$. Therefore

$$
\boxed{(X,d)\text{ is complete}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
