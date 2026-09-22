<h1 id="9e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [ratio test](../../../../../../ratio-test.md) says that a [series](../../../../../../series-mathematics.md) $\sum u_n$ whose terms are eventually nonzero converges absolutely if $\limsup |u_{n+1}/u_n|<1$; in particular, it suffices to have $|u_{n+1}/u_n|\leq q<1$ eventually, since then its terms are bounded by a convergent [geometric series](../../../../../../geometric-series.md). The [comparison test for series](../../../../../../comparison-test-for-series.md) states that, for nonnegative terms, comparison with a larger convergent series gives convergence, and comparison with a smaller divergent series gives divergence. For $u_n=n!/n^n$,

$$
\frac{u_{n+1}}{u_n}=\left(\frac n{n+1}\right)^n.
$$

By the [binomial theorem](../../../../../../binomial-theorem.md), $(1+1/n)^n\geq1+n(1/n)=2$. Thus $u_{n+1}/u_n\leq1/2$ for every $n\geq1$, and induction gives $0<u_n\leq2^{1-n}$. The [comparison test for series](../../../../../../comparison-test-for-series.md) with $\sum2^{1-n}=2$ proves

$$
\boxed{\sum_{n\geq1}\frac{n!}{n^n}\text{ converges absolutely}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
