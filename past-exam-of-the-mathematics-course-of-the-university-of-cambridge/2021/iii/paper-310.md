# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_310.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a component with constant [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state) $P=w\rho$, the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) gives

$$
\frac{d\rho}{\rho}=-3(1+w)\frac{da}{a}.
$$

Hence $\rho_i=\rho_{i,0}a^{-3(1+w_i)}$. Choose the present [scale factor](../../../cosmology.md#scale-factor-cosmology) to be $a_0=1$, so the [cosmological redshift](../../../cosmology.md#cosmological-redshift) obeys $1+z=a^{-1}$, and define the present [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) by

$$
\Omega_{i,0}=\frac{\rho_{i,0}}{\rho_{\rm crit,0}},
\qquad
\rho_{\rm crit,0}=\frac{3H_0^2}{8\pi G}.
$$

Substitution in the spatially flat [Friedmann equation](../../../cosmology.md#friedmann-equations) then yields

$$
\boxed{H(z)=H_0\left[\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}\right]^{1/2}}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) and $H=\dot a/a$ give the [deceleration parameter](../../../cosmology.md#deceleration-parameter)

$$
q=-\frac{\ddot a}{aH^2}
=\frac{4\pi G}{3H^2}\sum_i\rho_i(1+3w_i)
=\boxed{\frac12\sum_i\Omega_i(z)(1+3w_i)}.
$$

An [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) contains only [pressureless matter](../../../cosmology.md#pressureless-matter), so $q_0=1/2$ and cannot explain the observed negative value. For the stated [Lambda-CDM model](../../../cosmology.md#lambda-cdm-model),

$$
q_0=\frac12\left[0.3+0.7(1-3)\right]=-0.55,
$$

so its [cosmological constant](../../../cosmology.md#cosmological-constant) produces the required [accelerating universe](../../../cosmology.md#accelerating-expansion-of-the-universe).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [age of an FLRW universe](../../../cosmology.md#age-of-an-flrw-universe) follows from $dt=da/(aH)$. Neglecting radiation and spatial curvature gives

$$
t_0=\frac1{H_0}\int_0^1
\frac{da}{a\sqrt{\Omega_{m,0}a^{-3}+\Omega_{\Lambda,0}}}
=\frac1{H_0}\int_0^1
\frac{a^{1/2}\,da}{\sqrt{\Omega_{m,0}+\Omega_{\Lambda,0}a^3}}.
$$

For an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $\Omega_{m,0}=1$ and $\Omega_{\Lambda,0}=0$, so

$$
\boxed{t_0=H_0^{-1}\int_0^1a^{1/2}\,da=\frac{2}{3}H_0^{-1}}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The measured [Hubble time](../../../cosmology.md#hubble-time) would give the Einstein-de Sitter age

$$
t_0=\frac23(14\ {\rm Gyr})\simeq9.3\ {\rm Gyr},
$$

which is less than the measured $12\ {\rm Gyr}$ age of stars that must themselves be younger than the universe. The measurements are therefore incompatible with an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe). For the stated spatially flat [Lambda-CDM model](../../../cosmology.md#lambda-cdm-model), direct evaluation of the preceding integral gives

$$
H_0t_0=\frac{2}{3\sqrt{0.7}}\operatorname{arsinh}\sqrt{\frac{0.7}{0.3}}\simeq0.964,
$$

and hence $t_0\simeq13.5\ {\rm Gyr}$. The period of [accelerating expansion](../../../cosmology.md#accelerating-expansion-of-the-universe) caused by the [cosmological constant](../../../cosmology.md#cosmological-constant) therefore allows an age consistent with the stellar lower bound.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a spatially homogeneous canonical [scalar field](../../../quantum-field-theory.md#scalar-field), spatial derivatives vanish. Reading the time and spatial components of its [energy-momentum tensor](../../../general-relativity.md#stress-energy-tensor) in the comoving frame gives

$$
\boxed{\rho_\phi=\frac12\dot\phi^2+V(\phi)},
\qquad
\boxed{P_\phi=\frac12\dot\phi^2-V(\phi)}.
$$

**Thus the kinetic term contributes equally to [energy density](../../../statistical-physics.md#energy-density) and pressure, whereas the [scalar potential](../../../quantum-field-theory.md#scalar-potential) contributes negative pressure.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Substitution of these expressions into the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) gives

$$
\dot\phi\left(\ddot\phi+3H\dot\phi+V'(\phi)\right)=0.
$$

Continuity through a turning point therefore yields the homogeneous [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation)

$$
\boxed{\ddot\phi+3H\dot\phi=-V'(\phi)}.
$$

During [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation), the acceleration and kinetic-energy terms are negligible. In terms of the [reduced Planck mass](../../../physics.md#reduced-planck-mass), the approximate evolution is

$$
\boxed{3H\dot\phi\simeq-V'(\phi)},
\qquad
\boxed{H^2\simeq\frac{V(\phi)}{3M_{\rm Pl}^2}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

This is the potential of [Starobinsky inflation](../../../cosmic-inflation.md#starobinsky-inflation). Put $b=\sqrt{2/3}/M_{\rm Pl}$ and $y=e^{-b\phi}$, so $V=V_0(1-y)^2$. Its [potential slow-roll parameter](../../../cosmic-inflation.md#potential-slow-roll-parameter) and [second potential slow-roll parameter](../../../cosmic-inflation.md#second-potential-slow-roll-parameter) are

$$
\epsilon_V=\frac{M_{\rm Pl}^2}{2}\left(\frac{V'}V\right)^2
=\frac43\frac{y^2}{(1-y)^2},
$$



$$
\eta_V=M_{\rm Pl}^2\frac{V''}V
=\frac43\frac{-y+2y^2}{(1-y)^2}.
$$

At large positive $\phi$, $y\ll1$, so both $\epsilon_V$ and $|\eta_V|$ are small and [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation) is possible. Near the minimum, a [Taylor expansion](../../../calculus.md#taylor-expansion) gives $1-y\simeq b\phi$ and hence

$$
\epsilon_V\simeq\eta_V\simeq\frac{2M_{\rm Pl}^2}{\phi^2}.
$$

They are large for $|\phi|\ll M_{\rm Pl}$, so that region cannot sustain slow roll.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Near the minimum, the [Taylor expansion](../../../calculus.md#taylor-expansion) of the potential is

$$
V(\phi)\simeq V_0b^2\phi^2=\frac12m^2\phi^2,
\qquad
m^2=\frac{4V_0}{3M_{\rm Pl}^2}.
$$

Neglecting [Hubble friction](../../../cosmology.md#hubble-friction) during one short oscillation reduces the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) to the [harmonic oscillator equation](../../../classical-mechanics.md#simple-harmonic-motion)

$$
\boxed{\ddot\phi+m^2\phi\simeq0}.
$$

The [virial theorem](../../../classical-mechanics.md#virial-theorem) gives $\langle\dot\phi^2/2\rangle=\langle V\rangle$, so $\langle P_\phi\rangle=0$. Restoring the slow cosmological damping in the averaged [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) gives

$$
\dot{\langle\rho_\phi\rangle}+3H\langle\rho_\phi\rangle=0,
\qquad
\boxed{\langle\rho_\phi\rangle\propto a^{-3}}.
$$

The coherently oscillating inflaton therefore behaves as [pressureless matter](../../../cosmology.md#pressureless-matter).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The matter-like scaling is special to a quadratic minimum. More generally, the [effective equation of state of an oscillating scalar field](../../../cosmic-inflation.md#effective-equation-of-state-of-an-oscillating-scalar-field) in $V\propto|\phi|^n$ is

$$
\langle w\rangle=\frac{n-2}{n+2},
\qquad
\rho_\phi\propto a^{-6n/(n+2)}.
$$

For example, a quartic minimum has $\langle w\rangle=1/3$ and redshifts like [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology). Potentials without a stable minimum, oscillations whose period is not short relative to the [Hubble time](../../../cosmology.md#hubble-time), and significant decay of the inflaton into other particles also invalidate the matter-like argument.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

At [neutrino decoupling](../../../cosmology.md#neutrino-decoupling), neutrinos, electrons, positrons, and [photons](../../../quantum-mechanics.md#photon) share one temperature. The neutrinos subsequently free stream, so $T_\nu\propto a^{-1}$. In the still-coupled electromagnetic plasma, the effective entropy degrees of freedom change during [electron-positron annihilation in cosmology](../../../cosmology.md#electron-positron-annihilation-in-cosmology) from

$$
g_{*s,{\rm before}}=2+\frac78(2+2)=\frac{11}{2}
$$

to $g_{*s,{\rm after}}=2$. Separate [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) in that plasma gives $g_{*s}T_\gamma^3a^3={\rm constant}$, while $T_\nu a$ remains constant. Consequently the [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) temperature obeys

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac4{11}\right)^{1/3}}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For one species with two internal states, the [relic-neutrino energy density](../../../cosmology.md#relic-neutrino-energy-density) obtained from the frozen [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) is

$$
\rho_\nu=2\int\frac{d^3p}{(2\pi)^3}
\frac{\sqrt{p^2+m_\nu^2}}{e^{ap/T_\nu}+1}
=\frac1{\pi^2}\int_0^\infty
\frac{p^2\sqrt{p^2+m_\nu^2}}{e^{ap/T_\nu}+1}\,dp.
$$

In the relativistic limit, set $x=ap/T_\nu$ and use the standard [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) integral

$$
\int_0^\infty\frac{x^3}{e^x+1}\,dx=\frac{7\pi^4}{120}.
$$

This gives

$$
\boxed{\rho_\nu=\frac{7\pi^2}{120}\left(\frac{T_\nu}{a}\right)^4}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

At $T_\nu/a\ll m_\nu$, the [Taylor expansion](../../../calculus.md#taylor-expansion) of the relativistic energy is $\sqrt{p^2+m_\nu^2}=m_\nu+p^2/(2m_\nu)+O(p^4/m_\nu^3)$. The number density is

$$
n_\nu=\frac1{\pi^2}\left(\frac{T_\nu}{a}\right)^3
\int_0^\infty\frac{x^2}{e^x+1}\,dx
=\frac{3\zeta(3)}{2\pi^2}\left(\frac{T_\nu}{a}\right)^3.
$$

The ratio of the next momentum moment to this one is

$$
\frac{\int_0^\infty x^4/(e^x+1)\,dx}
{\int_0^\infty x^2/(e^x+1)\,dx}
=\frac{15\zeta(5)}{\zeta(3)}.
$$

Therefore

$$
\boxed{\rho_\nu\simeq n_\nu m_\nu
\left[1+\frac{15\zeta(5)}{2\zeta(3)}
\left(\frac{T_\nu}{am_\nu}\right)^2\right]},
$$

so $\boxed{F=15\zeta(5)/(2\zeta(3))\simeq6.47}$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Comparing the correction in part c with the nonrelativistic kinetic energy $m_\nu\langle v^2\rangle/2$ gives the characteristic late-time [speed](../../../classical-mechanics.md#speed)

$$
\boxed{v_{\rm rms}\simeq
\sqrt{\frac{15\zeta(5)}{\zeta(3)}}\frac{T_\nu}{am_\nu}
\simeq3.60\frac{T_\nu}{am_\nu}}.
$$

**Thus the [late-time relic-neutrino speed](../../../cosmology.md#late-time-relic-neutrino-speed) redshifts as $a^{-1}$.**

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) began free streaming at [neutrino decoupling](../../../cosmology.md#neutrino-decoupling), long before [cosmological recombination](../../../cosmology.md#recombination-cosmology), so its directional flux can retain information about density fluctuations from epochs inaccessible to the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background). Earlier decoupling does not by itself guarantee a larger [comoving radial distance](../../../cosmology.md#comoving-radial-distance). A sufficiently massive neutrino eventually becomes nonrelativistic, and its travelled distance is

$$
\chi_\nu=\int_{a_{\rm dec}}^1\frac{v(a)}{a^2H(a)}\,da,
$$

which may be smaller than the photon distance because $v(a)<c$. Hence the [cosmic neutrino background last-scattering surface](../../../cosmology.md#cosmic-neutrino-background-last-scattering-surface) need not lie beyond the [Cosmic microwave background last-scattering surface](../../../cosmology.md#cosmic-microwave-background-last-scattering-surface); it generally does for neutrinos that remain sufficiently relativistic for sufficiently long.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) obey

$$
[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k'),
\qquad
[\hat a_{\mathbf k},\hat a_{\mathbf k'}]
=[\hat a_{\mathbf k}^\dagger,\hat a_{\mathbf k'}^\dagger]=0.
$$

The [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) in their vacuum has Fourier amplitude $|f_k|^2/a^2$. After [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $|k\tau|\ll1$, and the stated [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) mode and $a=-1/(H\tau)$ give

$$
|f_k|^2\simeq\frac1{2k^3\tau^2},
\qquad
\frac{|f_k|^2}{a^2}=\frac{H^2}{2k^3}.
$$

The dimensionless [power spectrum](../../../probability-and-statistics.md#power-spectrum) is consequently

$$
\boxed{\Delta_{\delta\phi}^2(k)
=\frac{k^3}{2\pi^2}\frac{|f_k|^2}{a^2}
=\left(\frac{H}{2\pi}\right)^2}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The exact mode functions satisfy the Wronskian normalization

$$
f_kf_k^{*\prime}-f_k^*f_k'=i.
$$

Using the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) generated by the ladder-operator commutator therefore gives the exact [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
\boxed{[\hat f(\tau,\mathbf x),\hat\pi(\tau,\mathbf y)]
=i\delta^{(3)}(\mathbf x-\mathbf y)}.
$$

This remains true on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), so the exact operators do not literally commute. A claim of classical behavior must instead compare this fixed commutator with the growing statistical fluctuations, or appeal to [quantum decoherence](../../../quantum-theory.md#quantum-decoherence).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At leading order in $|k\tau|$, the inflationary [Fourier mode](../../../fourier-analysis.md#fourier-mode) and its derivative are

$$
f_k\simeq-\frac{i}{\sqrt{2k^3}\tau},
\qquad
f_k'\simeq\frac{i}{\sqrt{2k^3}\tau^2}.
$$

Thus the leading parts of $\hat f$ and $\hat\pi$ contain the same quadrature of the [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) and satisfy

$$
\hat\pi\simeq-\frac1\tau\hat f.
$$

Their commutator consequently vanishes in this leading approximation. The exact nonzero result in part b is carried by the subleading decaying mode. Relative to the rapidly growing anticommutator, its effect is suppressed by powers of $|k\tau|$, which is the squeezing captured by the [classicality parameter of a cosmological perturbation](../../../cosmic-inflation.md#classicality-parameter-of-a-cosmological-perturbation). The perturbation can therefore be treated as an effectively classical stochastic field on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale) even though its exact quantum commutator is unchanged.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The supplied superhorizon evolution equation is

$$
\frac{d\mathcal R}{d\ln a}
=-\frac{\delta P_{\rm nad}}{\bar\rho+\bar P},
\qquad
\delta P_{\rm nad}=\delta P-
\frac{\bar P'}{\bar\rho'}\delta\rho.
$$

For an [adiabatic cosmological perturbation](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions), $\delta P=(\bar P'/\bar\rho')\delta\rho$, so $\delta P_{\rm nad}=0$ and the [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) $\mathcal R$ is conserved on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale).

For photons and [cold dark matter](../../../cosmology.md#cold-dark-matter), put $A=\bar\rho_\gamma$, $C=\bar\rho_c$, and use $\bar P=A/3$, $A'=-4\mathcal H A$, and $C'=-3\mathcal H C$. Then

$$
\frac{\bar P'}{\bar\rho'}=\frac{4A}{3(4A+3C)}.
$$

The [cosmological entropy perturbation](../../../cosmic-inflation.md#cosmological-entropy-perturbation) $S=\delta_c-3\delta_\gamma/4$ implies $\delta_c=S+3\delta_\gamma/4$, so the adiabatic part cancels and

$$
\delta P_{\rm nad}
=-\frac{4AC}{3(4A+3C)}S.
$$

Since $\bar\rho+\bar P=C+4A/3$, the curvature evolves as

$$
\boxed{\frac{d\mathcal R}{d\ln a}
=\frac{4\bar\rho_\gamma\bar\rho_c}
{(4\bar\rho_\gamma+3\bar\rho_c)^2}S}.
$$

In the sign convention requested in the question, $d\mathcal R/d\ln a=-fS$, this means

$$
\boxed{f(\bar\rho_\gamma,\bar\rho_c)
=-\frac{4\bar\rho_\gamma\bar\rho_c}
{(4\bar\rho_\gamma+3\bar\rho_c)^2}}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
