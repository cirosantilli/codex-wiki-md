<h1 id="7g/solution">Solution</h1>

↑ **Parent:** [7G](../7g.md)

For constant density $\rho$, the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) with a conservative force per unit mass are

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi),\qquad \nabla\cdot\mathbf u=0.
$$

Set $\boldsymbol\omega=\nabla\times\mathbf u$. The vector identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$ and vanishing [curl](../../../../../curl.md) of a gradient give

$$
\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega)
=(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega,
$$

where both divergence terms vanish. Thus the [vorticity equation](../../../../../vorticity-equation.md) is

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

The partial time derivative measures Eulerian change; $(\mathbf u\cdot\nabla)\boldsymbol\omega$ is advection; the right-hand side describes stretching and tilting of vortex lines by [velocity](../../../../../velocity.md) gradients. A conservative body force supplies no [curl](../../../../../curl.md) source, and constant density removes any baroclinic [pressure](../../../../../pressure.md) source.

For planar [velocity](../../../../../velocity.md) independent of $z$, [vorticity](../../../../../vorticity.md) is perpendicular to the plane, $\boldsymbol\omega=(0,0,\omega)$, and $(\boldsymbol\omega\cdot\nabla)\mathbf u=\omega\partial_z\mathbf u=0$. Hence **each material particle conserves its [vorticity](../../../../../vorticity.md)**, $D\omega/Dt=0$. Choose the [stream function](../../../../../stream-function.md) convention $u=\psi_y$, $v=-\psi_x$. Then

$$
\boxed{\omega=v_x-u_y=-\Delta\psi.}
$$

In a steady flow, $\psi_y\omega_x-\psi_x\omega_y=0$, so [vorticity](../../../../../vorticity.md) is constant along [streamlines](../../../../../streamline.md). Where $\nabla\psi\ne0$, use $\psi$ as a local transverse coordinate: this equality makes $\omega$ independent of the coordinate along a streamline. Consequently

$$
\boxed{\Delta\psi=F(\psi)\quad\text{locally on a regular streamline patch}.}
$$

This is [steady planar vorticity as a local function of stream function](../../../../../steady-planar-vorticity-as-a-local-function-of-stream-function.md).

A global single-valued $F$ additionally requires compatible [vorticity](../../../../../vorticity.md) values on all components of each stream-function level set. That condition is not supplied by steady Euler flow alone. For example, $\psi=x^3-x$ gives $(u,v)=(0,1-3x^2)$, a smooth steady incompressible shear with zero advective acceleration and constant [pressure](../../../../../pressure.md). Yet $\psi(0,y)=\psi(1,y)=0$ while $\Delta\psi(0,y)=0$ and $\Delta\psi(1,y)=6$. Thus **the unrestricted global deduction is false; the local result, or a suitable connected-level-set hypothesis, is the valid conclusion**.

## ↑ Ancestors (10)

1. [7G](../7g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
