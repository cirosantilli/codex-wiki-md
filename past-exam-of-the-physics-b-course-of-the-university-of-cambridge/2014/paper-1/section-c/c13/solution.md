<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

In [irrotational flow](../../../../../irrotational-flow.md), the [velocity](../../../../../velocity.md) has a [velocity potential](../../../../../velocity-potential.md) locally, and globally in a simply connected flow domain. [incompressibility](../../../../../incompressible-flow.md) then gives $\nabla\cdot\mathbf v=\nabla^2\Phi=0$. For a sphere moving at [speed](../../../../../speed.md) $U$ along $z$ through fluid at rest far away, the [potential of a translating sphere](../../../../../potential-of-a-translating-sphere.md) is a decaying axisymmetric dipole. Its solution and its impermeability condition give

$$
\Phi=\frac{\beta\cos\theta}{r^2},\quad
\left.\partial_r\Phi\right|_a=U\cos\theta,
\qquad\boxed{\beta=-\frac12Ua^3.}
$$

These are laboratory fluid [velocities](../../../../../velocity.md) expressed relative to a moving origin. A [velocity](../../../../../velocity.md) field measured in the sphere-rest frame instead requires adding $-Ur\cos\theta$ to the potential.

**The vector identity printed in the PDF has its signs reversed.** The product rule gives the consistent identity $v^2=\nabla\cdot(\Phi\mathbf v)-\Phi\nabla\cdot\mathbf v$. With outward normal of the exterior fluid equal to $-\hat r$ at the sphere, the [divergence theorem](../../../../../divergence-theorem.md) yields

$$
\int_{r>a}v^2\,dV=\int_{r=a}\Phi(-v_r)\,dS
=\frac{U^2a}{2}\int\cos^2\theta\,dS=\frac{2\pi a^3U^2}{3}.
$$

The integral at infinity vanishes. Hence

$$
K_f=\frac{\pi\rho_0a^3U^2}{3}=\tfrac12m_aU^2,
\qquad\boxed{m_a=\frac{2\pi\rho_0a^3}{3},\quad m_{\rm eff}=\frac{4\pi a^3}{3}(\rho+\rho_0/2).}
$$

This [added mass of a sphere](../../../../../added-mass-of-a-sphere.md) is half the displaced fluid [mass](../../../../../mass.md). For a spring of unchanged stiffness, [buoyancy](../../../../../buoyancy.md) only shifts the static equilibrium. Its [oscillation frequency with fluid added mass](../../../../../oscillation-frequency-with-fluid-added-mass.md) is

$$
\boxed{\omega_s'=\omega_s\sqrt{\frac\rho{\rho+\rho_0/2}}.}
$$

For a small-angle [simple pendulum](../../../../../simple-pendulum-split.md), [buoyancy](../../../../../buoyancy.md) also reduces restoring [torque](../../../../../torque.md) from $mg\ell\theta$ to $(m-\rho_0V)g\ell\theta$, while the inertia is $(m+m_a)\ell^2$. Thus

$$
\boxed{\omega_p'=\omega_p\sqrt{\frac{\rho-\rho_0}{\rho+\rho_0/2}}.}
$$

The downward equilibrium is stable only for $\rho>\rho_0$. The ideal results assume unbounded fluid, negligible [viscosity](../../../../../dynamic-viscosity-split.md), small excursions, and no important free-surface or container corrections.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
