<h1 id="15/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Maclaurin series](../../../../../../maclaurin-series.md) give $e^{-x^3}=1-x^3+O(x^6)$ and $\cosh x=1+x^2/2+x^4/24+O(x^6)$. Inverting the latter using the [geometric series](../../../../../../geometric-series.md) gives

$$
\frac1{\cosh x}=1-\frac{x^2}{2}+\left(\frac14-\frac1{24}\right)x^4+O(x^6)
=1-\frac{x^2}{2}+\frac5{24}x^4+O(x^6).
$$

Multiplying the two expansions yields

$$
\boxed{\frac{e^{-x^3}}{\cosh x}=1-\frac{x^2}{2}-x^3+\frac5{24}x^4+O(x^5).}
$$

The remainder is $O(x^5)$ because the product already generates an $x^5$ term from $(-x^3)(-x^2/2)$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
