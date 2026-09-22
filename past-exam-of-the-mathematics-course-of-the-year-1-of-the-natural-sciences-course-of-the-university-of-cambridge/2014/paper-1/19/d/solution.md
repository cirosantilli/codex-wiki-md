<h1 id="19/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Index the terms from $n=0$:

$$
S(x)=\sum_{n=0}^{\infty}\frac{x^{n+4}}{(n+3)n!}.
$$

Its absolute successive-term ratio tends to zero for every fixed $x$, so it converges everywhere. Divide by $x$ temporarily and use the [exponential series divided by a shifted index](../../../../../exponential-series-divided-by-a-shifted-index.md) with $k=3$:

$$
\frac{S(x)}x=\int_0^x t^2e^t\,dt
=\big[e^t(t^2-2t+2)\big]_0^x.
$$

Therefore

$$
\boxed{S(x)=x\big[(x^2-2x+2)e^x-2\big].}
$$

At $x=0$ both the original series and this formula are zero, so the temporary division loses no value. The termwise [integration](../../../../../integral-split.md) is justified by uniform convergence of the exponential series on the finite [integration](../../../../../integral-split.md) interval.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
