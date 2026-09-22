<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Boussinesq approximation](../../../../../boussinesq-approximation.md) assumes that the fractional [mass density](../../../../../density.md) variations are small. Replace density by a constant reference value in inertia, pressure scaling and [mass conservation](../../../../../mass-conservation.md), but retain its small anomaly in the gravitational force: the large hydrostatic force otherwise cancels, leaving precisely the buoyancy-driving term. For temperature-driven motion, write $\rho=\rho_r[1-\alpha(T-T_r)]$ with $|\alpha(T-T_r)|\ll1$. The resulting velocity is an [incompressible flow](../../../../../incompressible-flow.md); compressional heating and acoustic effects are omitted in the shallow, low-compressibility regime.

For this convection problem, use the [strong Boussinesq approximation](../../../../../strong-boussinesq-approximation.md) in the constant-property sense: the [thermal expansion coefficient](../../../../../thermal-expansion-coefficient.md), [kinematic viscosity](../../../../../kinematic-viscosity.md), [thermal diffusivity](../../../../../thermal-diffusivity.md) and heat capacity are also independent of temperature over the layer. This additional assumption makes the conduction profile linear and the perturbation coefficients constant. This usage of “strong” is the convection convention described in [https://courses.physics.ucsd.edu/2021/Spring/physics218c/Spiegel%20Convection.pdf](https://courses.physics.ucsd.edu/2021/Spring/physics218c/Spiegel%20Convection.pdf) . Some stratified-flow literature uses “strong” instead to emphasize a globally constant reference density; that condition is also satisfied here. The equations below specify precisely which assumptions are being used.

Introduce the [thermal diffusivity](../../../../../thermal-diffusivity.md) $\kappa$ and positive [thermal expansion coefficient](../../../../../thermal-expansion-coefficient.md) $\alpha$, which are necessary material data even though the question names only $\nu$ explicitly. Measure $z$ upward from the bottom. The [conductive state of Rayleigh-Bénard convection](../../../../../conductive-state-of-rayleigh-benard-convection.md) is $T_b=T_0+\Delta T(1-z/d)$ with zero velocity. Let $\theta=T-T_b$ and let $\pi$ be perturbation pressure divided by the reference density, after subtracting the hydrostatic base pressure. Linearizing gives

$$
(\partial_t-\nu\nabla^2)u=-\nabla\pi+g\alpha\theta e_z,\qquad
\nabla\cdot u=0,\qquad
(\partial_t-\kappa\nabla^2)\theta=\frac{\Delta T}{d}w.
$$

The sign in the last equation is positive because upward motion carries warmer base-state fluid into cooler surroundings. Taking the divergence of momentum gives $\nabla^2\pi=g\alpha\theta_z$. Apply a Laplacian to its vertical component and subtract the vertical derivative of that pressure identity. This eliminates pressure:

$$
(\partial_t-\nu\nabla^2)\nabla^2w=g\alpha\nabla_h^2\theta,
\qquad\nabla_h^2=\partial_x^2+\partial_y^2.
$$

Apply the temperature operator to obtain the **vertical-velocity equation**

$$
\boxed{(\partial_t-\kappa\nabla^2)(\partial_t-\nu\nabla^2)\nabla^2w
=\frac{g\alpha\Delta T}{d}\nabla_h^2w.}
$$

This is the pressure- and temperature-eliminated [linear stability analysis](../../../../../linear-stability.md) equation for [Rayleigh-Bénard convection](../../../../../rayleigh-benard-convection.md).

At each boundary, impermeability gives $w=0$, the [stress-free boundary condition](../../../../../stress-free-boundary-condition.md) gives $w_{zz}=0$, and perfect thermal conduction gives $\theta=0$. To obtain the second condition, zero tangential traction gives $\partial_zu_h+\nabla_hw=0$; since $w$ vanishes identically along the boundary, differentiate horizontal [incompressibility](../../../../../incompressible-flow.md) to get $w_{zz}=0$. For the fully eliminated velocity equation, $\theta=0$ and the preceding momentum relation also imply $w_{zzzz}=0$ there. Thus suitable formulations are

$$
\boxed{w=w_{zz}=0,\quad\theta=0\quad(z=0,d),}
$$

or, for the sixth-order vertical equation alone, $w=w_{zz}=w_{zzzz}=0$ at both boundaries. Fixed boundary temperature means a zero perturbation there, not zero perturbation heat flux.

Use normal modes $w=W\sin(n\pi z/d)e^{\sigma t+i\boldsymbol k\cdot\boldsymbol x_h}$, $n\geq1$, $k=|\boldsymbol k|>0$. Put $K^2=k^2+n^2\pi^2/d^2$. Substitution yields the [stress-free convection growth-rate polynomial](../../../../../stress-free-convection-growth-rate-polynomial.md)

$$
\boxed{(\sigma+\nu K^2)(\sigma+\kappa K^2)K^2
=\frac{g\alpha\Delta T}{d}k^2.}
$$

At stationary marginal stability, $\sigma=0$. In terms of the [Rayleigh number](../../../../../rayleigh-number.md) $\mathrm{Ra}=g\alpha\Delta T d^3/(\nu\kappa)$ and dimensionless horizontal wave number $a=kd$, the [free-slip convection neutral curve](../../../../../free-slip-convection-neutral-curve.md) is

$$
\mathrm{Ra}_n(a)=\frac{(a^2+n^2\pi^2)^3}{a^2}.
$$

Writing $y=a^2$ and differentiating gives $d\log\mathrm{Ra}_n/dy=3/(y+n^2\pi^2)-1/y$. Its zero is $a^2=n^2\pi^2/2$, with minimum $27n^4\pi^4/4$. The smallest vertical mode is $n=1$, so the **critical temperature difference** is

$$
\boxed{\mathrm{Ra}_c=\frac{27\pi^4}{4},\qquad
\Delta T_{\max}=\frac{27\pi^4\nu\kappa}{4g\alpha d^3}.}
$$

The first unstable horizontal wavelength is $2\sqrt2d$. To check that an oscillatory mode cannot destabilize earlier, expand the growth-rate equation: its linear coefficient is $(\nu+\kappa)K^2>0$, and its constant term changes sign exactly at the stationary neutral curve. For positive temperature difference the discriminant is $(\nu-\kappa)^2K^4+4g\alpha\Delta T k^2/(dK^2)>0$, so the crossing root is real. Below the global critical value every convection mode decays; at criticality the selected mode is marginal; above it some modes grow and eventually require nonlinear advection, producing convective heat transport. This is [exchange of stabilities in stress-free convection](../../../../../exchange-of-stabilities-in-stress-free-convection.md).

Strictly, the linearized equations remain the correct small-amplitude equations on either side of onset. What fails above $\Delta T_{\max}$ is stability of the conductive state and long-time validity of a small-perturbation description, not the algebra of linearization. The threshold also presumes that the required small density variations and constant-property approximation hold at that temperature difference.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 84](../../paper-84-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
