<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a fixed [sphere](../../../../../../sphere.md) of radius $R$ in an unbounded incompressible inviscid fluid, with uniform [velocity](../../../../../../velocity.md) $U\mathbf e_z$ at infinity. Assume [irrotational flow](../../../../../../irrotational-flow.md), so $\mathbf v=\nabla\phi$ and [incompressibility](../../../../../../incompressible-flow.md) gives $\nabla^2\phi=0$. Axisymmetry and the dipolar angular dependence of the far field suggest

$$
\phi=(Ar+B/r^2)\cos\theta.
$$

Matching the far field gives $A=U$. The no-penetration condition $v_r(R)=0$ then gives $B=UR^3/2$. Thus

$$
\boxed{\phi=U\left(r+\frac{R^3}{2r^2}\right)\cos\theta,}
$$



$$
v_r=U\left(1-\frac{R^3}{r^3}\right)\cos\theta,\qquad
v_\theta=-U\left(1+\frac{R^3}{2r^3}\right)\sin\theta.
$$

The surface has [stagnation points](../../../../../../stagnation-point.md) at its front and rear poles, while the equatorial speed is $3U/2$. Fluid slips tangentially past the [sphere](../../../../../../sphere.md); imposing a no-slip condition would contradict this inviscid potential-flow model.

With gravity omitted or the hydrostatic [pressure](../../../../../../pressure-split.md) subtracted, steady Bernoulli gives

$$
p+\frac12\rho v^2=p_\infty+\frac12\rho U^2.
$$

At the surface,

$$
\boxed{p(R,\theta)=p_\infty+\frac12\rho U^2
\left(1-\frac94\sin^2\theta\right).}
$$

The front–rear symmetry makes the [integral](../../../../../../integral-split.md) of [pressure](../../../../../../pressure-split.md) [force](../../../../../../force-split.md) along the flow vanish: terms proportional to $\cos\theta$ integrate to zero over the [sphere](../../../../../../sphere.md). This is [D'Alembert's paradox](../../../../../../d-alembert-s-paradox.md), not a prediction that real spheres have no [drag](../../../../../../drag-physics.md). [Viscosity](../../../../../../dynamic-viscosity-split.md) creates [boundary layers](../../../../../../boundary-layer.md); separation and a wake break the fore–aft symmetry. [Potential flow](../../../../../../potential-flow.md) remains valuable for the outer [velocity](../../../../../../velocity.md) field when viscous regions are thin, but it cannot supply their [drag](../../../../../../drag-physics.md) by itself.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
