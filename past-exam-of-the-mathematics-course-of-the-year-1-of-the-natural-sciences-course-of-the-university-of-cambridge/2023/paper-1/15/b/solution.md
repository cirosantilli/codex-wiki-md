<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $u=\ln(1+x)=x-x^2/2+x^3/3+O(x^4)$. Since $u=O(x)$, the outer [Taylor series](../../../../../taylor-series.md) requires $u^2=x^2-x^3+O(x^4)$ and $u^3=x^3+O(x^4)$. Therefore

$$
\begin{aligned}
\ln(1+\ln(1+x))&=u-\frac{u^2}{2}+\frac{u^3}{3}+O(u^4)\\
&=x-\frac{x^2}{2}+\frac{x^3}{3}-\frac12(x^2-x^3)+\frac{x^3}{3}+O(x^4)\\
&=\boxed{x-x^2+\frac{7x^3}{6}+O(x^4).}
\end{aligned}
$$

Both [logarithms](../../../../../logarithm.md) are defined on a neighbourhood of zero, so this composition of [power series](../../../../../power-series.md) is valid there.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
