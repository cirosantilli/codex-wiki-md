<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use Cartesian coordinates along the edges from the pivot. With [surface mass density](../../../projected-surface-mass-density.md) $M/L^2$, the [moment of inertia](../../../moment-of-inertia.md) is

$$
I_O=\frac M{L^2}\int_0^L\!\int_0^L(x^2+y^2)\,dx\,dy
=\boxed{\frac23ML^2}.
$$

Equivalently, the [moment of inertia of a uniform square plate](../../../moment-of-inertia-of-a-uniform-square-plate.md) about its central perpendicular axis is $ML^2/6$, and the [parallel axis theorem](../../../parallel-axis-theorem.md) adds $M(L/\sqrt2)^2$.

The source figure measures $\theta$ from the upward vertical to $OC$, with $OC=L/\sqrt2$. The centre's height above the pivot is $(L/\sqrt2)\cos\theta$. The smooth fixed pivot does no work. [Conservation of energy](../../../conservation-of-energy.md), with the initially upright configuration as reference, gives

$$
\frac12I_O\dot\theta^2
=\frac{MgL}{\sqrt2}(1-\cos\theta),\qquad
\boxed{|\dot\theta|=\sqrt{\frac{3g}{\sqrt2L}(1-\cos\theta)}.}
$$

For rotation in the positive $\theta$ direction on the first descent, take the positive root. Its equivalent form is $\dot\theta=\sqrt{3\sqrt2g/L}\sin(\theta/2)$ for $0<\theta<\pi$.

Strictly, release from rest at a small angle $\theta_0$ replaces $1-\cos\theta$ by $\cos\theta_0-\cos\theta$. The displayed result is the $\theta_0\to0$ limiting [energy](../../../energy-split.md) relation. Exactly upright and exactly at rest is an unstable [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md); without a perturbation it stays there. This distinction prevents the infinitesimal displacement convention from being mistaken for spontaneous motion.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
