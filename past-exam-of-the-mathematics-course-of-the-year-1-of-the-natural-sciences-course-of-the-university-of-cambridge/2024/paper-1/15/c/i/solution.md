<h1 id="15/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Maclaurin series](../../../../../../maclaurin-series.md) of the [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) is $\cosh x=1+x^2/2+x^4/24+O(x^6)$. The [binomial series](../../../../../../binomial-series.md) with exponent $-1/2$ gives $(1+u)^{-1/2}=1-u/2+3u^2/8+O(u^3)$. Substituting $u=x^2/2+x^4/24+O(x^6)$ yields

$$
\begin{aligned}
(\cosh x)^{-1/2}&=1-\frac12\left(\frac{x^2}{2}+\frac{x^4}{24}\right)+\frac38\left(\frac{x^2}{2}\right)^2+O(x^6)\\
&=\boxed{1-\frac{x^2}{4}+\frac{7x^4}{96}+O(x^6).}
\end{aligned}
$$

These are the first three nonzero terms; the remainder is written in [Big O notation](../../../../../../big-o-notation.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
