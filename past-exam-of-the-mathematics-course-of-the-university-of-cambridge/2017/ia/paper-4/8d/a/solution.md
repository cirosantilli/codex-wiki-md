<h1 id="8d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [sequence](../../../../../../sequence.md) $(a_k)$ converges to $a\in\mathbb R$ when for every $\varepsilon>0$ there is $N$ such that $|a_k-a|<\varepsilon$ for all $k\ge N$. A [series](../../../../../../series-mathematics.md) $\sum_{k=1}^{\infty}a_k$ converges to a finite $S$ when its [partial sums](../../../../../../partial-sum.md) $s_n=\sum_{k=1}^n a_k$ converge to $S$.

If the [series](../../../../../../series-mathematics.md) converges, then $a_n=s_n-s_{n-1}\to S-S=0$, so **its terms tend to zero**. The converse is false: the [harmonic series](../../../../../../harmonic-series.md) has terms tending to zero but diverges.

For the arithmetic averages, suppose $a_k\to a$. Fix $\varepsilon>0$ and choose $K$ so $|a_k-a|<\varepsilon/2$ for $k\ge K$. The finite initial contribution $C=\sum_{k=1}^{K-1}|a_k-a|$ is fixed, and

$$
\left|\frac1n\sum_{k=1}^na_k-a\right|\le\frac Cn+\frac1n\sum_{k=K}^n|a_k-a|\le\frac Cn+\frac\varepsilon2.
$$

For sufficiently large $n$, $C/n<\varepsilon/2$, proving

$$
\boxed{\frac1n\sum_{k=1}^na_k\longrightarrow a.}
$$

This is the [Cesaro theorem for convergent sequences](../../../../../../cesaro-theorem-for-convergent-sequences.md). Its hypothesis concerns a [convergent sequence](../../../../../../convergent-sequence.md); the corresponding [series](../../../../../../series-mathematics.md) need not be a [convergent series](../../../../../../convergent-series.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
