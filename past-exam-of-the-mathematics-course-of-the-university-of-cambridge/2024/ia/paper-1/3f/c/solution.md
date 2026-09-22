<h1 id="3f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Another application of the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_{n=1}^N\sqrt{a_n}\,n^{-p}
\leq
\left(\sum_{n=1}^Na_n\right)^{1/2}
\left(\sum_{n=1}^Nn^{-2p}\right)^{1/2}.
$$

When $p>1/2$, the second factor is bounded because $2p>1$, so the [series](../../../../../../series-mathematics.md) converges.

At the endpoint, take $a_1=1$ and, for $n\geq2$,

$$
a_n=\frac1{n(\log n)^2}.
$$

Then $\sum a_n$ converges, while

$$
\sqrt{a_n}\,n^{-1/2}=\frac1{n\log n},
$$

whose [series](../../../../../../series-mathematics.md) diverges. This proves both parts of [weighted square roots of a summable sequence](../../../../../../weighted-square-roots-of-a-summable-sequence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3F](../../3f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
