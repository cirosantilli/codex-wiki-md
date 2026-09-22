<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

An [integrating factor](../../../../../integrating-factor.md) is

$$
\mu(x)=\exp\left(\int3x^2\,dx\right)=e^{x^3}.
$$

Multiplication by this [integrating factor](../../../../../integrating-factor.md) turns the [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md) into $(e^{x^3}y)'=x^2e^{x^3}$. Integrating from zero to $x$ gives

$$
e^{x^3}y(x)-a=\frac13(e^{x^3}-1).
$$

Thus the [initial value problem](../../../../../initial-value-problem.md) has the solution

$$
\boxed{y(x)=\frac13+\left(a-\frac13\right)e^{-x^3},\qquad \lim_{x\to+\infty}y(x)=\frac13.}
$$

Indeed, direct [differentiation](../../../../../differentiation.md) gives $y'=-3x^2(a-1/3)e^{-x^3}$, which verifies both the [differential equation](../../../../../differential-equation-split.md) and the [initial condition](../../../../../initial-condition.md).

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
