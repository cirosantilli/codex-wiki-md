<h1 id="37c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X^\mu(\tau)$ be the worldline, $u^\mu=dX^\mu/d\tau$ its [four-velocity](../../../../../../four-velocity.md), and

$$
\Omega=\frac{qB_0}{m}.
$$

The [relativistic Lorentz force](../../../../../../relativistic-lorentz-force.md) in the constant background is

$$
\frac{du^\mu}{d\tau}
=\frac qm F^\mu{}_\nu u^\nu.
$$

Because $F^3=0$, its exponential terminates:

$$
u(\tau)
=\exp\left(\frac qmF\tau\right)u(0)
=\left[
I+\frac qmF\tau
+\frac12\left(\frac qmF\tau\right)^2
\right]u(0).
$$

The particle starts from rest, so

$$
u(0)=(c,0,0,0).
$$

Using the matrix from part (c) gives

$$
u^0=c\left(1+\frac12\Omega^2\tau^2\right),
\qquad
u^1=c\Omega\tau,
\qquad
u^2=-\frac c2\Omega^2\tau^2,
\qquad
u^3=0.
$$

Integrating from the origin and using $X^0=ct$ yields the parametric trajectory

$$
\boxed{
\begin{aligned}
t(\tau)&=\tau+\frac{\Omega^2\tau^3}{6},\\
x(\tau)&=\frac{c\Omega\tau^2}{2},\\
y(\tau)&=-\frac{c\Omega^2\tau^3}{6},\\
z(\tau)&=0.
\end{aligned}}
$$

This is the [relativistic trajectory in a constant null crossed field](../../../../../../relativistic-trajectory-in-a-constant-null-crossed-field.md). The real cubic relation for $t(\tau)$ is strictly increasing, so it determines $\tau$ uniquely as a function of coordinate time if an explicit $\mathbf x(t)$ is desired.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [37C](../../37c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
