<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

For [complex differentiability at a point](../../../../../complex-differentiability-at-a-point.md), the derivative must have the same value along real and imaginary increments. Along real increments it equals $u_x+iv_x$, while along imaginary increments it equals $(u_y+iv_y)/i=v_y-iu_y$. Equating real and imaginary parts gives the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md)

$$
\boxed{u_x=v_y,\qquad u_y=-v_x}.
$$

For the given real part,

$$
u_x=\frac{y^2-x^2}{(x^2+y^2)^2},\qquad u_y=\frac{-2xy}{(x^2+y^2)^2}.
$$

Integrating the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) gives a [harmonic conjugate](../../../../../harmonic-conjugate.md)

$$
\boxed{v(x,y)=-\frac{y}{x^2+y^2}+C,\quad F(z)=\frac1z+iC,\quad \mathcal D=\mathbb C\setminus\{0\}},\qquad C\in\mathbb R.
$$

This [open set](../../../../../open-set.md) is open and connected; $F$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) there with derivative $-z^{-2}$. The origin must be excluded because the real part is undefined there. On this connected [open set](../../../../../open-set.md), any other [harmonic conjugate](../../../../../harmonic-conjugate.md) differs by a real constant: the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) make both partial derivatives of the difference zero.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
