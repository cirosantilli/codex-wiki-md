<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take a static, nonrotating, nonmagnetic spherical equilibrium with $\nabla P=-\rho\nabla\Phi$ and $\nabla^2\Phi=4\pi G\rho$. Use a [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $\boldsymbol\xi(\mathbf r)e^{-i\omega t}$. Write $p_1,\rho_1,\phi_1$ for [Eulerian fluid perturbations](../../../../../eulerian-fluid-perturbation.md). The [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md) and corresponding [mass density](../../../../../density.md) change obey $\Delta P=p_1+\boldsymbol\xi\cdot\nabla P$, $\Delta\rho=\rho_1+\boldsymbol\xi\cdot\nabla\rho$. Linearizing [mass conservation](../../../../../mass-conservation.md), the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) and [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) gives

$$
\boxed{\begin{aligned}
\rho_1&=-\nabla\cdot(\rho\boldsymbol\xi),\\
-\omega^2\rho\boldsymbol\xi&=-\nabla p_1-\rho_1\nabla\Phi-\rho\nabla\phi_1,\\
\nabla^2\phi_1&=4\pi G\rho_1.
\end{aligned}}
$$

There is no equilibrium acceleration to multiply a perturbed [mass density](../../../../../density.md). The [adiabatic process](../../../../../adiabatic-process.md) condition, with composition carried by the parcel, closes the system:

$$
\boxed{\frac{\Delta P}{P}=\Gamma_1\frac{\Delta\rho}{\rho},\qquad\Delta\rho=-\rho\nabla\cdot\boldsymbol\xi,\qquad p_1=-\Gamma_1P\nabla\cdot\boldsymbol\xi-\boldsymbol\xi\cdot\nabla P.}
$$

These are the complete [linear adiabatic stellar oscillation equations](../../../../../linear-adiabatic-stellar-oscillation-equations.md), including the perturbation of self-gravity. Neglect of heat exchange is appropriate when oscillation periods are short compared with relevant thermal relaxation times; it does not determine nonadiabatic excitation or damping.

For the pressure and buoyancy modes, separate angular dependence using [spherical harmonics](../../../../../spherical-harmonic.md):

$$
\boldsymbol\xi=\xi_r(r)Y_\ell^m\hat{\mathbf r}+\xi_h(r)\nabla_\Omega Y_\ell^m,\qquad (p_1,\rho_1,\phi_1)=(p_\ell,\rho_\ell,\phi_\ell)Y_\ell^m.
$$

