<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce the [thermal expansion coefficient](../../../../../../thermal-expansion-coefficient.md) $\alpha_T=-\rho_0^{-1}(\partial\rho/\partial T)$, so the linear [equation of state](../../../../../../equation-of-state.md) is $\rho=\rho_0[1-\alpha_T(T-T_0)]$. With gravity $-g\widehat{\boldsymbol z}$, the resting [conductive state of Rayleigh-Bénard convection](../../../../../../conductive-state-of-rayleigh-benard-convection.md) satisfies the steady [heat equation](../../../../../../heat-equation.md) and [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) balance. Consequently

$$
\boxed{\boldsymbol u_b=0,\qquad T_b(z)=T_0+\Delta T(1-z/d),}
$$

and, up to an arbitrary constant,

$$
\boxed{P_b(z)=P_b(0)-\rho_0g\left[(1-\alpha_T\Delta T)z+\frac{\alpha_T\Delta T}{2d}z^2\right].}
$$

Indeed $P_b'=-g\rho_b$, where $\rho_b=\rho_0[1-\alpha_T\Delta T(1-z/d)]$.

The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) retains temperature-dependent [mass density](../../../../../../density.md) in [buoyancy](../../../../../../buoyancy.md) while replacing it by $\rho_0$ in inertial coefficients; it requires $|\alpha_T\Delta T|\ll1$. Subtracting the [conductive state of Rayleigh-Bénard convection](../../../../../../conductive-state-of-rayleigh-benard-convection.md) and dropping products of perturbations gives the dimensional [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md)

$$
\partial_{t_*}\boldsymbol u_*=-\rho_0^{-1}\nabla_*p_*+g\alpha_T\theta_*\widehat{\boldsymbol z}+\nu\nabla_*^2\boldsymbol u_*,\qquad
\partial_{t_*}\theta_*-\frac{\Delta T}{d}w_*=\kappa\nabla_*^2\theta_*,\qquad \nabla_*\cdot\boldsymbol u_*=0.
$$

The minus sign in the temperature equation comes from $\boldsymbol u_*\cdot\nabla_*T_b=-w_*\Delta T/d$.

Use the [thermal-diffusion scaling of a convection layer](../../../../../../thermal-diffusion-scaling-of-a-convection-layer.md)

$$
\boldsymbol x_*=d\boldsymbol x,\qquad t_*=\frac{d^2}{\kappa}t,\qquad
\boldsymbol u_*=\frac\kappa d\boldsymbol u,\qquad
\theta_*=\Delta T\theta,\qquad p_*=\frac{\rho_0\kappa^2}{d^2}p.
$$

The [Rayleigh number](../../../../../../rayleigh-number.md) and [Prandtl number](../../../../../../prandtl-number.md) are

$$
\boxed{\mathrm{Ra}=\frac{g\alpha_T\Delta T d^3}{\nu\kappa},\qquad \mathrm{Pr}=\frac\nu\kappa.}
$$

Thus **the nondimensional perturbation equations are**

$$
\boxed{\partial_t\boldsymbol u=-\nabla p+\mathrm{Ra}\,\mathrm{Pr}\,\theta\widehat{\boldsymbol z}+\mathrm{Pr}\nabla^2\boldsymbol u,\qquad
\partial_t\theta-w=\nabla^2\theta,\qquad \nabla\cdot\boldsymbol u=0.}
$$

Here $\nu$ is [kinematic viscosity](../../../../../../kinematic-viscosity.md), $\kappa$ is [thermal diffusivity](../../../../../../thermal-diffusivity.md), and positive $\mathrm{Ra}$ denotes destabilizing heating from below for $\alpha_T>0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
