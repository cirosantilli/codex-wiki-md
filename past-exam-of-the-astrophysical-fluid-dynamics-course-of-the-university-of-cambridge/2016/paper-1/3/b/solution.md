<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\boldsymbol\omega=\nabla\times\mathbf u$ and use the vector identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$. Taking the [curl](../../../../../curl.md) of the momentum equation eliminates all pure [gradients](../../../../../gradient.md), including [gravity](../../../../../gravity.md) and the $\nabla(\nabla\cdot\mathbf u)$ viscous contribution. Before invoking barotropy, the [pressure](../../../../../pressure-split.md) term gives

$$
\nabla\times\left(-\frac1\rho\nabla p\right)=-\nabla(1/\rho)\times\nabla p=\frac{\nabla\rho\times\nabla p}{\rho^2}.
$$

This is [baroclinic vorticity generation](../../../../../baroclinic-vorticity-generation.md). For a [barotropic fluid](../../../../../barotropic-fluid.md), $p=p(\rho)$, so $\nabla p$ is parallel to $\nabla\rho$ and this source vanishes. Constant $\nu$ permits the [curl](../../../../../curl.md) and [Laplacian](../../../../../laplacian.md) to commute. The result is

$$
\boxed{\frac{\partial\boldsymbol\omega}{\partial t}=\nabla\times(\mathbf u\times\boldsymbol\omega)+\nu\nabla^2\boldsymbol\omega}.
$$

No incompressibility assumption was used. Since $\nabla\cdot\boldsymbol\omega=0$, an equivalent form is

$$
\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u-\boldsymbol\omega\,\nabla\cdot\mathbf u+\nu\nabla^2\boldsymbol\omega.
$$

The terms represent [vortex stretching](../../../../../vortex-stretching.md)/tilting, compression/dilatation and viscous diffusion. In particular, removing the baroclinic source does not make the [vorticity](../../../../../vorticity-split.md) of a three-dimensional parcel constant. A spatially varying entropy-dependent $K$ in $p=K\rho^\gamma$ need not define a single barotropic law; the common-pressure-law assumption matters.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
