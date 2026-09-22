<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [entrainment coefficient](../../../../../../entrainment-coefficient.md) $\alpha$ is the ratio of the inward ambient-fluid [velocity](../../../../../../velocity.md) normal to a [buoyant plume](../../../../../../buoyant-plume.md) edge to the characteristic [buoyant plume](../../../../../../buoyant-plume.md) [velocity](../../../../../../velocity.md). For an upward [buoyant plume](../../../../../../buoyant-plume.md), take $u_e=\alpha w>0$. There are two edges at half-width $b$, so the full-section volume source is $2u_e$. Dividing every integral balance by two gives consistent half-section equations.

For [top-hat plume](../../../../../../top-hat-plume-model.md) profiles, [volume conservation](../../../../../../volume-conservation.md) and [mass conservation](../../../../../../mass-conservation.md) are

$$
\boxed{b_t+(bw)_z=\alpha w,\qquad
(\rho b)_t+(\rho bw)_z=\rho_0(z)\alpha w.}
$$

The mass entering the [buoyant plume](../../../../../../buoyant-plume.md) is ambient mass with local [mass density](../../../../../../density.md) $\rho_0(z)$. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) uses a common reference [mass density](../../../../../../density.md) in inertia while retaining the [mass density](../../../../../../density.md) deficit in [buoyancy](../../../../../../buoyancy.md). The mass equation may be kept to the first order in that deficit to derive its transport.

Multiply the volume equation by the time-independent ambient [mass density](../../../../../../density.md). The product rule gives

$$
(\rho_0b)_t+(\rho_0bw)_z=\rho_0\alpha w+\rho_0'(z)bw.
$$

Subtract the mass equation and multiply by $g$. The [entrainment](../../../../../../fluid-entrainment.md) sources cancel exactly, leaving

$$
\boxed{\partial_t[(\rho_0-\rho)gb]+\partial_z[(\rho_0-\rho)gbw]
=g\rho_0'(z)bw=-\rho_0N^2bw,}
$$

where

$$
\boxed{N^2=-\frac{g}{\rho_0}\frac{d\rho_0}{dz}.}
$$

For stable [stratification](../../../../../../density-stratification.md), $\rho_0'<0$ and the [buoyancy frequency](../../../../../../buoyancy-frequency.md) $N$ is real. Rising fluid moves into lighter ambient fluid and loses its [mass density](../../../../../../density.md) deficit relative to that local ambient. Thus environmental [stratification](../../../../../../density-stratification.md) reduces the [buoyant plume](../../../../../../buoyant-plume.md)'s [buoyancy flux](../../../../../../buoyancy-flux.md), even though the ambient fluid entering by [entrainment](../../../../../../fluid-entrainment.md) contributes no [mass density](../../../../../../density.md) deficit at its own height.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
