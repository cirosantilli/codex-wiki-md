<h1 id="16/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $p>0$, [integration by parts](../../../../../integration-by-parts.md) gives the [Gamma function recurrence](../../../../../gamma-function-recurrence.md):

$$
\Gamma(p+1)=\int_0^\infty x^pe^{-x}dx=[-x^pe^{-x}]_0^\infty+p\int_0^\infty x^{p-1}e^{-x}dx=p\Gamma(p).
$$

The endpoint terms vanish because $x^p\to0$ at zero and the exponential dominates the power at infinity. Also $\Gamma(1)=\int_0^\infty e^{-x}dx=1$. Iterating for nonnegative [integers](../../../../../integer-split.md) $n$ therefore yields

$$
\boxed{\Gamma(n+1)=n!.}
$$

Negative integers are outside this integral definition and factorial conclusion.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
