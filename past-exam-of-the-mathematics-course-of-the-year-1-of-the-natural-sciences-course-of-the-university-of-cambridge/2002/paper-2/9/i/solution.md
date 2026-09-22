<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First expand the [exponential function](../../../../../exponential-function.md) and divide by $x$:

$$
\frac{1-e^{-x}}x=1-\frac x2+\frac{x^2}6-\frac{x^3}{24}+O(x^4).
$$

Seek its reciprocal as $1+Ax+Bx^2+Cx^3+O(x^4)$. Equating coefficients in the product with this expression gives

$$
A-\frac12=0,\qquad B-\frac A2+\frac16=0,\qquad C-\frac B2+\frac A6-\frac1{24}=0.
$$

Hence $A=1/2$, $B=1/12$, $C=0$. The first three nonzero terms of the [Taylor expansion](../../../../../taylor-expansion.md) are

$$
\boxed{\frac{x}{1-e^{-x}}=1+\frac x2+\frac{x^2}{12}+O(x^4).}
$$

Although the quotient is undefined at zero as written, its limit is one, and this [Taylor expansion](../../../../../taylor-expansion.md) belongs to its continuous, [real analytic](../../../../../real-analytic-function.md) extension.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
