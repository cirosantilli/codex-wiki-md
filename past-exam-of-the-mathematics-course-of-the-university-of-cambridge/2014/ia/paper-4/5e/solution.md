<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

A real [sequence](../../../../../sequence.md) $(x_n)$ has [limit of a sequence](../../../../../limit-of-a-sequence.md) $x$ when

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\geq N:\quad |x_n-x|<\varepsilon.
$$

A [series](../../../../../series-mathematics.md) $\sum_{n\geq1}x_n$ is a [convergent series](../../../../../convergent-series.md) with sum $s$ when its [partial sums](../../../../../partial-sum.md) $S_N=\sum_{n=1}^Nx_n$ have [limit of a sequence](../../../../../limit-of-a-sequence.md) $s$.

For the first [comparison test for series](../../../../../comparison-test-for-series.md), either of the two allowed bounds implies $0<x_n\leq a_n+b_n$. Hence

$$
0<\sum_{n=1}^Nx_n\leq\sum_{n=1}^{\infty}a_n+\sum_{n=1}^{\infty}b_n<\infty.
$$

The [partial sums](../../../../../partial-sum.md) form a [monotone bounded sequence](../../../../../monotone-bounded-sequence.md), so they converge. **The [series](../../../../../series-mathematics.md) $\sum x_n$ is convergent.**

For the exponent $2$, use $1/n^2\leq1/[n(n-1)]=1/(n-1)-1/n$ for $n\geq2$. The resulting [telescoping series](../../../../../telescoping-series.md) bounds every [partial sum](../../../../../partial-sum.md) by $2$, proving that the [series](../../../../../series-mathematics.md) converges by the [monotone bounded sequence](../../../../../monotone-bounded-sequence.md) property. To prove divergence of the [harmonic series](../../../../../harmonic-series.md), group the terms with $2^j<n\leq2^{j+1}$: their sum is at least $2^j/2^{j+1}=1/2$. Thus its [partial sums](../../../../../partial-sum.md) are unbounded. If $\alpha\leq1$, then $n^{-\alpha}\geq n^{-1}$, so the [comparison test for series](../../../../../comparison-test-for-series.md) proves

$$
\boxed{\sum_{n\geq1}n^{-2}<\infty,\qquad\sum_{n\geq1}n^{-\alpha}=\infty\quad(\alpha\leq1).}
$$

For the weighted square assumption, the finite-dimensional [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives, for every $N$,

$$
\sum_{n=1}^Nx_n=\sum_{n=1}^N(nx_n)\frac1n
\leq\left(\sum_{n=1}^Nn^2x_n^2\right)^{1/2}\left(\sum_{n=1}^N\frac1{n^2}\right)^{1/2}
\leq\left(\sum_{n\geq1}n^2x_n^2\right)^{1/2}\left(\sum_{n\geq1}n^{-2}\right)^{1/2}<\infty.
$$

Again the positive [partial sums](../../../../../partial-sum.md) form a [monotone bounded sequence](../../../../../monotone-bounded-sequence.md). This is the [weighted square roots of a summable sequence](../../../../../weighted-square-roots-of-a-summable-sequence.md) argument, with $a_n=n^2x_n^2$. **The weighted square condition implies $\sum x_n<\infty$.**

**The converse is false.** Take $x_n=n^{-3/2}$. Each block $2^j\leq n<2^{j+1}$ contributes at most $2^j2^{-3j/2}=2^{-j/2}$, and the resulting [geometric series](../../../../../geometric-series.md) converges. But $n^2x_n^2=1/n$, whose [harmonic series](../../../../../harmonic-series.md) diverges. This proves the counterexample without assuming the full [P-series](../../../../../p-series.md) criterion.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
