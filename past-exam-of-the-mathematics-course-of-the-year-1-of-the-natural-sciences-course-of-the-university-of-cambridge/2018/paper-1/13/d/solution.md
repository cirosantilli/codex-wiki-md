<h1 id="13/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For real solutions with $x>0$, the square root requires $y\ge0$. First retain the solution $y\equiv0$, which would be lost by dividing by a square root of $y$.

For $y>0$, use the [homogeneous first-order differential equation](../../../../../homogeneous-first-order-differential-equation.md) substitution $v=\sqrt{y/x}>0$, so $y=xv^2$, $\sqrt{xy}=xv$ and $y'=v^2+2xvv'$. The equation becomes

$$
(1+v)(v^2+2xvv')=v^2,
\qquad\frac{2(1+v)}{v^2}\,dv=-\frac{dx}{x}.
$$

This is now a [separable differential equation](../../../../../separable-differential-equation.md). Integration gives $-2/v+2\ln v=-\ln x+C$. Since $xv^2=y$, the positive solutions satisfy

$$
\boxed{\ln y-2\sqrt{\frac xy}=C\quad(y>0),\qquad\text{together with }y\equiv0.}
$$

The implicit family is sufficient here because only parts (a) and (b) request an explicit expression. It also shows why the nonnegative choice of $v$ matters: $\sqrt{xy}$ denotes the positive square root.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [13](../../13.md)
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
