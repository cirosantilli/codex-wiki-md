<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Write $y=e^{-px}v$. Direct differentiation gives

$$
y''+2py'+p^2y=e^{-px}v''.
$$

The [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md) therefore has $v=A+Bx$. A [linearly independent](../../../../../linear-independence.md) pair of solutions is

$$
\boxed{y_1=e^{-px},\qquad y_2=xe^{-px}.}
$$

Their [Wronskian](../../../../../wronskian.md) is $e^{-2px}$, which never vanishes; the argument also includes $p=0$.

For the [inhomogeneous linear differential equation](../../../../../inhomogeneous-linear-differential-equation.md), the same substitution gives $v''=1$. Since $y(0)=0$ implies $v(0)=0$, and $y'(0)=0$ then implies $v'(0)=0$, integration gives $v=x^2/2$. Thus the required solution of the [initial value problem](../../../../../initial-value-problem.md) is

$$
\boxed{y(x)=\frac{x^2}{2}e^{-px}.}
$$

## ↑ Ancestors (11)

1. [2B](../2b.md)
2. [Section I](../section-i.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
