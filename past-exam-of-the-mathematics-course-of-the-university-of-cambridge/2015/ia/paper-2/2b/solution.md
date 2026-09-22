<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

The [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are $y=0,1,-1$. To obtain the other solutions of this [separable differential equation](../../../../../separable-differential-equation.md) without losing their signs, set $z=y^{-2}$ on an interval where $y\ne0$. Then $z'=1-z$, so $z=1+Ke^{-t}$. Therefore **all real solutions** are

$$
\boxed{y(t)\equiv0\quad\text{or}\quad y(t)=\frac{s}{\sqrt{1+Ke^{-t}}},\qquad s\in\{-1,1\},}
$$

on intervals where $1+Ke^{-t}>0$. This family includes $y\equiv\pm1$ when $K=0$. For a prescribed finite nonzero $y(0)=y_0$, $s=\operatorname{sgn}y_0$ and $K=y_0^{-2}-1>-1$, so the solution exists for all future time. The [cubic logistic differential equation](../../../../../cubic-logistic-differential-equation.md) has

$$
\boxed{\lim_{t\to\infty}y(t)=\begin{cases}1&y_0>0,\\0&y_0=0,\\-1&y_0<0.\end{cases}}
$$

These are the only possible limits. The sign cannot change by uniqueness, and the denominator tends to one. A nonzero [initial condition](../../../../../initial-condition.md) producing a constant solution is **$y(0)=1$**; **$y(0)=-1$** also works. The central [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is unstable and the two outer [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) attract solutions from their respective half-lines.

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
