<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First use the usual idealization of a grounded infinite [conducting plane](../../../../conducting-plane.md) at $z=0$, with the real [point charge](../../../../point-charge.md) $+q$ at $(0,0,d)$. The [method of images](../../../../method-of-images.md) replaces the metal, for purposes of calculating the exterior [electric field](../../../../electric-field-split.md), by an image charge $-q$ at $(0,0,-d)$. The exact [electric potential](../../../../electric-potential.md) in $z>0$ is

$$
V(\rho,z)=\frac{q}{4\pi\epsilon_0}\left[\frac1{\sqrt{\rho^2+(z-d)^2}}-\frac1{\sqrt{\rho^2+(z+d)^2}}\right].
$$

It vanishes on the plane, and the [uniqueness theorem for the electrostatic potential](../../../../uniqueness-theorem-for-the-electrostatic-potential.md) identifies it with the physical exterior solution. The tangential [electric field](../../../../electric-field-split.md) cancels on the plane, while the normal components add:

$$
\boxed{\mathbf E(\rho,0^+)=-\frac{qd}{2\pi\epsilon_0(\rho^2+d^2)^{3/2}}\hat{\mathbf z}.}
$$

The [electric field](../../../../electric-field-split.md) inside the [conductor](../../../../electrical-conductor.md) is zero, so the [electrostatic boundary condition](../../../../electrostatic-boundary-conditions-at-a-conductor.md) gives $\sigma=\epsilon_0E_z(0^+)$. Integrating the [surface charge density](../../../../surface-charge-density.md) over the facing plane yields

$$
Q_{\rm face}=\int_0^\infty\frac{-qd}{2\pi(\rho^2+d^2)^{3/2}}2\pi\rho\,d\rho=-qd\left[-\frac1{\sqrt{\rho^2+d^2}}\right]_0^\infty,\qquad \boxed{Q_{\rm face}=-q.}
$$

The exact image expression is essential near the charge: using the far-field [electric dipole](../../../../electric-dipole.md) approximation at $\rho$ comparable with $d$ would be invalid.

**Electrical boundary condition.** The source does not specify grounding or the initial total [electric charge](../../../../electric-charge-split.md) of the slab. The boxed total is the grounded infinite-plane answer and the large-plane approximation to the charge on its nearby face. An initially neutral, finite, electrically isolated slab retains zero _total_ [electric charge](../../../../electric-charge-split.md); an approximately $-q$ accumulation near the real charge is then balanced by approximately $+q$ on its remote face and edges. This gives a concrete counterexample to interpreting $-q$ as the unconditional total charge of every large metal slab. The local image formula assumes the infinite-plane limit with no applied background [electric field](../../../../electric-field-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
