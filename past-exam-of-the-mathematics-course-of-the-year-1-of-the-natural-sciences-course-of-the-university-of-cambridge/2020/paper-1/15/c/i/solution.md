<h1 id="15/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Divide numerator and denominator by $x$ before taking their [Maclaurin series](../../../../../../maclaurin-series.md):

$$
\frac{\sin x}{\sinh x}
=\frac{1-x^2/6+x^4/120+O(x^6)}{1+x^2/6+x^4/120+O(x^6)}.
$$

For the reciprocal denominator, the [geometric series](../../../../../../geometric-series.md) gives $1-x^2/6+7x^4/360+O(x^6)$. Multiplying gives the [Taylor expansion](../../../../../../taylor-expansion.md)

$$
\boxed{\frac{\sin x}{\sinh x}=1-\frac{x^2}{3}+\frac{x^4}{18}+O(x^6).}
$$

Strictly, the original quotient has a [removable singularity](../../../../../../removable-singularity.md) at zero; this is the [Taylor series](../../../../../../taylor-series.md) of its continuous, analytic extension with value one there. The absence of odd powers also follows because the ratio of these two odd functions is even.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
