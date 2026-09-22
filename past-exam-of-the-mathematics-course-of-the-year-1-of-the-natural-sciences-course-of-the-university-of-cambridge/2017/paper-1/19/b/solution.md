<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $r=\sqrt a>0$ and subtract it from the iteration:

$$
e_{n+1}=\frac{x_n^2+a-2rx_n}{2x_n}
=\frac{(x_n-r)^2}{2x_n}
=\boxed{\frac{e_n^2}{2x_n}}.
$$

This is an [Exact Newton error identity for a quadratic](../../../../../exact-newton-error-identity-for-a-quadratic.md). If $x_n>r$, then $x_n>0$ and $e_n>0$, so $e_{n+1}>0$. Induction from $x_0>r$ proves **$x_n>r$ for every $n$**. Also $x_{n+1}-x_n=(a-x_n^2)/(2x_n)<0$, so the iterates decrease while remaining above the root. Their limit must satisfy $L=(L+a/L)/2$, hence $L=r$. The squared error numerator explains the ensuing [quadratic convergence](../../../../../quadratic-convergence.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
