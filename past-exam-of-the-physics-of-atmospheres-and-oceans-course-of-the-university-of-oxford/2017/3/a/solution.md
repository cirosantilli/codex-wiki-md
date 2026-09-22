<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put the rigid lid at $z=0$, the interface at $z=-h(x,y,t)$ and $\rho_1=\rho_0-\Delta\rho$. Assume [hydrostatic vertical balance](../../../../hydrostatic-equilibrium.md) and a resting deep layer. Its [pressure](../../../../pressure-split.md) is $p_2=C-\rho_0gz$, with horizontally uniform $C$. [Pressure](../../../../pressure-split.md) continuity at the interface then fixes the upper-layer [pressure](../../../../pressure-split.md):

$$
p_1=C+\rho_0gh-\rho_1g(z+h)
=C-\rho_1gz+\Delta\rho\,gh.
$$

Hence its [horizontal pressure gradient](../../../../gradient.md) at fixed $z$ is $\nabla_hp_1=\Delta\rho\,g\nabla_hh$, independent of depth. Taking the horizontal momentum equation and a vertically uniform upper-layer velocity gives

$$
\boxed{\frac{D\mathbf u}{Dt}+f\mathbf k\times\mathbf u+g'\nabla_hh=0,
\qquad g'=g\frac{\Delta\rho}{\rho_1}\simeq g\frac{\Delta\rho}{\rho_0}.}
$$

The exact [density](../../../../density.md) denominator for upper-layer acceleration is $\rho_1$; the familiar $\rho_0$ denominator is the small-density-contrast [Boussinesq approximation](../../../../boussinesq-approximation.md). The restoring [pressure](../../../../pressure-split.md) is weaker than for a free surface because only the [density](../../../../density.md) difference contributes.

The horizontal shallow-layer equations use the vertical component of planetary rotation: $f=2\Omega\sin\varphi$. Thus the source's [vector](../../../../vector.md) notation is interpreted as the projected [vector](../../../../vector.md) $f\mathbf k$ after the [traditional approximation](../../../../traditional-approximation-geophysical-fluid-dynamics.md). Taking the full magnitude $2\Omega$ as a midlatitude [Coriolis parameter](../../../../coriolis-parameter.md) would discard the [latitude](../../../../geographical-latitude.md) dependence. Together with [layer-volume conservation](../../../../volume-conservation.md), the model has $\partial_th+\nabla_h\cdot(h\mathbf u)=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
