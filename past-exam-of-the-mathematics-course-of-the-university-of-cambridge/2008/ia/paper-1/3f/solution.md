<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [ratio test](../../../../../ratio-test.md) states that, for a [series](../../../../../series-mathematics.md) $\sum a_n$ with nonzero terms eventually, if $|a_{n+1}/a_n|\to L<1$, the [series](../../../../../series-mathematics.md) converges absolutely; if $L>1$, including $L=\infty$, it diverges because its terms do not tend to zero. At $L=1$ the test is inconclusive: the [harmonic series](../../../../../harmonic-series.md) diverges while $\sum n^{-2}$ converges.

For $|x|<1$, the [ratio test](../../../../../ratio-test.md) applied to $x^n/n$ gives [absolute convergence](../../../../../absolute-convergence.md) when $x\ne0$, and at $x=0$ every such term vanishes. Thus

$$
\sum_{n=1}^N\frac{x^n-1}{n}
=\sum_{n=1}^N\frac{x^n}{n}-\sum_{n=1}^N\frac1n\longrightarrow-\infty.
$$

At $x=1$ all terms are zero, so the [series](../../../../../series-mathematics.md) converges to zero. At $x=-1$, the even terms vanish and the odd terms are $-2/n$, whose [partial sums](../../../../../partial-sum.md) tend to $-\infty$. Finally, if $|x|>1$, then $|x^n-1|/n\geq(|x|^n-1)/n\to\infty$, so the [term test for divergence](../../../../../term-test-for-divergence.md) applies. Consequently

$$
\boxed{\text{The series converges exactly for }x=1,\text{ and its sum there is }0.}
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
