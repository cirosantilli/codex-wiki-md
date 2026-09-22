<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

Let $\rho=3m/(4\pi R_0^3)$ be the uniform [mass density](../../../../../density.md). In [spherical coordinates](../../../../../spherical-coordinate-system.md) $(r,\vartheta,\phi)$ with the chosen diameter as polar axis, the squared perpendicular distance to that axis is $r^2\sin^2\vartheta$. The [moment of inertia](../../../../../moment-of-inertia.md) is therefore

$$
I=\rho\int_0^{R_0}r^4\,dr\int_0^\pi\sin^3\vartheta\,d\vartheta\int_0^{2\pi}d\phi
=\frac{8\pi\rho R_0^5}{15}=\boxed{\frac25mR_0^2}.
$$

This derives the [moment of inertia of a uniform solid sphere](../../../../../moment-of-inertia-of-a-uniform-solid-sphere.md) about any central axis by [spherical symmetry](../../../../../spherical-symmetry.md).

Put $a=R_1-R_0$. The [center of mass](../../../../../center-of-mass.md) follows the circle of radius $a$, with [position](../../../../../position.md) $\mathbf r_C=a(\sin\theta,-\cos\theta)$. Let $\mathbf e_r=(\sin\theta,-\cos\theta)$ and $\mathbf e_\theta=(\cos\theta,\sin\theta)$. Its [velocity](../../../../../velocity.md) is $a\dot\theta\mathbf e_\theta$, and the contact point is displaced from the [center of mass](../../../../../center-of-mass.md) by $R_0\mathbf e_r$. With positive spin [angular velocity](../../../../../angular-velocity.md) $\Omega_s$ counterclockwise, its contact-point [velocity](../../../../../velocity.md) is

$$
\mathbf v_{\rm contact}=a\dot\theta\mathbf e_\theta+\Omega_s\mathbf e_z\times R_0\mathbf e_r
=(a\dot\theta+R_0\Omega_s)\mathbf e_\theta.
$$

The cylinder is fixed, so [rolling without slipping](../../../../../rolling-without-slipping.md) requires this [velocity](../../../../../velocity.md) to vanish. Consequently $\Omega_s=-a\dot\theta/R_0$. If instead the spin angle $\psi$ is positive clockwise, opposite to increasing $\theta$, then the printed positive-coefficient convention is

$$
\boxed{\dot\psi=\frac{R_1-R_0}{R_0}\dot\theta.}
$$

The spin and orbital rotation have opposite directions when both are measured about the same oriented axis; the [angular speed](../../../../../angular-speed.md) is $a|\dot\theta|/R_0$. This specifies the sign convention in the printed expression.

The instantaneous contact point is at rest, so the [normal reaction](../../../../../normal-force.md) and [static friction](../../../../../static-friction.md) do no work. [Conservation of energy](../../../../../conservation-of-energy.md) equates the loss of [gravitational potential energy](../../../../../gravitational-energy.md) from release to the total [kinetic energy](../../../../../kinetic-energy.md):

$$
mg a(\cos\theta-\cos\alpha)=\frac12ma^2\dot\theta^2+\frac12I\left(\frac a{R_0}\dot\theta\right)^2
=\frac7{10}ma^2\dot\theta^2.
$$

On the descent from $0<\alpha<\pi/2$, $\theta$ decreases, so

$$
\dot\theta=-\sqrt{\frac{10g}{7a}(\cos\theta-\cos\alpha)}.
$$

Integrating $dt=-d\theta/|\dot\theta|$ from release to the bottom gives

$$
\boxed{T_R=\sqrt{\frac{7(R_1-R_0)}{10g}}\int_0^\alpha\frac{d\theta}{\sqrt{\cos\theta-\cos\alpha}}.}
$$

The integral is finite: at the release point its denominator is asymptotic to $\sqrt{\sin\alpha\,(\alpha-\theta)}$. Contact is maintained, since the inward radial [equation of motion](../../../../../equation-of-motion.md) gives the positive [normal reaction](../../../../../normal-force.md) $N=m(g\cos\theta+a\dot\theta^2)$ throughout this range.

For frictionless sliding, the [normal reaction](../../../../../normal-force.md) passes through the sphere's centre and produces no [torque](../../../../../torque.md); [Newtonian gravity](../../../../../gravitational-acceleration.md) also exerts no central [torque](../../../../../torque.md). With initial zero spin, the sphere remains nonrotating. All the lost [gravitational potential energy](../../../../../gravitational-energy.md) becomes translational [kinetic energy](../../../../../kinetic-energy.md), so

$$
\frac12ma^2\dot\theta^2=mga(\cos\theta-\cos\alpha),\qquad
\boxed{T_S=\sqrt{\frac{R_1-R_0}{2g}}\int_0^\alpha\frac{d\theta}{\sqrt{\cos\theta-\cos\alpha}}=\sqrt{\frac57}\,T_R.}
$$

A hollow spherical shell of the same [mass](../../../../../mass.md) and radius places its material farther from the centre, giving a larger [moment of inertia](../../../../../moment-of-inertia.md). Under [rolling without slipping](../../../../../rolling-without-slipping.md), a given centre [speed](../../../../../speed.md) therefore requires more rotational [kinetic energy](../../../../../kinetic-energy.md); the same gravitational drop yields a smaller [speed](../../../../../speed.md). **Replacing the solid sphere by a hollow shell increases $T_R$ and leaves $T_S$ unchanged.** The sliding case remains nonrotating and has the same [center of mass](../../../../../center-of-mass.md) path and gravitational drop. This is the general comparison for [rolling inside a fixed circular cylinder](../../../../../rolling-inside-a-fixed-circular-cylinder.md).

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
