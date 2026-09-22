<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume a nonrotating, nonmagnetic equilibrium, inviscid adiabatic perturbations, and no dissipation. Let $g=\phi'(R)>0$, so [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) is $p'=-\rho g$. Use $\boldsymbol\xi e^{i\omega t}$ for the [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md). To avoid a source ambiguity, write [Eulerian fluid perturbations](../../../../../eulerian-fluid-perturbation.md) as $p_1,\rho_1,\phi_1$, and use $\Delta$ for quantities following the displaced material element, as in [Eulerian and Lagrangian fluid perturbations](../../../../../eulerian-and-lagrangian-fluid-perturbations.md). They are related by $\Delta p=p_1+\xi_Rp'$ and similarly for [mass density](../../../../../density.md) and potential.

The printed identity needs two corrections: its compression denominator must be **$\gamma p$, not $\gamma\rho$**, and the [pressure](../../../../../pressure.md) and potential appearing in this form of the identity must be **[Eulerian fluid perturbations](../../../../../eulerian-fluid-perturbation.md)**. The printed denominator has the wrong dimensions for an [energy density](../../../../../energy-density.md). The claimed Lagrangian interpretation does not produce the displayed buoyancy-compression split; the following derivation specifies the consistent version.

Linearized [mass conservation](../../../../../mass-conservation.md), the adiabatic relation, and the [Poisson equation](../../../../../poisson-equation.md) give

$$
\boxed{\rho_1=-\nabla\cdot(\rho\boldsymbol\xi),\qquad \Delta p=-\gamma p\nabla\cdot\boldsymbol\xi,\qquad \nabla^2\phi_1=4\pi G\rho_1.}
$$

Consequently $p_1=-\gamma p\nabla\cdot\boldsymbol\xi-\xi_Rp'$. Linearizing the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) about the static star gives the [linear adiabatic stellar oscillation equations](../../../../../linear-adiabatic-stellar-oscillation-equations.md)

$$
-\omega^2\rho\boldsymbol\xi=-\nabla p_1-\rho_1\nabla\phi-\rho\nabla\phi_1.
$$

Require regularity at the center, a vanishing Lagrangian surface [pressure](../../../../../pressure.md), and the usual matching to a decaying exterior gravitational potential. Because $p$ and $\rho$ vanish at the surface, the [pressure](../../../../../pressure.md) boundary term vanishes for regular displacements; compactly supported trials also suffice below. The perturbed [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) solves Laplace's equation outside the star and must be included there when its field energy is computed.

Multiply the momentum equation by $-\boldsymbol\xi^*$ and integrate. The [pressure](../../../../../pressure.md) term is $-\int_Vp_1\nabla\cdot\boldsymbol\xi^*\,dV$. Let $d=\nabla\cdot\boldsymbol\xi$. The adiabatic relation and [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) imply

