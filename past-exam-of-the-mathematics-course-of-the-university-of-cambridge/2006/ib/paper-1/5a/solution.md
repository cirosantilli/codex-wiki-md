<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

The displayed evolution law uses the usual assumptions of [incompressible flow](../../../../../incompressible-flow.md), constant [density](../../../../../density.md) and conservative body force. With $\boldsymbol\omega=\nabla\times\mathbf u$, the [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md) is

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi).
$$

Use $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$ and take a [curl](../../../../../curl.md). [Gradients](../../../../../gradient.md) have zero [curl](../../../../../curl.md), and

$$
\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega)
=(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega
+\mathbf u\nabla\cdot\boldsymbol\omega-\boldsymbol\omega\nabla\cdot\mathbf u.
$$

Here $\nabla\cdot\boldsymbol\omega=0$ because it is a [curl](../../../../../curl.md), and $\nabla\cdot\mathbf u=0$ by incompressibility. The [vorticity equation](../../../../../vorticity-equation.md) is therefore

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

The [material derivative](../../../../../material-derivative.md) combines local change with advection by fluid particles. The right-hand side is [vortex stretching](../../../../../vortex-stretching.md) and tilting: spatial variation of velocity along a vortex line changes its strength and direction. Along each particle path this is a homogeneous linear equation for [vorticity](../../../../../vorticity.md). For a smooth velocity field its solution with zero initial [vorticity](../../../../../vorticity.md) remains zero by uniqueness. Thus an initially [irrotational flow](../../../../../irrotational-flow.md) remains irrotational while these assumptions and smoothness hold.

For a plane flow $\mathbf u=(u(x,y,t),v(x,y,t),0)$, the [vorticity](../../../../../vorticity.md) is $\boldsymbol\omega=(0,0,\zeta)$ and $(\boldsymbol\omega\cdot\nabla)\mathbf u=\zeta\partial_z\mathbf u=0$. Hence $D\zeta/Dt=0$. Every particle retains its initial value, so an initially uniform value gives

$$
\boxed{\boldsymbol\omega(x,y,t)=\boldsymbol\omega_0\quad\text{for all later times}.}
$$

Inviscid motion alone is insufficient for the printed simplified law: compressible variable-density motion generally adds $-\boldsymbol\omega\nabla\cdot\mathbf u+\nabla\rho\times\nabla p/\rho^2$. Those terms vanish under the assumptions used above.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
