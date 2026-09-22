<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the [Gaussian function](../../../../../gaussian-function.md) as $e^{-(x-a)^2}=e^{-a^2}e^{2ax}e^{-x^2}$. Multiplying the two [exponential series](../../../../../exponential-series.md) gives

$$
e^{-(x-a)^2}=e^{-a^2}\left[1+2ax+(2a^2-1)x^2+\left(\frac43a^3-2a\right)x^3+O(x^4)\right].
$$

For $a\ne0,\pm1/\sqrt2$, its first three nonzero terms are

$$
\boxed{e^{-a^2}\bigl[1+2ax+(2a^2-1)x^2\bigr].}
$$

Vanishing coefficients require separate treatment in this [Taylor expansion of a translated Gaussian](../../../../../taylor-expansion-of-a-translated-gaussian.md). If $a=0$, the first three nonzero terms are $\boxed{1-x^2+x^4/2}$. If $a=\pm1/\sqrt2$, they are

$$
\boxed{e^{-1/2}\left(1+2ax-\frac{4a}3x^3\right).}
$$

The latter expression retains the cubic term because the quadratic coefficient is zero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
