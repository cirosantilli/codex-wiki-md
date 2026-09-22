<h1 id="20/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the solution through $x=0$, work on the connected domain $x>-1$. While $y>0$, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\frac{dy}{\sqrt y}=-\frac{dx}{1+x},\qquad 2\sqrt y=-\ln(1+x)+C.
$$

The [initial condition](../../../../../../initial-condition.md) gives $C=2$, so

$$
\boxed{y(x)=\left(1-\frac12\ln(1+x)\right)^2\quad(-1<x\leq e^2-1)}.
$$

The restriction matters: the unsquared equation requires $1-\frac12\ln(1+x)\geq0$. The solution reaches zero at $x_*=e^2-1$. Continuing the squared formula beyond that point would give a positive [derivative](../../../../../../derivative.md), contradicting the original negative square-root right-hand side.

The nonnegative forward continuation is instead

$$
\boxed{y(x)=\begin{cases}
\left(1-\frac12\ln(1+x)\right)^2,&-1<x\leq e^2-1,\\
0,&x\geq e^2-1.
\end{cases}}
$$

The two pieces join with $y'=0$, and both satisfy the original equation. Because the right-hand side is nonpositive for $x>-1$, a nonnegative solution cannot leave zero in the forward direction. This is a finite-time extinction phenomenon for a [separable differential equation](../../../../../../separable-differential-equation.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [20](../../../20.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
