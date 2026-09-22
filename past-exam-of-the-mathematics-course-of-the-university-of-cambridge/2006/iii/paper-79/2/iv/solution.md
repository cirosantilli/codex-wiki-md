<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a [Burgers vortex](../../../../../../burgers-vortex.md), integrating the axial [vorticity](../../../../../../vorticity.md) gives the azimuthal [velocity](../../../../../../velocity.md):

$$
u_\theta(r)=\frac\Gamma{2\pi r}(1-e^{-r^2/\delta^2}),\qquad \delta^2=\frac{4\nu}{\alpha}.
$$

The swirl contribution to the [viscous dissipation](../../../../../../viscous-dissipation.md) per unit length and per unit density is

$$
\mathcal D_\theta=\nu\int_0^\infty
\left(\frac{du_\theta}{dr}-\frac{u_\theta}{r}\right)^2 2\pi r\,dr
=\nu\int_0^\infty\omega_z^2\,2\pi r\,dr.
$$

For the equality, expand the two squares using $\omega_z=u_\theta'+u_\theta/r$; their integrated difference is proportional to $[u_\theta^2]_0^\infty$, which vanishes. Substitution of the Gaussian [vorticity](../../../../../../vorticity.md) profile gives

$$
\mathcal D_\theta
=\frac{2\nu\Gamma^2}{\pi\delta^4}\int_0^\infty r e^{-2r^2/\delta^2}\,dr
=\frac{\nu\Gamma^2}{2\pi\delta^2}
=\boxed{\frac{\alpha\Gamma^2}{8\pi}}.
$$

This [excess dissipation of a Burgers vortex](../../../../../../excess-dissipation-of-a-burgers-vortex.md) is independent of [kinematic viscosity](../../../../../../kinematic-viscosity.md) at fixed strain $\alpha$ and [circulation](../../../../../../circulation-physics.md) $\Gamma$. Multiply by the [mass density](../../../../../../density.md) if a dimensional power per length is wanted.

The qualification "excess" matters. The imposed uniform strain itself has [viscous dissipation](../../../../../../viscous-dissipation.md) density $3\nu\alpha^2$ per unit mass, so its integral over an infinite cross-section diverges. One must subtract that background or restrict to a finite cross-section. In a core-sized area, its contribution is of order $\nu^2\alpha$, smaller than the swirl contribution by order $(\nu/\Gamma)^2$ as $\Gamma/\nu\to\infty$.

Meanwhile $\delta\propto\nu^{1/2}$ shrinks and the central [vorticity](../../../../../../vorticity.md) $\Gamma/(\pi\delta^2)$ grows. The finite dissipation becomes concentrated in a narrow tube: a useful local model of [internal intermittency](../../../../../../internal-intermittency.md) and the [turbulent dissipation anomaly](../../../../../../turbulent-dissipation-anomaly.md), though not a proof that an entire turbulent flow consists of such vortices.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
