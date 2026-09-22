<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\rho_0$ be the reference [mass density](../../../../../../density.md), $\nu$ the [kinematic viscosity](../../../../../../kinematic-viscosity.md), $\kappa$ the [thermal diffusivity](../../../../../../thermal-diffusivity.md), $\eta$ the [magnetic diffusivity](../../../../../../magnetic-diffusivity.md), and $\alpha_T$ the [coefficient of thermal expansion](../../../../../../coefficient-of-thermal-expansion.md). The [conductive state of Rayleigh-Bénard convection](../../../../../../conductive-state-of-rayleigh-benard-convection.md) is $T_b=T_0+\Delta T(1-z/d)$. For the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), density variation is retained only in buoyancy. Linearizing about this state and the imposed [magnetic field](../../../../../../magnetic-field.md) $B_0\hat{\mathbf y}$ gives

$$
\begin{aligned}
\partial_t\mathbf u&=-\frac1{\rho_0}\nabla p_*
+\frac{B_0}{\mu_0\rho_0}\partial_y\mathbf b
+g\alpha_T\theta\hat{\mathbf z}+\nu\Delta\mathbf u,\\
\partial_t\theta&=\frac{\Delta T}{d}w+\kappa\Delta\theta,\\
\partial_t\mathbf b&=B_0\partial_y\mathbf u+\eta\Delta\mathbf b,\qquad
\nabla\cdot\mathbf u=\nabla\cdot\mathbf b=0.
\end{aligned}
$$

Here $w=u_z$ and $p_*=p'+B_0b_y/\mu_0$ is the perturbation of [magnetohydrodynamic total pressure](../../../../../../magnetohydrodynamic-total-pressure.md). The gradient part of the [Lorentz force](../../../../../../lorentz-force.md) has been absorbed into $p_*$; the remaining term is [magnetic tension](../../../../../../magnetic-tension.md). The sign in the temperature equation follows from $dT_b/dz=-\Delta T/d$.

Use the [thermal-diffusion scaling of a convection layer](../../../../../../thermal-diffusion-scaling-of-a-convection-layer.md): length $d$, time $d^2/\kappa$, velocity $\kappa/d$, temperature perturbation $\Delta T$, field perturbation $B_0$, and total-pressure perturbation $\rho_0\nu\kappa/d^2$. Dropping dimensionless-variable decorations gives

$$
\begin{aligned}
\sigma^{-1}\partial_t\mathbf u&=-\nabla p+\zeta Q\,\partial_y\mathbf b
+R\theta\hat{\mathbf z}+\Delta\mathbf u,\\
\partial_t\theta&=w+\Delta\theta,\qquad
\partial_t\mathbf b=\partial_y\mathbf u+\zeta\Delta\mathbf b,\\
\nabla\cdot\mathbf u&=\nabla\cdot\mathbf b=0,
\end{aligned}
$$

with

$$
\boxed{R=\frac{g\alpha_T\Delta T\,d^3}{\nu\kappa},\quad
Q=\frac{B_0^2d^2}{\mu_0\rho_0\nu\eta},\quad
\sigma=\frac{\nu}{\kappa},\quad
\zeta=\frac{\eta}{\kappa}.}
$$

These are respectively the [Rayleigh number](../../../../../../rayleigh-number.md), [Chandrasekhar number](../../../../../../chandrasekhar-number.md), [Prandtl number](../../../../../../prandtl-number.md), and [magnetic-to-thermal diffusivity ratio](../../../../../../magnetic-to-thermal-diffusivity-ratio.md). In particular, the magnetic coefficient is $\zeta Q$, not $Q$ alone, in these thermal-time units. At $z=0,1$, the [boundary conditions](../../../../../../boundary-condition.md) are $\theta=w=b_z=0$, $\partial_z u_x=\partial_z u_y=0$, and $\partial_zb_x=\partial_zb_y=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
