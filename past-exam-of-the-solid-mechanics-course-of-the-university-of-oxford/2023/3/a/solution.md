<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first equation is the local [balance of linear momentum](../../../../balance-of-linear-momentum.md). Use $\mathsf M,\mathsf L,\mathsf T$ for the dimensions of [mass](../../../../mass.md), [length](../../../../length.md), and [time](../../../../time-in-physics.md), to distinguish dimensional time from the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md) $\mathbf T$.

- $\mathbf x(\mathbf X,t)$ is the current position of the particle labelled by reference position $\mathbf X$; both have dimension $\mathsf L$. The [deformation map](../../../../deformation-map.md) specifies the particle's trajectory.
- $\ddot{\mathbf x}=\partial_t^2\mathbf x|_{\mathbf X}$ is its [material acceleration](../../../../material-acceleration.md), with dimension $\mathsf L\mathsf T^{-2}$. The dots follow the particle and are not spatially fixed time derivatives.
- $\rho$ is current [mass density](../../../../density.md), with dimension $\mathsf M\mathsf L^{-3}$. For a homogeneous material with [incompressibility](../../../../incompressible-flow.md), [mass conservation](../../../../mass-conservation.md) makes it constant in space and time.
- $\mathbf b$ is [body force](../../../../body-force.md) per unit [mass](../../../../mass.md), such as gravitational [acceleration](../../../../acceleration.md), with dimension $\mathsf L\mathsf T^{-2}$. Hence $\rho\mathbf b$ is [force](../../../../force-split.md) per unit [volume](../../../../volume.md).
- $\mathbf T$ is the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md), mapping a unit [normal vector](../../../../normal-vector.md) $\mathbf n$ to surface [traction](../../../../traction.md) $\mathbf T\mathbf n$. Each component has dimension $\mathsf M\mathsf L^{-1}\mathsf T^{-2}$, or [force](../../../../force-split.md) per unit [area](../../../../surface-area.md).
- $\operatorname{div}$ differentiates in the [current configuration](../../../../current-configuration.md), with dimension $\mathsf L^{-1}$. In [Cartesian coordinates](../../../../cartesian-coordinate-system.md), $(\operatorname{div}\mathbf T)_i=\partial T_{ij}/\partial x_j$. Thus $\operatorname{div}\mathbf T$, $\rho\mathbf b$, and $\rho\ddot{\mathbf x}$ all have dimension $\mathsf M\mathsf L^{-2}\mathsf T^{-2}$.
- The superscript $T$ denotes the dimension-preserving [matrix transpose](../../../../transpose.md). The relation $\mathbf T=\mathbf T^T$ expresses [angular momentum conservation](../../../../conservation-of-angular-momentum.md) in a continuum without body couples or couple [stresses](../../../../stress.md).

Here $t$ has dimension $\mathsf T$. The hypothesis $\partial_t\mathbf b=\mathbf0$ means that the prescribed spatial [body force](../../../../body-force.md) field is the same for every member of the static family and the resulting motion.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
