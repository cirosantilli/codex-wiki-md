<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $w(x,t)$ for the vertical displacement of the [sea ice](../../../../../../sea-ice.md), and take the undisturbed water surface as $z=0$, with water occupying $z<0$. The [elastic plate](../../../../../../elastic-plate.md) has areal mass $m=\rho_i h$ and [bending stiffness](../../../../../../bending-stiffness.md)

$$
D=\frac{Eh^3}{12(1-\eta^2)}.
$$

Here $E$ is [Young's modulus](../../../../../../young-s-modulus.md) and $\eta$ is [Poisson's ratio](../../../../../../poisson-s-ratio.md). We neglect in-plane prestress, viscosity and plate shear deformation, and linearize about hydrostatic equilibrium. These are important assumptions: perfect elasticity alone does not specify every term in a floating-plate model.

For a [plane wave](../../../../../../plane-wave.md) $w=\widehat w e^{i(kx-\omega t)}$, $k>0$, [potential flow](../../../../../../potential-flow.md) in deep water has [velocity potential](../../../../../../velocity-potential.md) $\phi=\widehat\phi e^{kz}e^{i(kx-\omega t)}$. This solves [Laplace's equation](../../../../../../laplace-equation.md) and decays downwards. The [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) gives $k\widehat\phi=-i\omega\widehat w$. Linearizing the water pressure at the displaced interface gives an upward excess load

$$
\widehat p=-\rho_w(\phi_t+gw)
=\rho_w\left(\frac{\omega^2}{k}-g\right)\widehat w.
$$

The [elastic plate](../../../../../../elastic-plate.md) equation is $m w_{tt}+D w_{xxxx}=p$. Substitution and multiplication by $k$ therefore give the [flexural-gravity wave](../../../../../../flexural-gravity-wave.md) [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{Dk^5+(\rho_wg-\rho_i h\omega^2)k-\rho_w\omega^2=0.}
$$

Equivalently, with $\alpha=\rho_i h/\rho_w$ and $\beta=D/\rho_w$,

$$
\boxed{\omega^2=\frac{gk+\beta k^5}{1+\alpha k}.}
$$

This determines the positive [wavenumber](../../../../../../wavenumber.md) implicitly for prescribed positive [angular frequency](../../../../../../angular-frequency.md). It is unambiguous: the [derivative](../../../../../../derivative.md) of $\omega^2$ is $(g+5\beta k^4+4\alpha\beta k^5)/(1+\alpha k)^2>0$, while $\omega^2$ runs from zero to infinity.

The [phase velocity](../../../../../../phase-velocity.md) and [group velocity](../../../../../../group-velocity.md) are

$$
c_p=\frac{\omega}{k},\qquad
\boxed{c_g=\frac{g+5\beta k^4+4\alpha\beta k^5}{2\omega(1+\alpha k)^2}.}
$$

For open-water [deep-water gravity waves](../../../../../../deep-water-gravity-wave.md), $\omega^2=gk$, and hence $c_p=gT/(2\pi)$ and $c_g=gT/(4\pi)$. At large period the ice-covered curves approach these straight lines. At shorter period, plate bending raises the speeds, so both ice-covered curves turn upward as period decreases. In the bending regime with negligible plate inertia, $\omega\propto k^{5/2}$ and $c_g\simeq(5/2)c_p$; in the formal plate-inertia-dominated limit, $\omega\propto k^2$ and $c_g\simeq2c_p$. The latter extrapolation eventually leaves thin-plate validity and should not be read as a prediction at arbitrarily small [wavelength](../../../../../../wavelength.md).

<a id="1/a/image-phase-and-group-velocities-of-flexural-gravity-waves-compared-with-open-water-waves"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72-flexural-gravity.png)

**[Figure 1](#1/a/image-phase-and-group-velocities-of-flexural-gravity-waves-compared-with-open-water-waves). Phase and group velocities of flexural-gravity waves compared with open-water waves**.

The plotted parameters are illustrative rather than measured at the observation site. They give a [group-velocity minimum of a flexural-gravity wave](../../../../../../group-velocity-minimum-of-a-flexural-gravity-wave.md) near $15.1\,\mathrm{m\,s^{-1}}$ at period $17.6\,\mathrm s$. **There is no arbitrarily slow wave-energy branch under a continuous elastic sheet.** Energy put into a localized disturbance travels away at at least this minimum [group velocity](../../../../../../group-velocity.md); a slowly moving wind system cannot retain a [wave packet](../../../../../../wave-packet.md) indefinitely beneath itself. This reduces the opportunity for sustained local growth compared with slow, short open-water waves, and the continuous cover also prevents direct wind forcing of an exposed water surface. Incoming long swell can still propagate.

A [group-velocity minimum of a flexural-gravity wave](../../../../../../group-velocity-minimum-of-a-flexural-gravity-wave.md) is not by itself a universal minimum wind speed for wave generation. A steadily translating forcing pattern requires a [phase velocity](../../../../../../phase-velocity.md) matching its translation speed, so the minimum of $c_p$, not $c_g$, supplies the corresponding resonance threshold. Random wind forcing, dissipation and aerodynamic coupling must be specified before making an absolute generation claim.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
