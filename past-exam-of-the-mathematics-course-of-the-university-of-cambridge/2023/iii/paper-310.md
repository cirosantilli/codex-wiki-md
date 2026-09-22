# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_310.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

For a component with the [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state) $P=w\rho$, the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) is

$$
\dot\rho+3H(1+w)\rho=0.
$$

Using $H=\dot a/a$ makes this a [separable differential equation](../../../differential-equation.md#separable-differential-equation):

$$
\frac{d\rho}{\rho}=-3(1+w)\frac{da}{a}.
$$

Taking $a_0=1$ gives the [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling)

$$
\boxed{\rho(a)=\rho_0a^{-3(1+w)}
=\rho_0(1+z)^{3(1+w)}}.
$$

The spatially flat [Friedmann equation](../../../cosmology.md#friedmann-equations) and the [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) therefore give

$$
\boxed{H(z)=H_0E(z)},
\qquad
E(z)=\left[\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}\right]^{1/2}.
$$

Along a radial light ray, $d\chi=dt/a$. Since the [redshift-time relation](../../../cosmology.md#redshift-time-relation) is $dt=-dz/[(1+z)H]$ and $a=(1+z)^{-1}$,

$$
d\chi=-\frac{dz}{H(z)}.
$$

Hence the [comoving radial distance](../../../cosmology.md#comoving-radial-distance) is

$$
\boxed{\chi(z)=\frac1{H_0}\int_0^z
\frac{dz'}{\left[\sum_i\Omega_{i,0}(1+z')^{3(1+w_i)}\right]^{1/2}}}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In the flat [Lambda-CDM model](../../../cosmology.md#lambda-cdm-model),

$$
d_A(z)=\frac1{1+z}\frac1{H_0}
\int_0^z\frac{dz'}{\sqrt{\Omega_{m,0}(1+z')^3+1-\Omega_{m,0}}}.
$$

