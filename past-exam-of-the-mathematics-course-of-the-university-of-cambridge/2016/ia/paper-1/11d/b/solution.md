<h1 id="11d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Rationalize the numerator of the summand:

$$
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}
=\frac1{\sqrt n\,(\sqrt{n+1}+\sqrt n)}
=\frac1{n(\sqrt{1+1/n}+1)}.
$$

For every $n\ge1$ we have $\sqrt{1+1/n}\le\sqrt2$, and therefore

$$
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}
\ge\frac1{(\sqrt2+1)n}>0.
$$

The [harmonic series](../../../../../../harmonic-series.md) diverges, so the [comparison test for series](../../../../../../comparison-test-for-series.md) makes the given positive-term series diverge as well:

$$
\boxed{\sum_{n=1}^\infty
\frac{\sqrt{n+1}-\sqrt n}{\sqrt n}=+\infty.}
$$

For completeness, divergence of the [harmonic series](../../../../../../harmonic-series.md) follows by grouping the terms with $2^k<n\le2^{k+1}$: each such block contributes at least $2^k/2^{k+1}=1/2$. The same rationalization also shows that $n$ times the summand tends to $1/2$. **The summands tend to zero, but their harmonic-size tail prevents convergence.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
