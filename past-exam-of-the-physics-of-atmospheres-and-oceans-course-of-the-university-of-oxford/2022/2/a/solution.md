<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [pressure-linear grey opacity](../../../../pressure-linear-grey-opacity.md) model interprets $\kappa$ as a [mass absorption coefficient](../../../../mass-absorption-coefficient.md). If it is instead a molecular [absorption cross section](../../../../absorption-cross-section.md), replace $\kappa$ below by that cross section divided by molecular [mass](../../../../mass.md). Assume a plane-parallel [atmosphere](../../../../atmosphere.md), [hydrostatic balance](../../../../hydrostatic-balance.md), local [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md), and thermal [absorption](../../../../absorption-electromagnetic-radiation.md) and emission without [scattering of light](../../../../scattering-of-light.md). With height $z$ increasing upwards,

$$
d\tau=\kappa\rho\,dz=-\frac{\kappa}{g}\,dp.
$$

Integrating upwards from the surface gives

$$
\tau(p)=\frac{\kappa_s}{gp_s}\int_p^{p_s}p'\,dp'
=\frac{\kappa_sp_s}{2g}\left[1-\left(\frac p{p_s}\right)^2\right].
$$

Thus

$$
\boxed{\tau_\infty=\frac{\kappa_sp_s}{2g},\qquad
\tau(p)=\tau_\infty[1-(p/p_s)^2].}
$$

The vertical [optical depth](../../../../optical-depth.md) is dimensionless. The [atmosphere](../../../../atmosphere.md) is optically thick when $\tau_\infty\gg1$ and optically thin when $\tau_\infty\ll1$. A ray with zenith-angle cosine $\mu$ sees [optical depth](../../../../optical-depth.md) $\tau_\infty/\mu$, so even a vertically thin layer can be opaque along a sufficiently grazing ray.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
