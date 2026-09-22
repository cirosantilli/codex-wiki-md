<h1 id="8/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $t=1-x$. The analytic solution has $y_1=a_0+O(t)$ with $a_0\ne0$, so the integrand in the [reduction of order](../../../../../../reduction-of-order.md) formula satisfies

$$
\frac1{(1-x)y_1(x)^2}=\frac1{a_0^2(1-x)}+O(1).
$$

Integrating with respect to $x$ gives $-a_0^{-2}\log(1-x)+O(1)$. Multiplication by $y_1$ therefore gives

$$
y_2(x)=-\frac1{a_0}\log(1-x)+O(1).
$$

Any solution independent of $y_1$ has a nonzero coefficient of this second solution. Hence

$$
\boxed{y(x)=K\log(1-x)+O(1),\qquad K\ne0,\quad x\to1^-.}
$$

An added multiple of $y_1$ stays bounded and cannot cancel this logarithm. On the real side $x>1$, the corresponding statement uses $\log|1-x|$.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
