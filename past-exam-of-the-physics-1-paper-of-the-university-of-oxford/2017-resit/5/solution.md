<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Treat the ladder as a uniform slender [rigid body](../../../rigid-body-dynamics-split.md). While both contacts remain imposed, its [centre of mass](../../../center-of-mass.md) is $(l\sin\theta,l\cos\theta)$, with [speed](../../../speed.md) $l|\dot\theta|$. Its central [moment of inertia](../../../moment-of-inertia.md) is $m(2l)^2/12=ml^2/3$. Adding translational and rotational [kinetic energy](../../../kinetic-energy.md) gives

$$
K=\frac12ml^2\dot\theta^2+\frac12\frac{ml^2}{3}\dot\theta^2
=\frac23ml^2\dot\theta^2.
$$

Taking the floor as zero [gravitational potential energy](../../../gravitational-energy.md), the [Lagrangian](../../../lagrangian.md), [conjugate momentum](../../../canonical-momentum.md) and [Euler-Lagrange equation](../../../euler-lagrange-equation.md) are

$$
\boxed{L=\frac23ml^2\dot\theta^2-mgl\cos\theta,\qquad
p_\theta=\frac43ml^2\dot\theta,\qquad
\ddot\theta=\frac{3g}{4l}\sin\theta.}
$$

The positive sign is appropriate: gravity increases the angle from the vertical. These are the constrained equations of a [frictionless sliding ladder](../../../frictionless-sliding-ladder.md). Real wall contact is unilateral: a wall cannot pull the ladder. Once the computed [normal force](../../../normal-force.md) would become negative, the two-contact model ceases to apply; the question explicitly assumes that contact persists.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
