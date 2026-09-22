<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

All $a_n$ are positive, and $a_1=e^{-1}$. The [logarithm](../../../../../logarithm.md) turns consecutive ratios into differences, producing the finite [telescoping sum](../../../../../telescoping-sum.md)

$$
\sum_{k=1}^{n}u_k=\sum_{k=1}^{n}\bigl(\ln a_{k+1}-\ln a_k\bigr)=\ln a_{n+1}+1.
$$

Thus, already for every finite $n$,

$$
a_{n+1}=\exp\left(-1+\sum_{k=1}^{n}u_k\right).
$$

If the [partial sums](../../../../../partial-sum.md) converge to $S$, the [continuity](../../../../../continuous-function.md) of the [exponential function](../../../../../exponential-function.md) gives

$$
\boxed{\lim_{n\to\infty}a_n=\exp\left(-1+\lim_{n\to\infty}\sum_{k=1}^{n}u_k\right)=e^{-1+S}.}
$$

The shift from $a_{n+1}$ to $a_n$ preserves the [limit of a sequence](../../../../../limit-of-a-sequence.md). Convergence of the [partial sums](../../../../../partial-sum.md) is established in part (f), so no convergence assumption is left unsupported.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