The horizontal amplitude $\xi_h$ has dimensions of length. Angular differentiation gives $\nabla\cdot\boldsymbol\xi=[r^{-2}(r^2\xi_r)'-\ell(\ell+1)\xi_h/r]Y_\ell^m$, and tangential momentum gives $\omega^2r\xi_h=p_\ell/\rho+\phi_\ell$. Define the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md), [stellar buoyancy frequency](../../../../../stellar-buoyancy-frequency.md) and [Lamb frequency](../../../../../lamb-frequency.md) by

$$
c_s^2=\frac{\Gamma_1P}\rho,\qquad N^2=g\left(\frac1{\Gamma_1}\frac{d\log P}{dr}-\frac{d\log\rho}{dr}\right),\qquad S_\ell^2=\frac{\ell(\ell+1)c_s^2}{r^2}.
$$

The adiabatic [mass density](../../../../../density.md) relation becomes $\rho_\ell/\rho=p_\ell/(\rho c_s^2)+(N^2/g)\xi_r$. Substitution produces a radial form of the full oscillation equations for nonzero $\omega$:

$$
\begin{aligned}
\frac{d\xi_r}{dr}&=\left(\frac g{c_s^2}-\frac2r\right)\xi_r+\frac1{\rho c_s^2}\left(\frac{S_\ell^2}{\omega^2}-1\right)p_\ell+\frac{\ell(\ell+1)}{r^2\omega^2}\phi_\ell,\\
\frac{dp_\ell}{dr}&=\rho(\omega^2-N^2)\xi_r-\frac g{c_s^2}p_\ell-\rho\frac{d\phi_\ell}{dr},\\
\frac1{r^2}\frac d{dr}\left(r^2\frac{d\phi_\ell}{dr}\right)-\frac{\ell(\ell+1)}{r^2}\phi_\ell&=4\pi G\left(\frac{p_\ell}{c_s^2}+\rho\frac{N^2}{g}\xi_r\right).
\end{aligned}
$$

The apparent $N^2/g$ factor is evaluated through its defining gradient at the centre rather than by dividing two zeros.

Regularity at the centre excludes singular solutions. At a free surface the [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md) vanishes, $\Delta P=0$; outside the star the gravitational perturbation decays as $r^{-\ell-1}$. For a model with [mass density](../../../../../density.md) tending to zero at its surface, continuity of $\phi_\ell$ and its radial derivative gives $\phi_\ell'(R)=-(\ell+1)\phi_\ell(R)/R$. If the equilibrium [mass density](../../../../../density.md) jumps to vacuum, include the displaced-surface mass sheet: the outward-minus-inward derivative jump is $4\pi G\rho(R)\xi_r(R)$, so the interior condition is $\phi_\ell'(R)=-(\ell+1)\phi_\ell(R)/R-4\pi G\rho(R)\xi_r(R)$. An atmospheric [boundary condition](../../../../../boundary-condition.md) can replace the ideal free surface.

These conditions make $\omega^2$ an [eigenvalue](../../../../../eigenvalue.md), not an arbitrary local sound frequency. With conservative [boundary conditions](../../../../../boundary-condition.md) the adiabatic operator is [self-adjoint](../../../../../self-adjoint-operator.md), giving real $\omega^2$; negative values describe instability. The frequencies depend on $P(r),\rho(r),\Gamma_1(r)$, self-gravity, stratification and boundaries, as well as angular degree $\ell$ and radial order. In a spherical nonrotating star they are degenerate in $m$. For homologous equilibrium structures, their scale is

$$
\boxed{\omega\sim\left(\frac{GM}{R^3}\right)^{1/2};}
$$

thus the typical oscillation time measures inverse square root of mean [mass density](../../../../../density.md), while individual frequencies probe the interior [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) and [stellar buoyancy frequency](../../../../../stellar-buoyancy-frequency.md) profiles.

For radial modes, write $\xi_r=r\eta$. Eliminating the [pressure](../../../../../pressure.md) and gravitational perturbations gives the [radial stellar pulsation equation](../../../../../radial-stellar-pulsation-equation.md)

$$
\boxed{\frac d{dr}\left(\Gamma_1Pr^4\frac{d\eta}{dr}\right)+r^3\frac d{dr}[(3\Gamma_1-4)P]\eta+\rho r^4\omega^2\eta=0.}
$$

This is a [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md). Multiplication by $\eta$ and integration, with vanishing boundary terms, gives its [Rayleigh quotient](../../../../../rayleigh-quotient.md)

$$
\omega^2=\frac{\int_0^R\Gamma_1Pr^4(\eta')^2\,dr-\int_0^Rr^3[(3\Gamma_1-4)P]'\eta^2\,dr}{\int_0^R\rho r^4\eta^2\,dr}.
$$

For constant $\Gamma_1>4/3$, $P'<0$ makes both numerator contributions nonnegative. At $\Gamma_1=4/3$, a homologous displacement is neutral; for constant $\Gamma_1<4/3$ the same trial displacement makes the quotient negative. For the [uniform-density stellar model](../../../../../uniform-density-stellar-model.md), $\eta=$ constant is an exact mode and $\omega^2=(3\Gamma_1-4)GM/R^3$. With varying $\Gamma_1$, the integral criterion, rather than a universal pointwise threshold, controls radial stability.

The [Cowling approximation](../../../../../cowling-approximation.md) neglects $\phi_\ell$ while retaining the equilibrium gravitational field. It is useful for short-wavelength modes, but is not needed for the full derivation above. In a locally slowly varying region, take both remaining amplitudes proportional to $e^{i\int k_rdr}$ and retain the leading derivative terms. Then

$$
ik_r\xi_r\simeq\frac{S_\ell^2/\omega^2-1}{\rho c_s^2}p_\ell,\qquad ik_rp_\ell\simeq\rho(\omega^2-N^2)\xi_r.
$$

Eliminating either amplitude gives the [acoustic-gravity propagation relation](../../../../../acoustic-gravity-propagation-relation.md)

$$
\boxed{k_r^2\simeq\frac{(\omega^2-S_\ell^2)(\omega^2-N^2)}{c_s^2\omega^2}.}
$$

Positive $k_r^2$ is oscillatory propagation; negative $k_r^2$ means an [evanescent wave](../../../../../evanescent-wave.md). The high-frequency branch, $\omega^2>S_\ell^2,N^2$, describes [stellar acoustic modes](../../../../../stellar-acoustic-mode.md), restored chiefly by compressibility and [pressure](../../../../../pressure.md). At frequencies well above $N$, this gives $\omega^2\simeq c_s^2[k_r^2+\ell(\ell+1)/r^2]$. The low-frequency propagating branch in stable stratification, $\omega^2<N^2,S_\ell^2$, instead describes [stellar gravity modes](../../../../../stellar-gravity-mode.md), restored by [buoyancy](../../../../../buoyancy.md). At $\ell=0$ there is no such nonradial gravity-wave cavity.

A [stellar acoustic mode](../../../../../stellar-acoustic-mode.md) is trapped between an inner turning point near $\omega=S_\ell$ and an outer reflecting region. Low-$\ell$ modes penetrate deeply; radial modes reach the centre. Higher-degree modes turn farther out. Standing waves require the [WKB quantization condition](../../../../../wkb-quantization-condition.md)

$$
\int_{r_1}^{r_2}k_r\,dr\simeq\pi(n+\alpha),
$$

where the phase $\alpha$ depends on the central or turning-point behaviour and surface reflection. For high radial order and small degree, the leading acoustic travel-time result is the [large frequency separation](../../../../../large-frequency-separation.md)

$$
\boxed{\Delta\nu\simeq\left(2\int_0^R\frac{dr}{c_s}\right)^{-1},\qquad\nu_{n\ell}\simeq\Delta\nu\left(n+\frac\ell2+\varepsilon\right),\qquad\nu=\frac\omega{2\pi}.}
$$

The $\ell/2$ term is the leading central angular phase shift; smaller frequency separations depend on detailed interior gradients. The near-surface [mass density](../../../../../density.md) stratification sets the [acoustic cutoff frequency](../../../../../acoustic-cutoff-frequency.md). In a plane-parallel isothermal atmosphere with [mass density](../../../../../density.md) scale height $H_\rho$, $\omega_{\rm ac}\simeq c_s/(2H_\rho)$. Modes below this cutoff can reflect and form a cavity; waves sufficiently above it escape and need an outgoing-wave [boundary condition](../../../../../boundary-condition.md). Nonadiabatic damping, driving and rotation alter real-star mode properties, but the adiabatic frequency problem isolates their dependence on the equilibrium structure.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
