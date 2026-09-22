<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Rotating Rayleigh-Bénard convection](../../../../../rotating-rayleigh-benard-convection.md) combines buoyancy-driven instability with the [Coriolis force](../../../../../coriolis-force.md). Consider a plane layer of depth $d$ rotating uniformly about the vertical axis, heated from below. Adopt the [Boussinesq approximation](../../../../../boussinesq-approximation.md), fixed boundary temperatures and, for explicit formulas, impermeable [stress-free boundary conditions](../../../../../stress-free-boundary-condition.md). The [conductive state of Rayleigh-Bénard convection](../../../../../conductive-state-of-rayleigh-benard-convection.md) is motionless with a linear temperature profile. The dimensionless controls are the [Rayleigh number](../../../../../rayleigh-number.md), [Prandtl number](../../../../../prandtl-number.md) and [Taylor number](../../../../../taylor-number.md):

$$
\operatorname{Ra}=\frac{g\alpha_T\Delta T\,d^3}{\nu\kappa},\qquad
P=\operatorname{Pr}=\frac{\nu}{\kappa},\qquad
\operatorname{Ta}=\left(\frac{2\Omega d^2}{\nu}\right)^2.
$$

Here $\nu$ is [kinematic viscosity](../../../../../kinematic-viscosity.md) and $\kappa$ [thermal diffusivity](../../../../../thermal-diffusivity.md). In thermal-diffusion time units, linear perturbations satisfy

$$
P^{-1}\boldsymbol u_t+\sqrt{\operatorname{Ta}}\,\boldsymbol e_z\times\boldsymbol u
=-\nabla p+\nabla^2\boldsymbol u+\operatorname{Ra}\,\theta\boldsymbol e_z,
\qquad
\theta_t=w+\nabla^2\theta,\qquad\nabla\cdot\boldsymbol u=0.
$$

Rotation does no direct mechanical work, since $\boldsymbol u\cdot(\boldsymbol e_z\times\boldsymbol u)=0$, but couples vertical motion to vertical [vorticity](../../../../../vorticity.md) and changes the damping and oscillation balance.

For horizontal [wavenumber](../../../../../wavenumber.md) $k$ and vertical mode $n$, put $m=n^2\pi^2$ and $a=k^2+m$. Use $w=W\sin(n\pi z)$, $\theta=\Theta\sin(n\pi z)$ and vertical [vorticity](../../../../../vorticity.md) $\zeta=Z\cos(n\pi z)$ with growth rate $\sigma$. Curling the momentum equation and eliminating pressure gives

$$
a(\sigma/P+a)W+\sqrt{\operatorname{Ta}}\,n\pi Z
=\operatorname{Ra}k^2\Theta,\quad
(\sigma/P+a)Z=\sqrt{\operatorname{Ta}}\,n\pi W,\quad
(\sigma+a)\Theta=W.
$$

Their determinant, without dividing by a possibly zero factor, is the [rotating-convection growth-rate polynomial](../../../../../rotating-convection-growth-rate-polynomial.md)

$$
(\sigma+a)\left[a(\sigma/P+a)^2+\operatorname{Ta}m\right]
-\operatorname{Ra}k^2(\sigma/P+a)=0.
$$

This makes the [linear stability analysis](../../../../../linear-stability.md) question precise: onset occurs when a root reaches zero real part and all other modes still decay.

A stationary neutral root has $\sigma=0$, giving

$$
\boxed{R_s(k,n)=\frac{a^3+\operatorname{Ta}m}{k^2}.}
$$

Rotation raises this stationary threshold. An oscillatory neutral root has $\sigma=i\varpi$ with $\varpi\ne0$. Real-imaginary separation gives the [oscillatory neutral curve of rotating convection](../../../../../oscillatory-neutral-curve-of-rotating-convection.md)

$$
\boxed{\varpi^2=P^2\left[
\frac{1-P}{1+P}\frac{\operatorname{Ta}m}{a}-a^2\right],\qquad
R_o(k,n)=\frac{2(1+P)a^3+2P^2\operatorname{Ta}m/(1+P)}{k^2}.}
$$

This branch is admissible only when $\varpi^2>0$, requiring $P<1$ and sufficiently strong rotation. The restoring [Coriolis force](../../../../../coriolis-force.md) coupling permits an inertial/thermal oscillation whose phase-lagged buoyancy can overcome dissipation. At large $P$, temperature and momentum diffusion do not permit that overstability mechanism at primary onset, so the exchange of stabilities is stationary. The actual threshold is the minimum of the stationary and admissible oscillatory curves over all allowed modes, not an arbitrary formal value of $R_o$. Rigid plates require a different vertical eigenproblem and [Ekman layers](../../../../../ekman-layer.md), so the explicit free-slip numbers are not universal.

At large [Taylor number](../../../../../taylor-number.md), the first vertical mode is selected in the ideal plane layer. Let $t=k^2,m=\pi^2$. Minimizing the stationary curve gives

$$
(t+m)^2(2t-m)=\operatorname{Ta}m.
$$

Thus the [stationary neutral curve of rotating convection](../../../../../stationary-neutral-curve-of-rotating-convection.md) has

$$
\boxed{k_{s,c}\sim(\operatorname{Ta}\pi^2/2)^{1/6},\qquad
R_{s,c}\sim3(\operatorname{Ta}\pi^2/2)^{2/3}.}
$$

