<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On a branch with $y\ne0$, the given [derivative](../../../../../derivative.md) is nonzero wherever the original equation is defined, so use [inverse-function linearization of a first-order equation](../../../../../inverse-function-linearization-of-a-first-order-equation.md) and regard $x$ as a [function](../../../../../function-split.md) of $y$:

$$
\frac{dx}{dy}=\frac{x+y+2}{y},\qquad
\frac{dx}{dy}-\frac xy=1+\frac2y.
$$

The [integrating factor](../../../../../integrating-factor.md) $1/y$ gives

$$
\frac d{dy}\left(\frac xy\right)=\frac1y+\frac2{y^2},
\qquad \frac xy=\ln|y|-\frac2y+C.
$$

Thus the nonzero solutions are given implicitly by

$$
\boxed{x+2=y(\ln|y|+C),\qquad y\ne0.}
$$

Each branch must also retain **$x+y+2\ne0$**; at those excluded points the original right-hand side is undefined and the inverse graph cannot represent a regular $y(x)$. Differentiating the implicit equation gives $y'=1/(\ln|y|+C+1)$, equal to the required quotient wherever these restrictions hold.

The additional solution **$y=0$**, on any interval avoiding $x=-2$, was lost when dividing by $y$ and must be included. It is not defined through the point $(x,y)=(-2,0)$ in the original equation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
