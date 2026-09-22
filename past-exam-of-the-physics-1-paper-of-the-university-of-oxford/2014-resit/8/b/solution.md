<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Allowing azimuthal motion makes the endpoint speed satisfy $v^2=l^2(\dot\theta^2+\sin^2\theta\,\dot\varphi^2)$. The light-rod [spherical pendulum](../../../../spherical-pendulum.md) therefore has

$$
\boxed{\mathcal L=\frac12ml^2\left(\dot\theta^2+\sin^2\theta\,\dot\varphi^2\right)+mgl\cos\theta.}
$$

The azimuth $\varphi$ is a [cyclic coordinate](../../../../cyclic-coordinate.md), since the [Lagrangian](../../../../lagrangian.md) is independent of it. Its conjugate [canonical momentum](../../../../canonical-momentum.md) is the conserved vertical [angular momentum](../../../../angular-momentum.md):

$$
\boxed{p_\varphi=ml^2\sin^2\theta\,\dot\varphi=J_z=\text{constant}.}
$$

For a finite uniform rod, replace $ml^2$ by $I$ and $mgl$ by $A$ from [i](../a/i.md). The same azimuthal symmetry then gives $p_\varphi=I\sin^2\theta\,\dot\varphi$.

The [Hamiltonian](../../../../hamiltonian.md) is the [Legendre transform](../../../../convex-conjugate.md) of this [Lagrangian](../../../../lagrangian.md). With $p_\theta=I\dot\theta$,

$$
H=\frac{p_\theta^2}{2I}+\frac{p_\varphi^2}{2I\sin^2\theta}-A\cos\theta
=\frac I2\left(\dot\theta^2+\sin^2\theta\,\dot\varphi^2\right)-A\cos\theta.
$$

There is no explicit time dependence, so $dH/dt=\partial H/\partial t=0$. Here $H$ also equals the total mechanical [energy](../../../../energy-split.md): the constraint is stationary, the [kinetic energy](../../../../kinetic-energy.md) is quadratic in generalized velocities, and gravity is conservative. The apparent singularity of the momentum expression at $\sin\theta=0$ is a spherical-coordinate singularity; trajectories reaching a pole must be described consistently, and nonzero $J_z$ prevents reaching it at finite [energy](../../../../energy-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2014 resit](../../../2014-resit-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