The physical horizontal wavelength is $2\pi d/k_c$, hence decreases as $\operatorname{Ta}^{-1/6}$; its prefactor depends on the boundary convention. Thin nearly vertical cells reconcile the strong [Coriolis force](../../../../../coriolis-force.md) constraint with viscous and thermal diffusion. The oscillatory minimization replaces the right side of the [wavenumber](../../../../../wavenumber.md) equation by $P^2\operatorname{Ta}m/(1+P)^2$, giving the same [Taylor number](../../../../../taylor-number.md) exponent at fixed positive $P$. Where its frequency remains admissible,

$$
\frac{R_{o,c}}{R_{s,c}}\sim\frac{2P^{4/3}}{(1+P)^{1/3}}.
$$

Equality is $8P^4-P-1=0$, whose positive root is approximately **$P_*=0.6766$**. Accordingly, for sufficiently rapid rotation in this free-slip problem, $P<P_*$ selects oscillatory onset and $P>P_*$ stationary onset. The weaker condition $P<1$ is only necessary for an oscillatory neutral mode; it does not by itself identify the first instability. Finite [Taylor number](../../../../../taylor-number.md), finite lateral geometry, allowed discrete wave numbers and plate conditions change the selection.

For the [counterpropagating Hopf amplitudes in rotating convection](../../../../../counterpropagating-hopf-amplitudes-in-rotating-convection.md) near a simple oscillatory onset, the [Hopf bifurcation](../../../../../hopf-bifurcation.md) produces slow complex amplitudes for counterpropagating roll waves. After separating the fast carrier oscillation, symmetry permits the cubic equations

$$
\dot Z_\pm=rZ_\pm-
\left(g_s|Z_\pm|^2+g_c|Z_\mp|^2\right)Z_\pm,
$$

with generally complex coefficients; an $i\omega_0 Z_\pm$ term restores the fast frequency if desired. The real parts govern amplitude saturation and the imaginary parts give nonlinear frequency shifts. Write $a_s=\operatorname{Re}g_s$, $a_c=\operatorname{Re}g_c$. For a [travelling wave](../../../../../travelling-wave.md) from a [supercritical bifurcation](../../../../../supercritical-bifurcation.md) with only one amplitude nonzero, $|Z_\pm|^2=r/a_s$ with $r,a_s>0$, and the competing wave's growth rate is $r(1-a_c/a_s)$. It is amplitude-stable against that competitor when $a_c>a_s$. A [standing wave](../../../../../standing-wave.md) has equal intensities $r/(a_s+a_c)$; provided this is positive, its intensity-difference mode is stable when $a_s>a_c$. Temporal and spatial phase symmetries leave neutral phase directions, so these are orbital/amplitude stability statements, not decay of every phase displacement.

These coefficients follow from nonlinear interactions and the [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) obtained by projection onto an [adjoint eigenfunction](../../../../../adjoint-eigenfunction.md); symmetry alone cannot decide their signs. A negative saturating coefficient gives [subcritical bifurcation](../../../../../subcritical-bifurcation.md) behavior requiring higher-order terms. Spatial modulation leads to coupled [complex Ginzburg–Landau equations](../../../../../complex-ginzburg-landau-equation.md) with [group velocities](../../../../../group-velocity.md) and diffusion; phase instabilities, mean-flow coupling and differently oriented rolls can destabilize a wave stable in the restricted two-amplitude system. A [weakly nonlinear expansion](../../../../../weakly-nonlinear-expansion.md) of oscillations therefore predicts [travelling waves](../../../../../travelling-wave.md) or [standing waves](../../../../../standing-wave.md), frequency shifts, modulation and possible secondary mode competition, not a unique universal periodic state.

The [Küppers–Lortz instability](../../../../../kuppers-lortz-instability.md) is a different route to time dependence: it destabilizes steady saturated rolls against oblique roll perturbations. For stationary-roll amplitudes of orientations $\phi_j$, a leading competition system has

$$
\dot A_i=rA_i-g_0|A_i|^2A_i
-\sum_{j\ne i}g(\phi_j-\phi_i)|A_j|^2A_i.
$$

A pure roll has $|A_i|^2=r/g_0$ with $g_0>0$. An infinitesimal new roll at relative angle $\vartheta$ grows at

$$
\boxed{\lambda_{\rm inv}=r\left[1-\frac{g(\vartheta)}{g_0}\right].}
$$

For sufficiently strong rotation in appropriate boundary and [Prandtl number](../../../../../prandtl-number.md) regimes, some finite oblique angle has $g(\vartheta)<g_0$, so a steady roll is unstable arbitrarily close above its stationary onset. Rotation is handed and allows $g(\vartheta)\ne g(-\vartheta)$, so replacement of one roll by another can favor a definite cyclic sense. Three or more competing orientations can form a [heteroclinic cycle](../../../../../heteroclinic-cycle.md); whether it attracts depends on contraction/expansion rates and other modes. Noise, spatially varying domains and modulation can turn this competition into repeated orientation switching and irregular patterns.

The invading rolls are three-dimensional disturbances even when the original straight roll is described by a two-dimensional section. The finite-angle [Küppers–Lortz instability](../../../../../kuppers-lortz-instability.md) mechanism should also be distinguished from the [small-angle instability of rotating convection rolls](../../../../../small-angle-instability-of-rotating-convection-rolls.md) mediated by large-scale mean flow at finite [Prandtl number](../../../../../prandtl-number.md). Numerical thresholds and favored angles depend on mechanical boundaries and material parameters; the essential criterion is the cross-coupling relative to self-saturation. **Rotation both changes primary onset and wavelength, and can prevent the resulting steady roll pattern from remaining a stable nonlinear state.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
