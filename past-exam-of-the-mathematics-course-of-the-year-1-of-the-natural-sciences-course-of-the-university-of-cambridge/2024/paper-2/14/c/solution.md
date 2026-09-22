<h1 id="14/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [random variable](../../../../../random-variable-split.md) $T$ is the sum $E+(-S)$. The [linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\mathbb E[T]=\mathbb E[E]-\mathbb E[S]=\frac12-\frac12=0.
$$

Multiplication by $-1$ reverses the [mean](../../../../../expected-value-split.md) but preserves the [variance](../../../../../variance-split.md). Under the independence assumption used in part (b), the [variance of a sum](../../../../../variance-of-a-sum.md) gives

$$
\operatorname{Var}(T)=\operatorname{Var}(E)+\operatorname{Var}(-S)
=\frac1{12}+\frac1{12}=\frac16.
$$

Thus both predictions agree with the direct [integrals](../../../../../integral-split.md). For the actual elapsed time, adding twenty-five changes the [mean](../../../../../expected-value-split.md) to twenty-five minutes and leaves the [variance](../../../../../variance-split.md) at $1/6$ minute squared.

Without independence, the correct expression is $\operatorname{Var}(T)=1/6-2\operatorname{Cov}(E,S)$ when both marginals are uniform. This explains why independent endpoint errors must be part of the intended model rather than a consequence of the display format.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
