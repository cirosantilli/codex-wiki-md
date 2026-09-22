<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $b>0$, split the interval into $n$ equal widths $\Delta x=b/n$. Since $x^2$ increases on this interval, the left and right rectangles give lower and upper [Riemann sums](../../../../../riemann-sum.md):

$$
L_n=\frac{b^3}{n^3}\sum_{k=0}^{n-1}k^2,
\qquad
U_n=\frac{b^3}{n^3}\sum_{k=1}^{n}k^2.
$$

Using the finite sum of squares,

$$
U_n=\frac{b^3n(n+1)(2n+1)}{6n^3}\longrightarrow\frac{b^3}{3}.
$$

The rectangle bounds differ by $U_n-L_n=b^3/n\to0$. The [squeeze theorem](../../../../../squeeze-theorem.md) therefore gives, directly from elementary areas,

$$
\boxed{\int_0^b x^2dx=\frac{b^3}{3}.}
$$

For $b=0$ the result is zero. If negative $b$ is allowed, reverse the [integration](../../../../../integral-split.md) limits and use the reflection $x=-u$; the same signed formula holds. No [antiderivative](../../../../../antiderivative.md) is needed for this first-principles calculation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
