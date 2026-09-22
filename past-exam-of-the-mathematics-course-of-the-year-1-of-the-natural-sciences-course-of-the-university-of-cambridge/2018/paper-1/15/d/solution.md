<h1 id="15/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Combine the [logarithms](../../../../../logarithm.md) first and factor out the limiting constant:

$$
\ln(1+x+2x^2)-\ln x^2=\ln\left(2+\frac1x+\frac1{x^2}\right)
=\ln2+\ln\left(1+\frac1{2x}+\frac1{2x^2}\right).
$$

Apply the [Taylor expansion](../../../../../taylor-expansion.md) $\ln(1+u)=u-u^2/2+O(u^3)$ with $u=1/(2x)+1/(2x^2)$. The first three nonzero terms, including the constant, are

$$
\boxed{\ln(1+x+2x^2)-\ln x^2=\ln2+\frac1{2x}+\frac3{8x^2}+O(x^{-3}),\qquad x\to\infty.}
$$

This is an [asymptotic expansion](../../../../../asymptotic-expansion-split.md) in reciprocal powers of $x$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