$$
d=\frac{\rho g\xi_R-p_1}{\gamma p},\qquad \rho_1=\frac{\rho p_1}{\gamma p}-\left(\frac{\rho^2g}{\gamma p}+\rho'\right)\xi_R.
$$

The [pressure](../../../../../pressure.md) and equilibrium-gravity terms then combine pointwise as

$$
-p_1d^*+g\rho_1\xi_R^*=\frac{|p_1|^2}{\gamma p}-\left(\frac{\rho^2g^2}{\gamma p}+g\rho'\right)|\xi_R|^2=\frac{|p_1|^2}{\gamma p}+\rho N^2|\xi_R|^2,
$$

where $N^2=g[(1/\gamma)p'/p-\rho'/\rho]$ is the [stellar buoyancy frequency](../../../../../stellar-buoyancy-frequency.md). The potentially troublesome cross terms cancel exactly.

For the perturbed [self-gravity](../../../../../self-gravity.md) term, integration by parts gives

$$
\int_V\rho\boldsymbol\xi^*\cdot\nabla\phi_1\,dV=\int_V\rho_1^*\phi_1\,dV=\frac1{4\pi G}\int_{\mathbb R^3}\phi_1\nabla^2\phi_1^*\,dV=-\frac1{4\pi G}\int_{\mathbb R^3}|\nabla\phi_1|^2\,dV.
$$

Thus the corrected [stellar displacement energy identity](../../../../../stellar-displacement-energy-identity.md) is

$$
\boxed{\omega^2\int_V\rho|\boldsymbol\xi|^2\,dV=-\frac1{4\pi G}\int_{\mathbb R^3}|\nabla\phi_1|^2\,dV+\int_V\left(\frac{|p_1|^2}{\gamma p}+\rho N^2|\xi_R|^2\right)dV.}
$$

The right side is a real [quadratic form](../../../../../quadratic-form.md). With these conservative [boundary conditions](../../../../../boundary-condition.md), the force operator is a [self-adjoint operator](../../../../../self-adjoint-operator.md). Its [Rayleigh quotient](../../../../../rayleigh-quotient.md) characterizes squared mode frequencies, and a negative admissible trial quotient proves an unstable spectral component; it does not require the trial displacement itself to be an exact [eigenfunction](../../../../../eigenfunction.md).

For a generic compressive disturbance of scale $\ell$ in a region with slowly varying equilibrium coefficients, estimate $\rho_1\sim\rho\xi/\ell$, $p_1\sim\gamma p\xi/\ell$ and $\phi_1\sim4\pi G\rho_1\ell^2$. The [self-gravity](../../../../../self-gravity.md) and compression energy densities have orders

$$
|E_g|/V\sim4\pi G\rho^2\xi^2,\qquad E_p/V\sim\rho c_s^2\xi^2/\ell^2,\qquad \frac{|E_g|}{E_p}\sim\frac{4\pi G\rho\ell^2}{c_s^2},
$$

with [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) $c_s^2=\gamma p/\rho$. Under the plausible stellar estimate $c_s^2\sim G\bar\rho a^2$, global modes can have comparable gravity and [pressure](../../../../../pressure.md) contributions, while their ratio for small-scale compressive modes is of order $(\rho/\bar\rho)(\ell/a)^2$. Thus perturbations with $\ell\ll c_s/\sqrt{4\pi G\rho}$ admit the [Cowling approximation](../../../../../cowling-approximation.md). This estimate compares two nonzero compressive terms; it cannot alone justify neglecting gravity for a trial deliberately chosen to have $p_1=0$.

For an explicit convective trial, choose $c<d<e<b$ and a nonzero smooth bump

$$
f(R)=\begin{cases}\varepsilon\exp\!\left[-\dfrac{(e-d)^2}{(R-d)(e-R)}\right],&d<R<e,\\0,&\text{otherwise.}\end{cases}
$$

Let $Y$ be a normalized [spherical harmonic](../../../../../spherical-harmonic.md) of degree $\ell\geq1$, let $L=\ell(\ell+1)$, and let $\nabla_\Omega$ be the unit-sphere gradient. The [pressure-free localized stellar convective trial](../../../../../pressure-free-localized-stellar-convective-trial.md) is

$$
\boxed{\boldsymbol\xi=fY\mathbf e_R+h\nabla_\Omega Y,\qquad h=\frac R L\left[\frac{(R^2f)'}{R^2}-\frac{\rho g}{\gamma p}f\right].}
$$

It is supported away from the center and surface, so it satisfies every needed mechanical boundary condition. Since $\Delta_\Omega Y=-LY$,

$$
\nabla\cdot\boldsymbol\xi=\left[\frac{(R^2f)'}{R^2}-\frac LRh\right]Y=\frac{\rho g}{\gamma p}fY.
$$

Therefore $p_1=-\gamma p\nabla\cdot\boldsymbol\xi+\rho g\xi_R=0$ exactly. Its [buoyancy](../../../../../buoyancy.md) energy is $\int_d^e\rho N^2R^2|f|^2dR<0$, whereas its kinetic norm $\int_d^e\rho R^2(|f|^2+L|h|^2)dR$ is positive. In the [Cowling approximation](../../../../../cowling-approximation.md) this gives a negative [Rayleigh quotient](../../../../../rayleigh-quotient.md), and hence **$N^2<0$ in an interior shell implies convective instability**. Retaining perturbed [self-gravity](../../../../../self-gravity.md) only adds a nonpositive term, so the same trial proves instability in the full conservative problem too.

There is also a quantitative small-scale check for this very trial. Its [mass density](../../../../../density.md) amplitude is $\rho_1=(\rho N^2/g)fY$, independent of $\ell$. Write $\rho_1=s(R)Y$ and $\phi_1=F(R)Y$. The radial [Poisson equation](../../../../../poisson-equation.md) gives

$$
A=\int_0^\infty\left(R^2|F'|^2+L|F|^2\right)dR=-4\pi G\int_0^\infty R^2F^*s\,dR.
$$

By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $A\leq4\pi G(\int R^4|s|^2dR)^{1/2}(A/L)^{1/2}$, and so the [angular-degree bound on perturbed stellar self-gravity](../../../../../angular-degree-bound-on-perturbed-stellar-self-gravity.md) is

$$
|E_g|=\frac A{4\pi G}\leq\frac{4\pi G}{\ell(\ell+1)}\int_d^eR^4|s|^2dR.
$$

It tends to zero with horizontal scale $R/\ell$, while the strictly negative [buoyancy](../../../../../buoyancy.md) integral is fixed. This justifies the small-scale neglect of gravity even though the trial's compression term vanishes.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
