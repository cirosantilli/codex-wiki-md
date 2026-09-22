<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The steady [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) are

$$
\rho(u\cdot\nabla)u=-\nabla p-\nabla\chi.
$$

Taking the [scalar](../../../../../scalar.md) product with $u$ and using

$$
u\cdot(u\cdot\nabla u)
=u\cdot\nabla\left(\frac12|u|^2\right)
$$

gives

$$
u\cdot\nabla
\left(\frac12\rho|u|^2+p+\chi\right)=0.
$$

Thus

$$
\boxed{u\cdot\nabla H=0}.
$$

The [Bernoulli function](../../../../../bernoulli-function.md) $H$ is constant along each [streamline](../../../../../streamline.md): fluid particles in steady flow exchange [pressure](../../../../../pressure.md), kinetic, and [potential energy](../../../../../potential-energy.md) without changing their total mechanical energy density.

Let $y(t)$ be the downward displacement of the free surface from its initial level, and let $U$ be the speed in the tube. Conservation of volume gives

$$
aU=A\dot y.
$$

The free surface and the outlet are both at atmospheric [pressure](../../../../../pressure.md), and their vertical separation is $H+h_0-y$. Applying the [Bernoulli equation](../../../../../bernoulli-equation.md) between them, while retaining the small free-surface speed, gives

$$
\frac12\left(U^2-\dot y^2\right)
=g(H+h_0-y).
$$

Therefore

$$
\dot y=
\sqrt{\frac{2g(H+h_0-y)}{A^2/a^2-1}}.
$$

The surface reaches the upper tube end when $y=h_0$. Hence the [draining time of a uniform tank through a siphon](../../../../../draining-time-of-a-uniform-tank-through-a-siphon.md) is

$$
\begin{aligned}
t
&=\sqrt{\frac{A^2/a^2-1}{2g}}
\int_0^{h_0}\frac{dy}{\sqrt{H+h_0-y}}\\
&=\boxed{
\sqrt{2}\left(\frac{A^2}{a^2}-1\right)^{1/2}
\frac{\sqrt{H+h_0}-\sqrt H}{\sqrt g}}.
\end{aligned}
$$

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
