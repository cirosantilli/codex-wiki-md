<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $b=\delta B_\parallel/B_0$ and $\mathbf b_\perp=\delta\mathbf B_\perp/B_0=\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$. Define the two-dimensional [Poisson bracket](../../../../../../poisson-bracket.md) by

$$
\{f,g\}=\partial_xf\,\partial_yg-\partial_yf\,\partial_xg.
$$

Then, to the retained anisotropic order, the derivative along the perturbed [magnetic field](../../../../../../magnetic-field.md) is

$$
\boxed{\nabla_\parallel\equiv\frac{\mathbf B}{B_0}\cdot\nabla=\partial_z+\mathbf b_\perp\cdot\nabla_\perp=\partial_z+\frac1{v_A}\{\Psi,\cdot\}.}
$$

The omitted $b\partial_z$ term is smaller by $\epsilon$ than either retained term. The nonlinear field-line-bending term is of the same order as $\partial_z$, which is why it must remain.

Use $\mathbf u_e=-\alpha\nabla\times\mathbf B$ with $\alpha B_0=v_Ad_i$. The leading parallel and perpendicular [Electron](../../../../../../electron.md) [velocities](../../../../../../velocity.md) are

$$
\boxed{\mathbf u_{e\perp}=v_Ad_i\hat{\mathbf z}\times\nabla_\perp b,\qquad u_{e\parallel}=-d_i\nabla_\perp^2\Psi.}
$$

In detail, $\nabla\times(B_0b\hat{\mathbf z})=-B_0\hat{\mathbf z}\times\nabla_\perp b$, while the parallel [curl](../../../../../../curl.md) of $B_0\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$ is $B_0\nabla_\perp^2\Psi/v_A$. The perpendicular [curl](../../../../../../curl.md) involving $\partial_z\delta\mathbf B_\perp$ is order-smaller. Exact [Electron](../../../../../../electron.md) [incompressibility](../../../../../../incompressible-flow.md) follows from the [divergence](../../../../../../divergence.md) of a [curl](../../../../../../curl.md); its small [velocity](../../../../../../velocity.md) correction supplies any [divergence](../../../../../../divergence.md) omitted by this leading representation.

The [electron magnetohydrodynamics](../../../../../../electron-magnetohydrodynamics.md) equation is frozen-in induction,

$$
\partial_t\mathbf B=(\mathbf B\cdot\nabla)\mathbf u_e-(\mathbf u_e\cdot\nabla)\mathbf B,
$$

because both $\mathbf B$ and $\mathbf u_e$ are [solenoidal](../../../../../../solenoidal-vector-field.md). Keeping its leading order-$\epsilon^2$ perpendicular terms gives

$$
\partial_t\mathbf b_\perp=\partial_z\mathbf u_{e\perp}+(\mathbf b_\perp\cdot\nabla_\perp)\mathbf u_{e\perp}-(\mathbf u_{e\perp}\cdot\nabla_\perp)\mathbf b_\perp.
$$

Let $X_f=\hat{\mathbf z}\times\nabla_\perp f=(-f_y,f_x)$. Expanding the two components gives $(X_f\cdot\nabla)X_g-(X_g\cdot\nabla)X_f=X_{\{f,g\}}$. Substitution therefore reduces the perpendicular equation to

$$
\frac1{v_A}X_{\partial_t\Psi}=v_Ad_iX_{\partial_zb}+d_iX_{\{\Psi,b\}}=v_Ad_iX_{\nabla_\parallel b}.
$$

The perpendicular-constant freedom in $\Psi$ has no magnetic effect and can be fixed so that

$$
\boxed{\partial_t\Psi=v_A^2d_i\nabla_\parallel b.}
$$

The parallel induction component at the same order is

$$
\partial_tb+\mathbf u_{e\perp}\cdot\nabla_\perp b=\nabla_\parallel u_{e\parallel}.
$$

The advection term vanishes since $\mathbf u_{e\perp}\cdot\nabla_\perp b=v_Ad_i\{b,b\}=0$. Thus

$$
\boxed{\partial_tb=-d_i\nabla_\parallel\nabla_\perp^2\Psi.}
$$

Together these are both required [reduced electron magnetohydrodynamics](../../../../../../reduced-electron-magnetohydrodynamics.md) equations. Terms such as $u_{e\parallel}\partial_zb$ and $b\partial_z\mathbf u_e$ are order-$\epsilon^3$ and consistently absent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
