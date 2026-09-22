<h1 id="section-b/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Normalization of a probability distribution](../../../../../../normalization-of-a-probability-distribution.md) and the [geometric series](../../../../../../geometric-series.md) give $1=A/(1-\rho)$, so $A=1-\rho$. For a nonnegative [integer](../../../../../../integer-split.md) $n$, the strict tail starts at $n+1$:

$$
\boxed{\mathbb P(N>n)=\sum_{j=n+1}^\infty(1-\rho)\rho^j=\rho^{n+1}.}
$$

For nonnegative [integers](../../../../../../integer-split.md) $n>m$, the [event](../../../../../../event.md) $\{N>n\}$ is contained in $\{N>m\}$. Therefore

$$
\boxed{\mathbb P(N>n\mid N>m)=\frac{\rho^{n+1}}{\rho^{m+1}}=\rho^{n-m}.}
$$

This is the [memorylessness of the geometric distribution](../../../../../../memorylessness-of-the-geometric-distribution.md) with the zero-based counting convention. Keeping strict versus non-strict inequalities explicit is essential: $N-m-1$, conditional on $N>m$, has the original distribution of $N$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
