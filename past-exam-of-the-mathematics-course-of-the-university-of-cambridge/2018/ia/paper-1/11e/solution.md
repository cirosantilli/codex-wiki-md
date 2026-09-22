<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The [comparison test for series](../../../../../comparison-test-for-series.md) states that if $0\leq a_n\leq b_n$ eventually and $\sum b_n$ converges, then $\sum a_n$ converges. The partial sums of $\sum a_n$ are increasing and bounded above by a constant plus the bounded partial sums of $\sum b_n$, so the [monotone bounded sequence](../../../../../monotone-bounded-sequence.md) theorem applies.

If $\sum x_n$ converges, then $x_n^2\leq x_n$ proves convergence of $\sum x_n^2$. Also $x_n\to0$, so eventually $x_n\leq1/2$ and $x_n/(1-x_n)\leq2x_n$, proving convergence of $\sum x_n/(1-x_n)$. The converse for the square series is false: $x_n=1/(n+1)$ has convergent square series but divergent original series. The converse for the fraction series is true because $x_n\leq x_n/(1-x_n)$.

If $(x_n)$ is positive and decreasing and $\sum x_n$ converges, put $m=\lfloor n/2\rfloor$. Then

$$
(n-m)x_n\leq\sum_{k=m+1}^{n}x_k\longrightarrow0,
$$

so **$nx_n\to0$**. The converse fails for $x_n=1/(n\log n)$ for $n\geq2$: it is decreasing and $nx_n\to0$, but the [integral test for convergence](../../../../../integral-test-for-convergence.md) shows that its series diverges.

Even convergence of $\sum x_n$ need not imply $(n\log n)x_n\to0$. Choose integers $N_j=\lceil e^{2^j}\rceil$ and set $x_n=(N_j\log N_j)^{-1}$ for $N_{j-1}<n\leq N_j$. This is decreasing, and the $j$th block contributes at most $1/\log N_j\leq2^{-j}$, so the series converges. At $n=N_j$, however, $(n\log n)x_n=1$.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
