<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [alternating series test](../../../../../alternating-series-test.md) says that if $a_n\geq0$, $a_{n+1}\leq a_n$, and $a_n\to0$, then $\sum_{n\geq1}(-1)^{n+1}a_n$ converges.

To prove it, let $S_N$ be the partial sums. The even sums satisfy

$$
S_{2m+2}-S_{2m}
=a_{2m+1}-a_{2m+2}\geq0,
$$

so $(S_{2m})$ is increasing. The odd sums satisfy

$$
S_{2m+3}-S_{2m+1}
=-a_{2m+2}+a_{2m+3}\leq0,
$$

so $(S_{2m+1})$ is decreasing. Also $S_{2m}\leq S_{2m+1}$, so both are bounded and converge. Their difference is $a_{2m+1}\to0$, hence their limits agree and the whole sequence $(S_N)$ converges.

Taking $a_n=1/n$ proves convergence of the [alternating harmonic series](../../../../../alternating-harmonic-series.md). Its even partial sums lie below its limit $S$, while its odd partial sums lie above it. Since

$$
S_4=1-\frac12+\frac13-\frac14=\frac7{12}
$$

and

$$
S_5=S_4+\frac15=\frac{47}{60},
$$

we obtain

$$
\boxed{\frac7{12}\leq S\leq\frac{47}{60}}.
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