At low redshift, $H(z)=H_0+O(z)$, so the [angular diameter distance](../../../cosmology.md#angular-diameter-distance) satisfies $d_A(z)=z/H_0+O(z^2)$ and initially increases from zero. At high redshift, [pressureless matter](../../../cosmology.md#pressureless-matter) dominates and the integral converges:

$$
\chi(z)\longrightarrow\chi_\infty<\infty,
\qquad
d_A(z)\sim\frac{\chi_\infty}{1+z}\longrightarrow0.
$$

Thus the positive continuous function $d_A$ rises from zero and returns toward zero, so it attains an interior maximum. This is the [angular diameter distance turnover](../../../cosmology.md#angular-diameter-distance-turnover); beyond it, a fixed physical size appears larger at higher redshift.

If the [variable dark-energy equation of state](../../../cosmology.md#variable-dark-energy-equation-of-state) differs slightly from $-1$, matter still controls the large-$z$ expansion, while the same low-$z$ limit holds. The turnover therefore persists under such a small change. More generally, it persists whenever the high-redshift comoving distance grows more slowly than $1+z$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For the transverse [baryon acoustic oscillation](../../../cosmology.md#baryon-acoustic-oscillation) ruler, $d_A=a\chi$ and the physical ruler length is $a\chi_d$. Its observed angle is therefore

$$
\theta(z)=\frac{a\chi_d}{d_A(z)}
=\frac{\chi_d}{\chi(z)}
=\frac{H_0\chi_d}{I(z;\Omega_{m,0})},
$$

where

$$
I(z;\Omega_{m,0})=
\int_0^z\frac{dz'}{\sqrt{\Omega_{m,0}(1+z')^3+1-\Omega_{m,0}}}.
$$

The unknown [cosmological standard ruler](../../../cosmology.md#cosmological-standard-ruler) length and $H_0$ occur only through the common amplitude $H_0\chi_d$. Measurements at two distinct redshifts give

$$
\frac{\theta(z_1)}{\theta(z_2)}
=\frac{I(z_2;\Omega_{m,0})}{I(z_1;\Omega_{m,0})},
$$

which generically determines the one shape parameter $\Omega_{m,0}$. Thus two redshifts suffice; additional redshifts overdetermine the model and improve precision.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

To first order, the radial and transverse comoving separations are

$$
\Delta\chi_\parallel=\frac{\Delta z}{H(z)}
=\frac{f(z,\Omega_{m,0})}{H_0}\Delta z,
\qquad
\Delta\chi_\perp=\chi(z)\Delta\theta
=\frac{I(z;\Omega_{m,0})}{H_0}\Delta\theta,
$$

where

$$
f(z,\Omega_{m,0})=
\frac1{\sqrt{\Omega_{m,0}(1+z)^3+1-\Omega_{m,0}}}.
$$

The local spatial geometry is that of [Euclidean space](../../../functional-analysis.md#euclidean-norm), so the [Pythagorean theorem](../../../geometry-and-topology.md#pythagorean-theorem) gives

$$
\Delta\chi
=\frac{f}{H_0}
\sqrt{(\Delta z)^2+\left(\frac I f\right)^2(\Delta\theta)^2}.
$$

Consequently the requested function is

$$
\boxed{y(z,\Omega_{m,0})=
\frac{I(z;\Omega_{m,0})}{f(z,\Omega_{m,0})}
=H(z)\chi(z)}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

**Yes.** A [radial baryon acoustic oscillation measurement](../../../cosmology.md#radial-baryon-acoustic-oscillation-measurement) and a [transverse baryon acoustic oscillation measurement](../../../cosmology.md#transverse-baryon-acoustic-oscillation-measurement) of the same ruler at one redshift obey

$$
\Delta z=H(z)\chi_d,
\qquad
\Delta\theta=\frac{\chi_d}{\chi(z)}.
$$

Their ratio cancels both the unknown ruler length and the overall Hubble scale:

$$
\boxed{\frac{\Delta z}{\Delta\theta}
=H(z)\chi(z)=y(z,\Omega_{m,0})}.
$$

This is the [Alcock-Paczyński parameter](../../../cosmology.md#alcock-paczynski-parameter). At a specified redshift its dependence on $\Omega_{m,0}$ permits a one-redshift determination within the assumed flat [Lambda-CDM model](../../../cosmology.md#lambda-cdm-model).

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Before [electron-positron annihilation in cosmology](../../../cosmology.md#electron-positron-annihilation-in-cosmology), photons and electron-positron pairs share a temperature. Their effective entropy degrees of freedom are

$$
g_{*s}^{\rm before}=2+\frac78(2+2)=\frac{11}{2}.
$$

After annihilation the electromagnetic plasma contains only the two photon polarizations, so $g_{*s}^{\rm after}=2$. The already decoupled neutrinos receive none of this entropy and simply cool as $T_\nu\propto a^{-1}$. Applying [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) separately to the coupled electromagnetic plasma gives

$$
g_{*s}^{\rm before}T_{\rm before}^3a_{
m before}^3
=g_{*s}^{\rm after}T^3a^3,
$$

whereas $T_\nu^3a^3=T_{\rm before}^3a_{
m before}^3$. Division yields the [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) temperature

$$
\boxed{\frac{T_\nu}{T}=\left(\frac4{11}\right)^{1/3}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The energy density from a [phase-space distribution function](../../../statistical-physics.md#phase-space-distribution-function) with $g=2$ internal states is

$$
\rho_\nu=\frac{g}{(2\pi)^3}
\int_{\mathbb R^3}\frac{\sqrt{p^2+m_\nu^2}}{e^{p/T_\nu}+1}\,d^3p
=\frac{g}{2\pi^2}\int_0^\infty
\frac{p^2\sqrt{p^2+m_\nu^2}}{e^{p/T_\nu}+1}\,dp.
$$

In the ultrarelativistic limit $T_\nu\gg m_\nu$, set $x=p/T_\nu$. The [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) then gives

$$
\rho_\nu=\frac{T_\nu^4}{\pi^2}
\int_0^\infty\frac{x^3}{e^x+1}\,dx
=\frac{T_\nu^4}{\pi^2}
3!\left(1-2^{-3}\right)\zeta(4).
$$

Since $\zeta(4)=\pi^4/90$,

$$
\boxed{\rho_\nu=\frac{7\pi^2}{120}T_\nu^4}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

When $\mu_\nu/T_\nu\gg1$, the [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) approaches the [step function](../../../measure-theory.md#step-function) $f(p)=1$ for $p<\mu_\nu$ and zero for $p>\mu_\nu$. For one internal state and negligible mass, the [degenerate relic neutrino](../../../cosmology.md#degenerate-relic-neutrino) energy density is therefore

$$
\rho_\nu\simeq\frac1{2\pi^2}\int_0^{\mu_\nu}p^3\,dp
=\boxed{\frac{\mu_\nu^4}{8\pi^2}},
$$

so $\boxed{A=1/(8\pi^2)}$.

At [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium), the [antineutrino](../../../standard-model.md#antineutrino) chemical potential is $-\mu_\nu$. Its occupation is approximately $e^{-(p+\mu_\nu)/T_\nu}$, giving

$$
\rho_{\bar\nu}\simeq
\frac{3T_\nu^4}{\pi^2}e^{-\mu_\nu/T_\nu}.
$$

It is exponentially smaller than the neutrino density; this particle-antiparticle imbalance is a [cosmological lepton asymmetry](../../../cosmology.md#cosmological-lepton-asymmetry).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write the [neutrino degeneracy parameter](../../../cosmology.md#neutrino-degeneracy-parameter) as $\xi_\nu=\mu_\nu/T_\nu$. Requiring one degenerate species not to exceed today's [critical density](../../../cosmology.md#critical-density) gives

$$
\frac{\xi_\nu^4T_\nu^4}{8\pi^2}
\leq6\times10^4T^4.
$$

Using $T/T_\nu=(11/4)^{1/3}$,

$$
\boxed{\xi_\nu\leq
\left(48\pi^2\times10^4\right)^{1/4}
\left(\frac{11}{4}\right)^{1/3}
\simeq65}.
$$

Several equally degenerate species would strengthen the bound by the fourth root of their number.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

A large [neutrino degeneracy parameter](../../../cosmology.md#neutrino-degeneracy-parameter) raises the relativistic energy density and therefore the expansion rate. [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) tests this through primordial light-element abundances; an electron-neutrino chemical potential also shifts neutron--proton chemical equilibrium directly. The [Cosmic microwave background power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum) tests the changed expansion rate, matter-radiation equality, sound horizon, damping scale, and neutrino anisotropic stress. Finally, [large-scale structure of the universe](../../../large-scale-structure-of-the-universe.md) and the matter power spectrum test the altered equality scale and [neutrino free streaming](../../../linear-cosmological-density-perturbation.md#neutrino-free-streaming). These observables distinguish a degenerate-neutrino cosmology from the standard thermal relic scenario in complementary epochs.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology), $\bar P_r=\bar\rho_r/3$ and $\delta P_r=\delta\rho_r/3$, so both terms proportional to the equation-of-state difference vanish. During matter domination the gravitational potential is constant, $\Phi'=0$. Writing $\theta_r=\nabla\mathbin\cdot\mathbf v_r$, the continuity and Euler equations reduce to

$$
\delta_r'=-\frac43\theta_r,
\qquad
\theta_r'=-\frac14\nabla^2\delta_r-\nabla^2\Phi.
$$

Differentiate the first equation and substitute the second:

$$
\delta_r''=\frac13\nabla^2\delta_r+\frac43\nabla^2\Phi.
$$

Thus the radiation perturbation obeys the forced acoustic equation

$$
\boxed{\delta_r''-\frac13\nabla^2\delta_r
=\frac43\nabla^2\Phi}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

After a spatial [Fourier transform](../../../analysis.md#fourier-transform), the preceding equation is

$$
\delta_r''+\frac{k^2}{3}\delta_r=-\frac43k^2\Phi.
$$

The constant particular solution is $\delta_r=-4\Phi$. Hence the [Sachs-Wolfe combination](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination)

$$
S=\frac14\delta_r+\Phi
$$

contains only the homogeneous [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) modes and satisfies

$$
S''+\frac{k^2}{3}S=0.
$$

For [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) on large scales, $S=\Phi/3=\mathcal R/5$ and $S'=0$ at the start of matter domination. Up to an irrelevant choice of the phase origin,

$$
\boxed{S(k,\tau)=\frac15\mathcal R(k,0)
\cos\left(\frac{k\tau}{\sqrt3}\right)},
\qquad
\boxed{T_S(k,\tau)=\frac15
\cos\left(\frac{k\tau}{\sqrt3}\right)}.
$$

Thus the [radiation acoustic transfer function](../../../linear-cosmological-perturbation-theory.md#radiation-acoustic-transfer-function) is flat at $1/5$ as $k\to0$ and oscillates on smaller scales. Projection onto the sky produces a large-angle Sachs-Wolfe plateau and, after the full photon-baryon physics is included, the acoustic structure of the [Cosmic microwave background power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum).

The [baryon transfer function](../../../linear-cosmological-perturbation-theory.md#baryon-transfer-function) should also oscillate soon after [cosmological recombination](../../../cosmology.md#recombination-cosmology): before decoupling, Thomson scattering forced baryons to share the acoustic motion of the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid), and recombination does not instantly erase the resulting density pattern.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $k_{\rm eq}$ be the horizon scale at [matter-radiation equality](../../../cosmology.md#matter-radiation-equality). At a fixed time soon after recombination, the [cold-dark-matter transfer function](../../../linear-cosmological-perturbation-theory.md#cold-dark-matter-transfer-function) defined as $T_c=\Delta_c/\mathcal R$ has the schematic behavior

$$
T_c(k)\propto
\begin{cases}
k^2,&k\ll k_{\rm eq},\\
\log(k/k_{\rm eq}),&k\gg k_{\rm eq},
\end{cases}
$$

with a smooth turnover near $k_{\rm eq}$. Large-scale modes enter the horizon during matter domination and the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) converts an almost scale-independent primordial potential into a density contrast proportional to $k^2$. Small-scale modes enter during radiation domination; radiation controls the potential and pressure prevents it from clustering, so cold-dark-matter growth is only logarithmic until equality. Subsequent matter-era growth multiplies all these modes by the same [linear growth factor](../../../linear-cosmological-density-perturbation.md#linear-growth-factor).

Equivalently, if the conventional matter transfer function is normalized to one as $k\to0$, it is constant for $k\ll k_{\rm eq}$ and falls approximately as $\log(k/k_{\rm eq})/k^2$ for $k\gg k_{\rm eq}$. Multiplication by the Poisson factor $k^2$ gives the behavior of the definition used here.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Subtracting the baryon equation from the cold-dark-matter equation cancels their common gravitational source and gives the [baryon--cold-dark-matter relative density mode](../../../linear-cosmological-perturbation-theory.md#baryon-cold-dark-matter-relative-density-mode)

$$
\boxed{\ddot D+2H\dot D=0},
\qquad D=\delta_c-\delta_b.
$$

Because the background fractions $\bar\rho_c/\bar\rho_m$ and $\bar\rho_b/\bar\rho_m$ are constant after recombination, their weighted sum gives

$$
\boxed{\ddot\delta_m+2H\dot\delta_m
-4\pi G\bar\rho_m\delta_m=0}.
$$

During matter domination, $a\propto t^{2/3}$. The first equation gives $a^2\dot D=\text{constant}$ and hence

$$
\boxed{D=D_0+D_1a^{-1/2}}.
$$

The [cosmic-time matter density modes](../../../linear-cosmological-density-perturbation.md#cosmic-time-matter-density-modes) give

$$
\boxed{\delta_m=Aa+Ba^{-3/2}}.
$$

Solving the definitions for the individual contrasts,

$$
\delta_c=\delta_m+\frac{\bar\rho_b}{\bar\rho_m}D,
\qquad
\delta_b=\delta_m-\frac{\bar\rho_c}{\bar\rho_m}D,
$$

so

$$
\frac{\delta_c}{\delta_b}
=\frac{\bar\rho_m\delta_m+\bar\rho_bD}
{\bar\rho_m\delta_m-\bar\rho_cD}
\longrightarrow\boxed{1}.
$$

Thus $\boxed{f=1}$. Both species feel the same gravitational potential after baryon pressure becomes negligible; the growing total mode overtakes the constant relative mode, so baryons catch up with cold dark matter.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

**Yes.** The baryons carry the oscillatory [baryon transfer function](../../../linear-cosmological-perturbation-theory.md#baryon-transfer-function) inherited from the pre-recombination [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid). Their later infall toward cold-dark-matter overdensities suppresses the relative mode and drives $\delta_b/\delta_c\to1$, but gravitational evolution does not remove every scale-dependent acoustic phase. The total [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) therefore contains the small wiggles known as a [baryon acoustic oscillation in the matter power spectrum](../../../cosmology.md#baryon-acoustic-oscillation-in-the-matter-power-spectrum).

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The right-hand side of the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum) is evaluated at [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $k=aH$. Using

$$
\dot\phi^2=2\epsilon M_{\rm Pl}^2H^2
$$

rewrites it as

$$
\Delta_{\mathcal R}^2
=\frac{H^2}{8\pi^2M_{\rm Pl}^2\epsilon}.
$$

At horizon exit, $d\log k=d\log(aH)=(1-\epsilon)dN$, so $d/d\log k=d/dN$ to first slow-roll order. With the [first Hubble slow-roll parameter](../../../cosmic-inflation.md#first-hubble-slow-roll-parameter) and [second Hubble slow-roll parameter](../../../cosmic-inflation.md#second-hubble-slow-roll-parameter),

$$
n_s-1=\frac{d\log\Delta_{\mathcal R}^2}{d\log k}
=-2\epsilon-\eta.
$$

The supplied relations $\epsilon=\epsilon_V$ and $\eta_V=2\epsilon-\eta/2$ imply $\eta=4\epsilon_V-2\eta_V$. Therefore

$$
\boxed{n_s-1=-6\epsilon_V+2\eta_V}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a monotonic inflaton trajectory, the [potential slow-roll parameter](../../../cosmic-inflation.md#potential-slow-roll-parameter) satisfies

$$
\left|\frac{d\phi}{dN}\right|
=M_{\rm Pl}\sqrt{2\epsilon_V(\phi)}.
$$

The remaining [slow-roll e-fold count](../../../cosmic-inflation.md#slow-roll-e-fold-count) is the integral from the present field value to its end value along the direction of motion:

$$
\boxed{\widetilde N(\phi)
=\int_\phi^{\phi_e}
\frac{d\widetilde\phi}
{M_{\rm Pl}\sqrt{2\epsilon_V(\widetilde\phi)}}}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Taking the ratio of the supplied [primordial tensor power spectrum](../../../cosmic-inflation.md#primordial-tensor-power-spectrum) and scalar spectrum cancels the common factor $(H/2\pi)^2$:

$$
r=\frac{8}{M_{\rm Pl}^2}
\frac{\dot\phi^2}{H^2}
=16\epsilon.
$$

To first slow-roll order $\epsilon=\epsilon_V$, so the [tensor-to-scalar ratio](../../../cosmic-inflation.md#tensor-to-scalar-ratio) is

$$
\boxed{r=16\epsilon_V},
\qquad
\boxed{C=16}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For the quadratic [hilltop inflation](../../../cosmic-inflation.md#hilltop-inflation) potential while $V_0$ dominates,

$$
\eta_V\simeq-\frac{m^2M_{\rm Pl}^2}{V_0},
\qquad
\epsilon_V\simeq
\frac{M_{\rm Pl}^2m^4\phi^2}{2V_0^2}
=\frac12\eta_V^2\frac{\phi^2}{M_{\rm Pl}^2}.
$$

Since $\epsilon_V$ is of higher order near the hilltop, the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) obeys $n_s-1\simeq2\eta_V$. The e-fold integral becomes

$$
\widetilde N(\phi)
=\frac1{|\eta_V|}\log\frac{\phi_e}{\phi}
=\frac2{1-n_s}\log\frac{\phi_e}{\phi},
$$

and hence

$$
\phi=\phi_e
e^{(n_s-1)\widetilde N/2}.
$$

Substitution into $r=C\epsilon_V$ yields the [quadratic hilltop slow-roll prediction](../../../cosmic-inflation.md#quadratic-hilltop-slow-roll-prediction)

$$
\boxed{r\simeq\frac18C(n_s-1)^2
\left(\frac{\phi_e}{M_{\rm Pl}}\right)^2
e^{(n_s-1)\widetilde N}},
$$

so $\boxed{f=1/8}$.

For $n_s-1=-0.04$ the expression decreases as $\widetilde N$ increases. Its largest allowed value therefore uses $\widetilde N=40$ and $\phi_e/M_{\rm Pl}<1$:

$$
r<\frac18(16)(0.04)^2e^{-0.04(40)}
=0.0032e^{-1.6}
\simeq\boxed{6.5\times10^{-4}}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
