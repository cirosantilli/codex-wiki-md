<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because the equation depends on the ratio $y/x$, set $u=y/x$, so $y'=u+xu'$. Dividing by $x^2$ and substituting gives

$$
u+xu'+u=1+u^2,\qquad x\frac{du}{dx}=(u-1)^2.
$$

This reduces the [homogeneous first-order differential equation](../../../../../homogeneous-first-order-differential-equation.md) to a [separable differential equation](../../../../../separable-differential-equation.md). For $u\ne1$,

$$
\int\frac{du}{(u-1)^2}=\int\frac{dx}{x},\qquad
-\frac1{u-1}=\ln x+C.
$$

At $x=e$, the condition $y=0$ gives $u=0$, so $1=1+C$ and $C=0$. Hence

$$
\boxed{y(x)=x\left(1-\frac1{\ln x}\right),\qquad 1<x<\infty.}
$$

The interval displayed is the maximal solution interval containing $x=e$: there is a pole at $x=1$. Separating variables omitted the solution $u=1$, or $y=x$, but that solution does not satisfy the given condition.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
