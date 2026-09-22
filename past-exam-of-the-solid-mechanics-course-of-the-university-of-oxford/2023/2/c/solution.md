<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First let $A\downarrow0$ at fixed positive cavity radius $a$ and fixed reference outer radius $B$. Then

$$
\lambda_a=\frac aA\longrightarrow\infty,\qquad
\lambda_b\longrightarrow\left(1+\frac{a^3}{B^3}\right)^{1/3},
$$

and the [pressure](../../../../pressure-split.md) sustaining a finite cavity is

$$
P(a)=-\int_{(1+a^3/B^3)^{1/3}}^\infty
\frac{h'(\lambda)}{\lambda^3-1}\,d\lambda.
$$

**The onset of cavitation is the additional limit $a\downarrow0$.** The outer stretch then tends to one, and the signed critical [pressure](../../../../pressure-split.md) is

$$
\boxed{P_{\mathrm{crit}}=-\int_1^\infty
\frac{h'(\lambda)}{\lambda^3-1}\,d\lambda.}
$$

When this [improper integral](../../../../improper-integral.md) is positive and finite before the minus sign, the tensile loading magnitude is $-P_{\mathrm{crit}}>0$. Thus the cavity opens under tension, even though the load variable is named [pressure](../../../../pressure-split.md). The critical value is independent of the original sphere radius $B$.

For $A=0$ and $a>0$, the [deformation map](../../../../deformation-map.md) is smooth away from $R=0$ but singular at the original centre: $r=(R^3+a^3)^{1/3}$ approaches $a$, rather than zero, as $R\downarrow0$. This is the [elastic cavitation](../../../../elastic-cavitation.md) mechanism; it cannot be represented by a smooth [deformation map](../../../../deformation-map.md) through the centre.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
