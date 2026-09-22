<h1 id="15e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Lagrange top](../../../../../../lagrange-top.md) is a [rigid body](../../../../../../rigid-body-dynamics.md) that is symmetric about a principal axis, has a point on that axis fixed in space, and has its [center of mass](../../../../../../center-of-mass.md) on the same axis while gravity acts uniformly. Here $I_1=I_2$ is the transverse [principal moment of inertia](../../../../../../principal-moment-of-inertia.md) about the fixed point, $I_3$ is the moment about the symmetry axis, $M$ is the total mass, and $l$ is the distance from the fixed point to the center of mass.

The [Euler angles for a symmetric top](../../../../../../euler-angles-for-a-symmetric-top.md) use $\theta$ for inclination, $\phi$ for precession, and $\psi$ for spin about the body axis. Since $\psi$ is a [cyclic coordinate](../../../../../../cyclic-coordinate.md), its [generalized momentum](../../../../../../generalized-momentum.md)

$$
\boxed{p_\psi=I_3(\dot\psi+\dot\phi\cos\theta)}
$$

is conserved. The coordinate $\phi$ is also cyclic, so

$$
\boxed{p_\phi=I_1\dot\phi\sin^2\theta+p_\psi\cos\theta}
$$

is a second integral. Finally, the Lagrangian has no explicit time dependence, and [conservation of energy from time-translation invariance](../../../../../../conservation-of-energy-from-time-translation-invariance.md) gives the independent integral

$$
\boxed{E=\frac12I_1(\dot\theta^2+\dot\phi^2\sin^2\theta)
+\frac{p_\psi^2}{2I_3}+Mgl\cos\theta.}
$$

For steady precession set $\theta$ constant and $\dot\phi=\Omega$ constant. The $\theta$ [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md), with $0<\theta<\pi/2$, reduces after division by $\sin\theta$ to

$$
I_1\Omega^2\cos\theta-p_\psi\Omega+Mgl=0.
$$

This quadratic has a real precession rate precisely when its [quadratic discriminant](../../../../../../quadratic-discriminant.md) is nonnegative. Hence [Steady precession of a Lagrange top](../../../../../../steady-precession-of-a-lagrange-top.md) is possible if and only if

$$
\boxed{p_\psi^2\geq4MglI_1\cos\theta.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15E](../../15e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
