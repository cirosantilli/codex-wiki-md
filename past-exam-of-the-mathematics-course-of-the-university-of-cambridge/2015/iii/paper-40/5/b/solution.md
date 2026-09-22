<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every integer $m\in\{0,\ldots,N\}$,

$$
m+2\sum_{K=1}^N(m-K)^+
=m+2\sum_{K=1}^{m-1}(m-K)
=m+m(m-1)=m^2.
$$

Thus the [static replication on a finite terminal support](../../../../../../static-replication-on-a-finite-terminal-support.md) consists of **one share and two calls of every listed strike**, held to maturity:

$$
\boxed{S_T^2=S_T+2\sum_{K=1}^N(S_T-K)^+.}
$$

The strike-$N$ call contributes zero at maturity but is harmless in this identity. The portfolio costs $S_0+2\sum_{K=1}^NC_0(K)$. No distributional assumption on the [stock](../../../../../../stock.md) is needed beyond its stated terminal support.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
