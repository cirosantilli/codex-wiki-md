<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $L_\perp=k_\perp^{-1}$ and let $U$ be the common size of horizontal and vertical [velocity](../../../../velocity.md) perturbations, as found in part [b](../b.md). The linear [inertial wave](../../../../inertial-wave.md) time and nonlinear advection time are

$$
\tau_w^{-1}\sim2\Omega\frac{|k_\parallel|}{k_\perp},\qquad
\tau_{\rm nl}^{-1}\sim k_\perp U.
$$

The [critical balance in a rapidly rotating fluid](../../../../critical-balance-in-a-rapidly-rotating-fluid.md) is therefore

$$
\boxed{\epsilon=\frac{|k_\parallel|}{k_\perp}
\sim\frac{k_\perp U}{2\Omega}\ll1,\qquad
\omega\sim k_\perp U\sim2\Omega\epsilon.}
$$

The [Rossby number](../../../../rossby-number.md) is of order $\epsilon$. Horizontal [geostrophic flow](../../../../geostrophic-flow.md) balances the leading [pressure gradient](../../../../pressure-gradient.md) against [Coriolis acceleration](../../../../coriolis-acceleration.md), so

$$
\boxed{u_\perp\sim u_\parallel\sim U,\quad
\delta p\sim2\Omega L_\perp U\sim U^2/\epsilon,\quad
k_\parallel\sim\epsilon k_\perp.}
$$

These are dimensionally comparable statements, rather than comparisons of a dimensional [frequency](../../../../frequency.md) with a dimensional [velocity](../../../../velocity.md). Equivalently, use $L_\perp$ and $(2\Omega)^{-1}$ as units. Then

$$
k_\perp L_\perp=O(1),\quad
k_\parallel L_\perp=O(\epsilon),\quad
\frac{\omega}{2\Omega}=O(\epsilon),\quad
\frac{u_\perp}{2\Omega L_\perp},\frac{u_\parallel}{2\Omega L_\perp}=O(\epsilon),\quad
\frac{\delta p}{(2\Omega L_\perp)^2}=O(\epsilon).
$$

Thus rotation stays $O(1)$ in these units, while the motions evolve on the slower $O(\epsilon^{-1})$ time. Vertical advection $u_\parallel\partial_z$ is smaller than horizontal advection by $\epsilon$.

Write $\mathbf u_\perp=\mathbf u_\perp^{(0)}+\mathbf u_\perp^{(1)}+\cdots$, with $\mathbf u_\perp^{(1)}=O(\epsilon U)$, and $p=p_0+p_1+\cdots$. At leading horizontal order,

$$
0=-\nabla_\perp p_0+2\Omega\mathbf u_\perp^{(0)}\times\widehat{\mathbf z}.
$$

Define the [stream function](../../../../stream-function.md) $\Phi=p_0/(2\Omega)$, including its horizontally uniform part in this convention. Then

$$
\boxed{\mathbf u_\perp^{(0)}=\widehat{\mathbf z}\times\nabla_\perp\Phi
=(-\partial_y\Phi,\partial_x\Phi),\qquad
\nabla_\perp\cdot\mathbf u_\perp^{(0)}=0.}
$$

The next-order [incompressibility](../../../../incompressible-flow.md) condition is not zero horizontal divergence:

$$
\boxed{\nabla_\perp\cdot\mathbf u_\perp^{(1)}=-\partial_z u_\parallel.}
$$

This term has size $\epsilon k_\perp U$ and is essential: its product with the large rotation rate is a leading contribution to the vertical [vorticity](../../../../vorticity-split.md) equation.

To see that contribution explicitly, write $D_\perp=\partial_t+\mathbf u_\perp^{(0)}\cdot\nabla_\perp$. At the first horizontal inertial order,

$$
D_\perp\mathbf u_\perp^{(0)}=-\nabla_\perp p_1
+2\Omega\mathbf u_\perp^{(1)}\times\widehat{\mathbf z}.
$$

Taking its vertical [curl](../../../../curl.md) eliminates $p_1$. The two-dimensional advection identity and the two divergence orders give

$$
D_\perp\zeta=-2\Omega\nabla_\perp\cdot\mathbf u_\perp^{(1)}
=2\Omega\partial_z u_\parallel,\qquad
\zeta=(\nabla_\perp\times\mathbf u_\perp^{(0)})_z=\nabla_\perp^2\Phi.
$$

Equivalently the [ageostrophic flow](../../../../ageostrophic-flow.md) satisfies

$$
\mathbf u_\perp^{(1)}=\frac{\widehat{\mathbf z}\times[D_\perp\mathbf u_\perp^{(0)}+\nabla_\perp p_1]}{2\Omega},
$$

whose divergence is $-D_\perp\zeta/(2\Omega)$. This explicitly verifies that the next-order divergence has the required sign.

The vertical momentum equation, at the same slow order, is

$$
D_\perp u_\parallel=-\partial_zp_0=-2\Omega\partial_z\Phi.
$$

Finally $\mathbf u_\perp^{(0)}\cdot\nabla_\perp f=\{\Phi,f\}$, where the canonical two-dimensional [Poisson bracket](../../../../poisson-bracket.md) is $\{f,g\}=f_xg_y-f_yg_x$. The [reduced equations for an anisotropic rotating fluid](../../../../reduced-equations-for-an-anisotropic-rotating-fluid.md) are

$$
\boxed{\begin{aligned}
\partial_t\nabla_\perp^2\Phi+\{\Phi,\nabla_\perp^2\Phi\}
&=2\Omega\partial_z u_\parallel,\\
\partial_tu_\parallel+\{\Phi,u_\parallel\}
&=-2\Omega\partial_z\Phi.
\end{aligned}}
$$

The omitted vertical-advection, ageostrophic-advection and relative-vorticity stretching terms are smaller by $O(\epsilon)$ in the equations retained here. Linearizing these equations recovers $\omega^2=4\Omega^2k_\parallel^2/k_\perp^2$, the anisotropic limit of part [a](../a.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
