<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $I=I_1=I_2$. The third of the [Euler equations for a torque-free rigid body](../../../../../../euler-equations-for-a-torque-free-rigid-body.md) gives $I_3\dot\omega_3=0$, so $\omega_3$ is constant. Define $\Omega=(I_3-I)\omega_3/I$. The first two [Euler equations for a torque-free rigid body](../../../../../../euler-equations-for-a-torque-free-rigid-body.md) become

$$
\dot\omega_1=-\Omega\omega_2,\qquad\dot\omega_2=\Omega\omega_1,
$$

so $\omega_1+i\omega_2=C e^{i\Omega t}$. Since the body-frame [angular momentum](../../../../../../angular-momentum.md) has components $(I\omega_1,I\omega_2,I_3\omega_3)$, its transverse components rotate at $\Omega$ while its axial component is constant. Substitution of the [principal moments of inertia](../../../../../../principal-moment-of-inertia.md) gives

$$
\boxed{\Omega=\frac{3a^2-h^2}{3a^2+h^2}\,\omega_3.}
$$

This is precession relative to the body axes; the [angular momentum](../../../../../../angular-momentum.md) is constant in an inertial frame. If $h^2=3a^2$, the rate is zero even when $\omega_3\ne0$. If the transverse components vanish, the precession cone degenerates to its axis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
