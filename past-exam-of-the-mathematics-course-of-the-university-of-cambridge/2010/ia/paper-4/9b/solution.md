<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

For the [moment of inertia of a uniform solid sphere](../../../../../moment-of-inertia-of-a-uniform-solid-sphere.md), write the [mass density](../../../../../density.md) as $\rho=3m/(4\pi a^3)$. In spherical coordinates about the chosen axis, the squared perpendicular distance is $R^2\sin^2\vartheta$. The volume element is $R^2\sin\vartheta\,dR\,d\vartheta\,d\varphi$, so

$$
I=\rho\int_0^aR^4\,dR\int_0^\pi\sin^3\vartheta\,d\vartheta
\int_0^{2\pi}d\varphi
=\rho\frac{a^5}{5}\frac43\,2\pi
=\boxed{\frac25ma^2}.
$$

Take $0<\alpha<\pi/2$ and $\ell>0$, with a fixed plane. The [normal force](../../../../../normal-force.md) has magnitude $N=mg\cos\alpha$ and is perpendicular to the plane. On the perfectly smooth plane there is no friction. Both gravity and the [normal force](../../../../../normal-force.md) have zero [torque](../../../../../torque.md) about the marble's centre, so a marble released from rest does not rotate. The component of [Newton's second law](../../../../../newton-s-second-law.md) down the plane is $mA_1=mg\sin\alpha$, hence

$$
A_1=g\sin\alpha,\qquad
\boxed{t_1=\sqrt{\frac{2\ell}{g\sin\alpha}}}.
$$

The [normal force](../../../../../normal-force.md) does no work because the velocity is tangent to the plane. Gravity is conservative, so [mechanical energy](../../../../../mechanical-energy.md), the sum of translational [kinetic energy](../../../../../kinetic-energy.md) and [gravitational potential energy](../../../../../gravitational-energy.md), is conserved.

For [rolling without slipping](../../../../../rolling-without-slipping.md), let the [static friction](../../../../../static-friction.md) force have magnitude $f$, pointing up the plane. It supplies the [torque](../../../../../torque.md) that spins the marble while reducing its translational acceleration. If $\Omega$ is the [angular velocity](../../../../../angular-velocity.md) and $A_2$ the acceleration down the plane, the rolling constraint is $a\Omega=\dot s$, hence $a\dot\Omega=A_2$. The translation and rotation equations are

$$
mA_2=mg\sin\alpha-f,\qquad
fa=I\dot\Omega=\frac{I A_2}{a}.
$$

Thus $f=IA_2/a^2$ and

$$
A_2=\frac{g\sin\alpha}{1+I/(ma^2)}=\frac57g\sin\alpha,
\qquad f=\frac27mg\sin\alpha.
$$

These are the equations for [rolling acceleration with rotational inertia](../../../../../rolling-acceleration-with-rotational-inertia.md); the plane must be rough enough to supply this [static friction](../../../../../static-friction.md).

The point of contact is instantaneously at rest relative to the fixed plane, so [static friction](../../../../../static-friction.md) does no total work on the rolling marble. Equivalently, its translational power is $-f\dot s$ and its rotational power is $fa\Omega=f\dot s$, which cancel. The [normal force](../../../../../normal-force.md) also does no work. Consequently [mechanical energy](../../../../../mechanical-energy.md) is conserved here too, now with [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) included:

$$
\frac12m\dot s^2+\frac12I\Omega^2+mgH=\text{constant},
$$

where $H$ is the centre's height. No energy loss is implied by the presence of ideal [static friction](../../../../../static-friction.md). Constant acceleration from rest gives

$$
\boxed{t_2=\sqrt{\frac{14\ell}{5g\sin\alpha}},\qquad
\frac{t_1}{t_2}=\sqrt{\frac57}.}
$$

For the hollow marble, put $I=\lambda ma^2$ in the same equations. The smooth-plane time is unchanged, while the rolling acceleration becomes $g\sin\alpha/(1+\lambda)$. Therefore

$$
\boxed{t_2=\sqrt{\frac{2\ell(1+\lambda)}{g\sin\alpha}},\qquad
\frac{t_1}{t_2}=\frac1{\sqrt{1+\lambda}}.}
$$

This again assumes [rolling without slipping](../../../../../rolling-without-slipping.md) and enough [static friction](../../../../../static-friction.md); the ratio depends on the mass distribution through its [moment of inertia](../../../../../moment-of-inertia.md).

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
