<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

[irrotational flow](../../../../../irrotational-flow.md) has $\nabla\times\mathbf v=0$, so locally $\mathbf v=\nabla\Phi$; the simply connected fluid domain here permits a globally single-valued [velocity potential](../../../../../velocity-potential.md). Incompressibility gives $\nabla\cdot\mathbf v=0$, hence **$\nabla^2\Phi=0$**. In a multiply connected domain, zero local [vorticity](../../../../../vorticity-split.md) alone would not rule out [circulation](../../../../../circulation-physics.md) and a multivalued potential.

Take $k>0$ so the disturbance decays at depth. Differentiating the given candidate potential yields

$$
v_x=h_0\omega\cos(\omega t)\cos(kx)e^{kz},\qquad v_y=0,\qquad v_z=h_0\omega\cos(\omega t)\sin(kx)e^{kz}.
$$

The $x$ and $z$ second derivatives of $\Phi$ cancel in the [Laplacian](../../../../../laplacian.md). At $z=0$, $v_z=h_0\omega\cos(\omega t)\sin(kx)=\partial_t Z$, so the linearized kinematic free-surface condition holds. This uses $kh_0\ll1$; advection of the displaced surface is higher order.

Since $\cos^2(kx)+\sin^2(kx)=1$, the local squared [speed](../../../../../speed.md) is $h_0^2\omega^2\cos^2(\omega t)e^{2kz}$. The depth integral is therefore

$$
T=\frac{\rho h_0^2\omega^2}{2}\cos^2(\omega t)\int_{-\infty}^0e^{2kz}\,dz=\boxed{\frac{\rho h_0^2\omega^2}{4k}\cos^2(\omega t).}
$$

It is independent of horizontal position; no further spatial average is needed for this [kinetic energy](../../../../../kinetic-energy.md). Replacing the upper boundary $Z$ by zero changes it only beyond quadratic order in [amplitude](../../../../../wave-amplitude.md).

Relative to the flat surface, the gravitational [energy](../../../../../energy-split.md) at each horizontal position changes by $\rho g\int_0^Z z\,dz=\rho gZ^2/2$. Averaging over one [wavelength](../../../../../wavelength.md) gives

$$
\boxed{\langle U\rangle_x=\frac{\rho gh_0^2}{4}\sin^2(\omega t).}
$$

The [energy of a deep-water standing gravity wave](../../../../../energy-of-a-deep-water-standing-gravity-wave.md), averaged over [wavelength](../../../../../wavelength.md), is $T+\langle U\rangle_x$ and must be constant for a free inviscid [standing wave](../../../../../standing-wave.md), which requires equal coefficients of the complementary squared sine and cosine:

$$
\boxed{\omega^2=gk.}
$$

As an independent check, the linearized dynamic [boundary condition](../../../../../boundary-condition.md) $\partial_t\Phi+gZ=0$ at $z=0$ gives exactly $g-\omega^2/k=0$. Infinite depth, negligible [surface tension](../../../../../surface-tension-split.md) and no dissipative forcing are part of this gravity-wave model.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
