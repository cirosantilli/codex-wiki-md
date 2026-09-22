<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $t=0$ be the start of deposition and $I_0=MR^2/2$ be the original [moment of inertia of a uniform disc](../../../moment-of-inertia-of-a-uniform-disc.md). Assume that all deposited sand sticks and remains at radius $r$, with negligible thickness and no losses. The sand's incoming [angular momentum](../../../angular-momentum.md) about the vertical axis is zero. Neither the bearing nor [gravity](../../../gravity.md) supplies an axial [torque](../../../torque.md), so [conservation of angular momentum](../../../conservation-of-angular-momentum.md) gives

$$
I(t)=I_0+\alpha r^2t,\qquad
I(t)\omega(t)=I_0\omega_0.
$$

Consequently the [angular velocity](../../../angular-velocity.md) and [angular acceleration](../../../angular-acceleration.md) are

$$
\boxed{\omega(t)=\frac{I_0\omega_0}{I_0+\alpha r^2t}
=\frac{MR^2\omega_0}{MR^2+2\alpha r^2t},}
\qquad
\boxed{\dot\omega(t)=-\frac{\alpha r^2I_0\omega_0}{(I_0+\alpha r^2t)^2}.}
$$

The [rotational kinetic energy](../../../rotational-kinetic-energy.md) is

$$
\boxed{K(t)=\frac12I(t)\omega(t)^2
=\frac{I_0^2\omega_0^2}{2(I_0+\alpha r^2t)}
=K(0)\frac{I_0}{I_0+\alpha r^2t}.}
$$

Thus, for $\alpha r^2>0$,

$$
\boxed{t_{1/2}=\frac{I_0}{\alpha r^2}=\frac{MR^2}{2\alpha r^2}.}
$$

This is [mass-loaded rotation](../../../mass-loaded-rotation.md): the sticking process dissipates [mechanical energy](../../../mechanical-energy.md) even though [angular momentum](../../../angular-momentum.md) is conserved. Indeed $\dot K=-\alpha r^2\omega^2/2$. If $r=0$ or $\alpha=0$, no additional axial [moment of inertia](../../../moment-of-inertia.md) is deposited and the nonzero initial [rotational kinetic energy](../../../rotational-kinetic-energy.md) never halves.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
