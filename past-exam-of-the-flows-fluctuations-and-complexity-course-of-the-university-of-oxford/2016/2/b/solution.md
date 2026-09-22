<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the cylinder radius be $a$, with $h/a\ll1$ and slowly varying thickness. Arc length is $s=a\theta$, with increasing $\theta$ following the upward-moving surface at the right-hand side. Gravity has tangential component $-g\cos\theta$. In the leading thin-film balance, normal viscous gradients dominate tangential ones, curvature corrections are small, and the longitudinal hydrostatic-pressure gradient is smaller by the aspect ratio. Neglect capillary-pressure gradients and imposed gas shear. The tangential Stokes balance is then

$$
\boxed{\nu\,\partial_z^2u=g\cos\theta.}
$$

These assumptions also require that inertia and curvature effects from rotation remain small on the thin-film scale; an arbitrary high-speed coating need not obey this equation.

No-slip at the solid wall and negligible [shear stress](../../../../shear-stress.md) at the [free surface](../../../../free-surface.md) give

$$
u(\theta,0)=U,\qquad \left.\partial_zu\right|_{z=h}=0.
$$

Twice integrating the constant normal forcing determines the two integration constants:

$$
\boxed{u(\theta,z)=U+\frac g\nu\left(\frac{z^2}{2}-zh\right)\cos\theta.}
$$

The profile is most strongly retarded by gravity on the ascending side. The surface [velocity](../../../../velocity.md) is $U-gh^2\cos\theta/(2\nu)$, not generally equal to the wall speed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
