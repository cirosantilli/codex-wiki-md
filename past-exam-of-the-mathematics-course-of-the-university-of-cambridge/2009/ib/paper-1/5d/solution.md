<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

The [divergence](../../../../../divergence.md) of this axisymmetric [velocity field](../../../../../velocity-field.md) is $r^{-1}\partial_r(-\alpha r^2)+\partial_z(2\alpha z)=-2\alpha+2\alpha=0$. Thus it satisfies [incompressibility](../../../../../incompressible-flow.md). The apparent axis singularity in the azimuthal component is removable, since $u_\theta\sim\gamma\beta r$ as $r\to0$.

Only the axial [vorticity](../../../../../vorticity.md) component is nonzero:

$$
\boxed{\boldsymbol\omega=\nabla\times\mathbf u=(0,0,w(r)),\qquad w(r)=2\beta\gamma e^{-\beta r^2}.}
$$

The [cross product](../../../../../cross-product.md) is $\mathbf u\times\boldsymbol\omega=(u_\theta w,\alpha r w,0)$. Its components are independent of $z$ and $\theta$, so its [curl](../../../../../curl.md) also has only an axial component:

$$
\bigl[\nabla\times(\mathbf u\times\boldsymbol\omega)\bigr]_z=\frac1r\frac d{dr}(\alpha r^2w)=\alpha(2w+rw')=2\alpha(1-\beta r^2)w.
$$

Meanwhile $w'=-2\beta rw$ and $w''=(-2\beta+4\beta^2r^2)w$, giving

$$
\nabla^2\boldsymbol\omega=(0,0,w''+w'/r)=(0,0,-4\beta(1-\beta r^2)w).
$$

Thus the required steady [vorticity equation](../../../../../vorticity-equation.md) holds with **$\nu=\alpha/(2\beta)$**. This is the balance between vortex stretching and viscous diffusion in a [Burgers vortex](../../../../../burgers-vortex.md).

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
