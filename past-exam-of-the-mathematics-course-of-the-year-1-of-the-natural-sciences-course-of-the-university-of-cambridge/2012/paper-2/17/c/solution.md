<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor $1+e^x=2e^{x/2}\cosh(x/2)$. This gives

$$
\ln(1+e^x)=\ln2+\frac x2+\ln\cosh\frac x2.
$$

The last [function](../../../../../function-split.md) is even. Its [Taylor series](../../../../../taylor-series.md) begins $\ln\cosh(x/2)=x^2/8+O(x^4)$, since $\cosh(x/2)=1+x^2/8+O(x^4)$ and $\ln(1+w)=w+O(w^2)$. Therefore

$$
\boxed{\ln(1+e^x)=\ln2+\frac x2+\frac{x^2}{8}+0x^3+O(x^4)}.
$$

In particular, the cubic coefficient is zero; the identity explains its cancellation before any lengthy differentiation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
