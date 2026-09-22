<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $K$ denote isotropic [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md), $\mu$ the fluid [dynamic viscosity](../../../../../dynamic-viscosity.md), $\rho_0$ the reference fluid [mass density](../../../../../density.md), $\alpha>0$ its volumetric thermal-expansion coefficient and $g$ [gravitational acceleration](../../../../../gravitational-acceleration.md). The [Boussinesq approximation](../../../../../boussinesq-approximation.md) uses $\rho=\rho_0[1-\alpha(T-T_*)]$ only in the gravitational force. With upward coordinate $z$, hydraulic [pressure](../../../../../pressure.md) $P$ and [Darcy flux](../../../../../darcy-velocity.md) $\mathbf q$, the equations are

$$
\mathbf q=-\frac K\mu\nabla P+B\theta\mathbf e_z,\qquad\nabla\cdot\mathbf q=0,\qquad B=\frac{\rho_0g\alpha K}{\mu},
$$

where $\theta$ is the perturbation to the conductive [temperature](../../../../../temperature.md). To keep porous heat-capacity conventions explicit, let $C_e$ be effective [heat capacity](../../../../../heat-capacity.md) per bulk volume, $C_f=\rho_0c_f$ the liquid volumetric [heat capacity](../../../../../heat-capacity.md), $k_e$ effective [thermal conductivity](../../../../../thermal-conductivity.md), $\sigma=C_e/C_f$, and $\kappa=k_e/C_f$. The thermal equation is $\sigma T_t+\mathbf q\cdot\nabla T=\kappa\nabla^2T$. If the usual unit-capacity convention is adopted, $\sigma=1$ and $\kappa$ is the [thermal diffusivity](../../../../../thermal-diffusivity.md). Thresholds below do not depend on $\sigma$; it only changes temporal rates.

For a conductive state with upward [temperature](../../../../../temperature.md) decrease $\Gamma=-\overline T_z>0$, linearization gives

$$
\sigma\theta_t-\Gamma w=\kappa\nabla^2\theta,\qquad
\nabla^2w=B\nabla_\perp^2\theta,
$$

where $w=q_z$. The second equation follows by taking the divergence of [Darcy law](../../../../../darcy-law.md) to eliminate $P$ and then differentiating its vertical component. It is important that the Laplacian on its right is horizontal.

In the horizontal layer, both boundary planes prescribe the [temperature](../../../../../temperature.md) and are impermeable, so $\theta=w=0$ at $z=0,h$. Use a [normal mode](../../../../../normal-mode.md) proportional to $e^{st+i\mathbf k\cdot\mathbf x}\sin(n\pi z/h)$, with horizontal [wavenumber](../../../../../wavenumber.md) $k=|\mathbf k|$, $n\geq1$. Writing $b=n\pi/h$, the momentum relation gives $w=Bk^2\theta/(k^2+b^2)$, and the thermal relation gives

$$
\sigma s=\frac{B\Gamma k^2}{k^2+b^2}-\kappa(k^2+b^2).
$$

A neutral mode therefore requires $B\Gamma/\kappa=(k^2+b^2)^2/k^2$. Since $k^2+2b^2+b^4/k^2\geq4b^2$, the smallest value is $4\pi^2/h^2$, attained at $n=1$ and $k=\pi/h$. This derives the [onset of convection in a horizontal Darcy layer](../../../../../onset-of-convection-in-a-horizontal-darcy-layer.md) rather than simply importing its critical number. Thus

$$
\boxed{T_{m,\mathrm{crit}}=T_0+\frac{4\pi^2\mu\kappa}{\rho_0g\alpha Kh}.}
$$

**Every small disturbance decays for $T_m<T_{m,\mathrm{crit}}$; at equality the critical roll is neutral.** Strict decay has this threshold as a supremum, not an attained maximum. The first roll wavelength is $2h$, compatible with the very large horizontal extent. Cooling from above gives the opposite, stable [buoyancy](../../../../../buoyancy.md) feedback.

For the tall square column, define $a$ as its side length and $H\gg a$ as its height. The insulated vertical walls impose $\partial_n\theta=0$, while impermeability imposes zero normal [Darcy flux](../../../../../darcy-velocity.md). Away from the remote ends, a nearly height-independent mode has [hydrostatic pressure](../../../../../hydrostatic-pressure.md) adjustment and $w=B\theta$, with zero cross-sectional mean. The transverse [temperature](../../../../../temperature.md) modes are

$$
\theta\propto\cos(m\pi x/a)\cos(n\pi y/a),\qquad
k_\perp^2=\frac{\pi^2(m^2+n^2)}{a^2},
$$

where $m,n\geq0$ but $(m,n)=(0,0)$ is excluded: a closed column cannot support a net vertical discharge. Its horizontally uniform [density](../../../../../density.md) perturbation is balanced by [pressure](../../../../../pressure.md), rather than driving overturning. The rate of a nonconstant mode is

$$
\sigma s=B\Gamma-\kappa k_\perp^2.
$$

The smallest allowed [eigenvalue](../../../../../eigenvalue.md) is $\pi^2/a^2$, so the [insulated square-column Darcy convection onset](../../../../../insulated-square-column-darcy-convection-onset.md) is

$$
\boxed{\Gamma_{\mathrm{crit}}=\frac{\pi^2\mu\kappa}{\rho_0g\alpha Ka^2}.}
$$

Again strict decay requires $\Gamma<\Gamma_{\mathrm{crit}}$. This is the leading long-column result. End conditions that maintain the basic gradient require the vertical [velocity](../../../../../velocity.md) to turn around near the ends and give small finite-height corrections; their exact coefficient cannot be inferred from insulation of the vertical walls alone. For a separated vertical mode of small [wavenumber](../../../../../wavenumber.md) $k_z$, the neutral expression is $B\Gamma/\kappa=(k_\perp^2+k_z^2)^2/k_\perp^2$, which tends to the displayed value as $H/a\to\infty$.

Just above threshold, warm fluid rises along one side and colder fluid sinks along the opposite side, with horizontal return flow at the top and bottom. The two lowest modes, proportional to $\cos(\pi x/a)$ and $\cos(\pi y/a)$, have the same threshold. A square therefore admits either orientation or a superposition, including diagonal overturning. Linear theory predicts the weak columnar circulation and its degeneracy; it does not select a unique nonlinear planform.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
