<h1 id="13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M=2x+e^y$ and $N=xe^y-\cos y$. Their cross [partial derivatives](../../../../../partial-derivative.md) agree: $M_y=e^y=N_x$. On the [simply connected](../../../../../simply-connected-space.md) plane, this makes the [differential form](../../../../../differential-form-split.md) exact. Integrating $F_x=M$ gives $F=x^2+xe^y+h(y)$; matching $F_y=N$ then requires $h'(y)=-\cos y$, so one potential is

$$
F(x,y)=x^2+xe^y-\sin y.
$$

The [ordinary differential equation](../../../../../ordinary-differential-equation.md) states $dF/dx=0$ along a solution. Its [initial condition](../../../../../initial-condition.md) fixes the constant to $F(1,\pi/2)=e^{\pi/2}$. Hence the solution is specified implicitly by

$$
\boxed{x^2+xe^y-\sin y=e^{\pi/2},\qquad y(1)=\frac\pi2.}
$$

At the initial point $F_y=e^{\pi/2}\ne0$, so the [implicit function theorem](../../../../../implicit-function-theorem.md) guarantees a unique local branch $y(x)$ through that point.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
