<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [series](../../../../../series-mathematics.md) $\sum_{n\ge1}a_n$ converges to $A$ when its [partial sums](../../../../../partial-sum.md) $s_n$ have [limit of a sequence](../../../../../limit-of-a-sequence.md) $A$: for every $\varepsilon>0$, there is $N$ such that $|s_n-A|<\varepsilon$ for all $n\ge N$.

Its averages are the [Cesaro means](../../../../../cesaro-mean.md) of the sequence of [partial sums](../../../../../partial-sum.md). To prove their convergence, choose $N$ with $|s_k-A|<\varepsilon/2$ for $k\ge N$. Then

$$
\left|\frac1n\sum_{k=1}^n s_k-A\right|
\le\frac1n\sum_{k=1}^{N-1}|s_k-A|+\frac{n-N+1}{n}\frac\varepsilon2.
$$

The finite first sum divided by $n$ tends to zero. This proves the [Cesaro theorem for convergent sequences](../../../../../cesaro-theorem-for-convergent-sequences.md) in this setting, and

$$
\boxed{\widetilde A=A.}
$$

The converse fails. Take $a_n=(-1)^{n+1}$, so $s_n=1$ for [odd](../../../../../odd-function.md) $n$ and $s_n=0$ for [even](../../../../../even-function.md) $n$. The [partial sums](../../../../../partial-sum.md) do not converge, but

$$
\boxed{\frac{s_1+\cdots+s_n}{n}=\frac{\lceil n/2\rceil}{n}\longrightarrow\frac12.}
$$

Thus the alternating [series](../../../../../series-mathematics.md) is [Cesàro summable](../../../../../cesaro-summation.md) without having an ordinary sum.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
