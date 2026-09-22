<h1 id="g/g2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Discard the constant factor $2\pi$ when forming the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). For $F=y\sqrt{1+y'^2}$ it becomes

$$
\sqrt{1+y'^2}-\frac d{dx}\frac{yy'}{\sqrt{1+y'^2}}=0,
\qquad yy''=1+y'^2.
$$

The [Beltrami identity](../../../../../beltrami-identity.md), since $F$ has no explicit $x$ dependence, gives $F-y'F_{y'}=y/\sqrt{1+y'^2}=C>0$. Combining with the differential equation yields $y''=y/C^2$. Its exponential solution has coefficients whose product is $C^2/4$, by $y'^2=y^2/C^2-1$. Positivity therefore puts it in the form

$$
\boxed{y(x)=C\cosh((x-K)/C),\qquad C>0}.
$$

Its constants must satisfy $y_1=C\cosh((x_1-K)/C)$ and $y_2=C\cosh((x_2-K)/C)$. Depending on the endpoint data, these equations may have no solution or more than one. A constant function can satisfy a formal first-integral equation but fails the full [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md); it is not an extra extremal.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [G2](../../g2.md)
3. [G](../../../g.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
