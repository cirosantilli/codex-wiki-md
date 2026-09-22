<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [rotating-hoop bead](../../../../../../rotating-hoop-bead.md) problem, use a signed angle in the hoop plane from the downward vertical. The gravitational [potential energy](../../../../../../potential-energy.md) is $-mga\cos\theta$, the rotating-frame [speed](../../../../../../speed.md) is $a\dot\theta$, and the distance from the rotation axis is $a\sin\theta$. The [centrifugal potential](../../../../../../centrifugal-potential.md) gives

$$
E=\frac{ma^2}{2}\dot\theta^2-mga\cos\theta-\frac{m\omega^2a^2}{2}\sin^2\theta.
$$

Gravity is stationary in these rotating coordinates, and the frictionless constraint does no work. Projecting the rotating equation along the hoop, or differentiating its effective potential in the one-dimensional [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md), gives

$$
\boxed{\ddot\theta+\left(\frac ga-\omega^2\cos\theta\right)\sin\theta=0.}
$$

If $\omega^2>g/a$, the two off-axis positions are

$$
\boxed{\theta=\pm\theta_0,\qquad\theta_0=\arccos\left(\frac{g}{a\omega^2}\right).}
$$

Their unsigned angle to the downward vertical is the same; they lie on opposite sides of the hoop. The second [derivative](../../../../../../derivative.md) of the effective potential there is $m\omega^2a^2\sin^2\theta_0>0$. Equivalently, writing $\theta=\theta_0+\delta$ gives to first order

$$
\ddot\delta+\omega^2\sin^2\theta_0\,\delta=0.
$$

The same holds at $-\theta_0$. Thus **both equilibria are stable**, with small-oscillation angular frequency $|\omega|\sin\theta_0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
