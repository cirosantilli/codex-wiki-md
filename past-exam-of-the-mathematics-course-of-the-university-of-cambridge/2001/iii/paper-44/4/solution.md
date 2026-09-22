<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a stationary solid skeleton, the [Darcy velocity](../../../../../darcy-velocity.md) $\mathbf u$ is liquid volume transport per unit total cross-sectional area, while the [pore velocity](../../../../../pore-velocity.md) $\mathbf v$ is the intrinsic mean fluid [velocity](../../../../../velocity.md) within the connected pore space. Thus

$$
\boxed{\mathbf u=\phi\mathbf v.}
$$

For an incompressible liquid in a saturated region, [conservation of mass](../../../../../mass-conservation.md) is $\phi_t+\nabla\cdot\mathbf u=0$. With time-independent but spatially varying [porosity](../../../../../porosity.md), it becomes

$$
\boxed{\nabla\cdot\mathbf u=\nabla\cdot(\phi\mathbf v)=0,}
$$

not generally $\nabla\cdot\mathbf v=0$. Neglecting dispersion, a fluid interface is advected by the pore [velocity](../../../../../velocity.md); its mean normal speed is $V_n=\mathbf v\cdot\mathbf n=\mathbf u\cdot\mathbf n/\phi$.

For the thin layer on the inclined plane, the [gravitational acceleration](../../../../../gravitational-acceleration.md) components are $g\sin\theta$ downslope and $-g\cos\theta$ normal to the plane. The [hydrostatic approximation](../../../../../hydrostatic-approximation.md) and constant [pressure](../../../../../pressure.md) $p_a$ above the current give

$$
p=p_a+\rho g\cos\theta(h-z).
$$

With [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) $k(z)$, [Darcy's law](../../../../../darcy-law.md) therefore gives

$$
u_x=\frac{\rho gk(z)}\mu(\sin\theta-\cos\theta\,h_x),
\qquad u_y=-\frac{\rho gk(z)}\mu\cos\theta\,h_y.
$$

Here $u_x,u_y$ denote the components of the Darcy [velocity](../../../../../velocity.md). Integrate over depth, using the prescribed power laws:

$$
\mathcal V=\int_0^h\phi(z)\,dz=\frac P\alpha h^\alpha,
$$



$$
\mathbf Q=\int_0^h(u_x,u_y)\,dz
=\frac{\rho gK}{\beta\mu}h^\beta
(\sin\theta-\cos\theta\,h_x,-\cos\theta\,h_y).
$$

Both integrals are finite for the positive exponents in the model. Conservation of the stored fluid gives $\mathcal V_t+\nabla_{x,y}\cdot\mathbf Q=0$, or

$$
\frac P\alpha\partial_t h^\alpha+
\frac{\rho gK\sin\theta}{\beta\mu}\partial_xh^\beta
=\frac{\rho gK\cos\theta}{\beta\mu}
\nabla_{x,y}\cdot(h^\beta\nabla_{x,y}h).
$$

For $0<\theta<\pi/2$, set $X=x\tan\theta$, $Y=y\tan\theta$ and

$$
T=\frac{\alpha\rho gK\sin\theta\tan\theta}{\beta\mu P}t.
$$

Since $\cos\theta\tan^2\theta=\sin\theta\tan\theta$, the [depth-dependent inclined porous-current equation](../../../../../depth-dependent-inclined-porous-current-equation.md) is

$$
\boxed{\partial_T h^\alpha+\partial_Xh^\beta
=\partial_X(h^\beta h_X)+\partial_Y(h^\beta h_Y).}
$$

The longitudinal flux carries fluid downslope, while the thickness-gradient terms spread it. The degenerate horizontal or vertical slope limits need their own coordinate scaling.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
