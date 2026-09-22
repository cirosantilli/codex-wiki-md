<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S_N=\sum_{n=1}^N(-1)^{n+1}/n$. Integrate the finite [geometric series](../../../../../geometric-series.md) identity $\sum_{k=0}^{N-1}(-t)^k=[1-(-t)^N]/(1+t)$ over $0\leq t\leq1$:

$$
S_N=\int_0^1\frac{1-(-t)^N}{1+t}\,dt=\ln2-(-1)^N\int_0^1\frac{t^N}{1+t}\,dt.
$$

The remainder has [absolute value](../../../../../absolute-value.md) at most $\int_0^1t^Ndt=1/(N+1)\to0$. Hence the [partial sums](../../../../../partial-sum.md) converge, with

$$
\boxed{\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}n=\ln2.}
$$

This proves both convergence and the value of the [alternating harmonic series](../../../../../alternating-harmonic-series.md) without substituting an endpoint into an unproved infinite [power series](../../../../../power-series.md). Its convergence is conditional because the corresponding [harmonic series](../../../../../harmonic-series.md) of [absolute values](../../../../../absolute-value.md) diverges.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
