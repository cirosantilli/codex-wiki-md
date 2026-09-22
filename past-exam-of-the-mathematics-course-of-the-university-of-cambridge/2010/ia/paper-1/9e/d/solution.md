<h1 id="9e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $s=\pm1$, the identity $s/(2+s)=-1/3+(2/3)s$ gives

$$
\frac{(-1)^n}{n(2+(-1)^n)}
=-\frac1{3n}+\frac23\frac{(-1)^n}{n}.
$$

The [alternating series test](../../../../../../alternating-series-test.md) applies to $\sum(-1)^n/n$ because $1/n$ decreases to zero; its [partial sums](../../../../../../partial-sum.md) consequently have a finite limit. The [harmonic series](../../../../../../harmonic-series.md) $\sum1/n$ diverges to $+\infty$. Applying the displayed identity to each finite [partial sum](../../../../../../partial-sum.md) yields

$$
\sum_{n=1}^N\frac{(-1)^n}{n(2+(-1)^n)}
=-\frac13\sum_{n=1}^N\frac1n
+\frac23\sum_{n=1}^N\frac{(-1)^n}{n}
\longrightarrow-\infty.
$$

Therefore $\boxed{\text{the series diverges to }-\infty}$. Alternating signs alone do not satisfy the [alternating series test](../../../../../../alternating-series-test.md): the magnitudes jump from $1/(3n)$ at even $n$ to $1/(n+1)$ at the next odd index.

## ↑ Ancestors (11)

1. [D](../d.md)
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
