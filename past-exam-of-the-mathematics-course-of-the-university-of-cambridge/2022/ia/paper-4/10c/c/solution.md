<h1 id="10c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Neglecting terms of order $\Omega^2$ and linearizing in $\theta$ gives

$$
R\ddot\theta=-g\theta-2\Omega\dot y,
\qquad
\ddot y=2\Omega R\dot\theta.
$$

The second equation and the initial data imply

$$
\dot y=2\Omega R(\theta-\theta_0).
$$

Its contribution to the first equation is of order $\Omega^2$, so the retained equation is

$$
\ddot\theta+\frac gR\theta=0.
$$

Thus

$$
\boxed{\theta(t)=\theta_0\cos(\omega_0t)},
\qquad
\boxed{\omega_0=\sqrt{\frac gR}}.
$$

Integrating the associated $y$ velocity and using $y(0)=0$ gives

$$
\boxed{
y(t)=2\Omega R\theta_0
\left(\frac{\sin(\omega_0t)}{\omega_0}-t\right)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10C](../../10c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
