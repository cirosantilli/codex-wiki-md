# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper62.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $H=\dot a/a$ be the [Hubble parameter](../../../cosmology.md#hubble-parameter), and normalize the [scale factor](../../../cosmology.md#scale-factor-cosmology) by $a(t_0)=1$. The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) gives $\rho_M=\rho_{M0}a^{-3}$ for [pressureless matter](../../../cosmology.md#pressureless-matter), whereas the [cosmological constant](../../../cosmology.md#cosmological-constant) has constant energy density $\rho_\Lambda$. The spatially flat [Friedmann equation](../../../cosmology.md#friedmann-equations) therefore becomes

$$
H^2=\frac{8\pi G}{3}(\rho_{M0}a^{-3}+\rho_\Lambda).
$$

The present [Hubble constant](../../../cosmology.md#hubble-constant) is $H_0=H(t_0)$. In terms of the present [critical density](../../../cosmology.md#critical-density) $\rho_{\mathrm{crit},0}=3H_0^2/(8\pi G)$, the matter [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) is $\Omega_M=\rho_{M0}/\rho_{\mathrm{crit},0}$. Spatial flatness gives $\rho_\Lambda/\rho_{\mathrm{crit},0}=1-\Omega_M$, so

$$
\boxed{\left(\frac{\dot a}{a}\right)^2=H_0^2\left[\frac{\Omega_M}{a^3}+1-\Omega_M\right].}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $0<\Omega_M<1$, set $x=a^{3/2}$ and choose the expanding branch of the [Friedmann equation](../../../cosmology.md#friedmann-equations). Then

$$
\dot x=\frac32H_0\sqrt{\Omega_M+(1-\Omega_M)x^2}.
$$

Separating variables and choosing [cosmic time](../../../cosmology.md#cosmic-time) $t=0$ at the [Big Bang](../../../cosmology.md#big-bang) gives

$$
\frac{\operatorname{arsinh}\!\left(x\sqrt{(1-\Omega_M)/\Omega_M}\right)}{\sqrt{1-\Omega_M}}=\frac32H_0t.
$$

Thus the [flat dust-and-vacuum expansion](../../../cosmology.md#flat-dust-and-vacuum-expansion) is

$$
\boxed{a(t)=\left(\frac{\Omega_M}{1-\Omega_M}\right)^{1/3}\sinh^{2/3}\!\left(\frac32H_0\sqrt{1-\Omega_M}\,t\right).}
$$

Setting $a(t_0)=1$ gives the [age of a flat matter-Lambda universe](../../../cosmology.md#age-of-a-flat-matter-lambda-universe),

$$
t_0=\frac{2}{3H_0\sqrt{1-\Omega_M}}\operatorname{arsinh}\sqrt{\frac{1-\Omega_M}{\Omega_M}}.
$$

The two [matter-vacuum age endpoint limits](../../../cosmology.md#matter-vacuum-age-endpoint-limits) follow below.

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

As $\Omega_M\downarrow0$, use $\operatorname{arsinh}z=\log(z+\sqrt{1+z^2})\sim\log(2z)$ to obtain

$$
\boxed{H_0t_0\sim\frac13\log\frac4{\Omega_M}\ \longrightarrow\ \infty.}
$$

At fixed [Hubble constant](../../../cosmology.md#hubble-constant), the [age of a flat matter-Lambda universe](../../../cosmology.md#age-of-a-flat-matter-lambda-universe) diverges logarithmically. The limiting purely vacuum-dominated [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) has an exponential [scale factor](../../../cosmology.md#scale-factor-cosmology) and no [Big Bang](../../../cosmology.md#big-bang) at a finite value of [cosmic time](../../../cosmology.md#cosmic-time) in this flat slicing.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

As $\Omega_M\uparrow1$, use $\operatorname{arsinh}z\sim z$ near zero. Consequently

$$
\boxed{t_0\longrightarrow\frac2{3H_0}.}
$$

The [flat dust-and-vacuum expansion](../../../cosmology.md#flat-dust-and-vacuum-expansion) tends to $a(t)=(3H_0t/2)^{2/3}$, the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A radial light ray in the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) travels [comoving radial distance](../../../cosmology.md#comoving-radial-distance) $d\chi=dt/a$ in units $c=1$. The [total comoving visibility radius](../../../cosmology.md#total-comoving-visibility-radius) is therefore the full available [conformal time](../../../cosmology.md#conformal-time) interval,

$$
d_c=\int_0^\infty\frac{dt}{a(t)}=\int_0^\infty\frac{da}{a^2H(a)}.
$$

Insert the [Friedmann equation](../../../cosmology.md#friedmann-equations) from part (a), then put $y=1/a$ to get

$$
\boxed{d_c=\frac1{H_0}\int_0^\infty\frac{dy}{\sqrt{1-\Omega_M+\Omega_My^3}}.}
$$

For $0<\Omega_M<1$ the integrand is bounded at zero and decays as $y^{-3/2}$ at infinity, so the [total conformal lifetime of a flat matter-Lambda universe](../../../cosmology.md#total-conformal-lifetime-of-a-flat-matter-lambda-universe) is finite. Equivalently, this distance is the present [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) plus the remaining comoving distance to the [cosmological event horizon](../../../general-relativity.md#cosmological-event-horizon). This describes causal visibility under the assumed ability to see back to the initial singularity.

The substitution $u=y[\Omega_M/(1-\Omega_M)]^{1/3}$ also evaluates the integral using the [beta function](../../../complex-analysis.md#beta-function):

$$
d_c=\frac{\Omega_M^{-1/3}(1-\Omega_M)^{-1/6}}{3H_0}\,\mathrm B\!\left(\frac13,\frac16\right).
$$

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [degeneracy factor](../../../statistical-physics.md#degeneracy-factor) $g_A$ counts internal states with the same energy, including the allowed [spin](../../../quantum-mechanics.md#spin) states. The [chemical potential](../../../thermodynamics.md#chemical-potential) $\mu_A$ measures the free-energy cost of changing the number of particles of species $A$; in this convention the rest energy remains in the exponential of the [nonrelativistic Maxwell--Boltzmann number density](../../../statistical-physics.md#nonrelativistic-maxwell-boltzmann-number-density).

The [chemical potential](../../../thermodynamics.md#chemical-potential) is fixed by the densities of [conserved charges](../../../quantum-field-theory.md#conserved-charge) and by [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) between reactions. For a reaction $\sum_A\nu_A A=0$, [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) requires $\sum_A\nu_A\mu_A=0$. Equivalently, when these are the only constraints, $\mu_A$ is a linear combination of the [chemical potentials](../../../thermodynamics.md#chemical-potential) of the [conserved charges](../../../quantum-field-theory.md#conserved-charge) carried by $A$. An unconstrained species has zero [chemical potential](../../../thermodynamics.md#chemical-potential). In particular, the [photon chemical potential](../../../thermodynamics.md#photon-chemical-potential) vanishes in thermal equilibrium when photon-number-changing reactions are effective.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $p+e\rightleftharpoons H+\gamma$, [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) and the vanishing [photon chemical potential](../../../thermodynamics.md#photon-chemical-potential) imply $\mu_H=\mu_p+\mu_e$. Taking the ratio of the three [nonrelativistic Maxwell--Boltzmann number densities](../../../statistical-physics.md#nonrelativistic-maxwell-boltzmann-number-density) cancels these [chemical potentials](../../../thermodynamics.md#chemical-potential):

$$
\frac{n_H}{n_pn_e}=\frac{g_H}{g_pg_e}\left(\frac{2\pi M_H}{M_pM_eT}\right)^{3/2}\exp\!\left(\frac{M_p+M_e-M_H}{T}\right).
$$

The ground-state [hydrogen atom](../../../physics.md#hydrogen-atom) has four combined [Electron](../../../physics.md#electron) and [proton](../../../physics.md#proton) [spin](../../../quantum-mechanics.md#spin) states if the small hyperfine splitting is ignored, whereas $g_p=g_e=2$. Hence $g_H/(g_pg_e)=1$. With [Hydrogen binding energy](../../../cosmology.md#hydrogen-binding-energy) $B=M_p+M_e-M_H$ and $M_H\simeq M_p$, the [Saha ionization equation](../../../cosmology.md#saha-ionization-equation) gives

$$
\boxed{\frac{n_H}{n_pn_e}\simeq\left(\frac{2\pi}{M_eT}\right)^{3/2}e^{B/T}.}
$$

The approximation in the prefactor neglects relative corrections of order $(M_e+B)/M_p$; the [Hydrogen binding energy](../../../cosmology.md#hydrogen-binding-energy) must be retained in the exponential.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $n_b=n_p+n_H$ for the [cosmological baryon density](../../../cosmology.md#cosmological-baryon-density) in this hydrogen-only model, and $x_e=n_p/n_b$ for the [hydrogen ionization fraction](../../../cosmology.md#hydrogen-ionization-fraction). By [charge neutrality](../../../electromagnetism.md#charge-neutrality), $n_e=n_p$, so the [Saha ionization equation](../../../cosmology.md#saha-ionization-equation) becomes

$$
\frac{1-x_e}{x_e^2}=n_b\left(\frac{2\pi}{M_eT}\right)^{3/2}e^{B/T}.
$$

The [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) is $\eta=n_b/n_\gamma$, and the equilibrium [photon number density](../../../statistical-physics.md#photon-number-density) is $n_\gamma=2\zeta(3)T^3/\pi^2$. At an order-one [hydrogen ionization fraction](../../../cosmology.md#hydrogen-ionization-fraction), neglecting factors of order one therefore gives

$$
1\simeq\eta\left(\frac T{M_e}\right)^{3/2}e^{B/T},\qquad T\simeq\frac{B}{\log[\eta^{-1}(M_e/T)^{3/2}]}.
$$

Replacing $T$ inside the slowly varying logarithm by $B$ gives

$$
\boxed{T\simeq\frac{B}{\log[\eta^{-1}(M_e/B)^{3/2}]}\ll B.}
$$

With $B=13.6\,\mathrm{eV}$, $M_e=5\times10^5\,\mathrm{eV}$ and $\eta=10^{-10}$, this is $T\simeq0.351\,\mathrm{eV}\simeq4.1\times10^3\,\mathrm K$. Solving the preceding implicit approximation instead gives $T\simeq0.306\,\mathrm{eV}\simeq3.5\times10^3\,\mathrm K$. Both are reasonable estimates of the [recombination temperature](../../../cosmology.md#recombination-temperature) at the accuracy requested. The [small baryon abundance delays hydrogen recombination](../../../cosmology.md#small-baryon-abundance-delays-hydrogen-recombination): even when $T\ll B$, the high-energy tail of the abundant [photons](../../../quantum-mechanics.md#photon) can still ionize the much rarer [hydrogen atoms](../../../physics.md#hydrogen-atom).

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

With an approximately constant [Hubble parameter](../../../cosmology.md#hubble-parameter) $H$, the [scale factor](../../../cosmology.md#scale-factor-cosmology) is $a(t)=e^{Ht}$ after a choice of normalization. Integrate $d\tau=dt/a(t)$ and choose the integration constant so that the future endpoint is $\tau=0$:

$$
\tau=-\frac{e^{-Ht}}H,\qquad\boxed{a(\tau)=-\frac1{H\tau},\quad-\infty<\tau<0.}
$$

Substituting $dt=a\,d\tau$ in the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) gives $ds^2=a^2(\tau)(-d\tau^2+d\mathbf x^2)$. This is [Conformal time during de Sitter expansion](../../../cosmology.md#conformal-time-during-de-sitter-expansion).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) in [conformal time](../../../cosmology.md#conformal-time), $\sqrt{-g}=a^4$, $g^{00}=-a^{-2}$ and $g^{ij}=a^{-2}\delta^{ij}$. The equation for a [minimally coupled massless scalar field](../../../scalar-field-theory.md#minimally-coupled-massless-scalar-field) is consequently

$$
-(a^2\delta\phi')'+a^2\nabla^2\delta\phi=0.
$$

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode) of comoving wavevector $\mathbf k$, the [Laplacian](../../../calculus.md#laplacian) contributes $-k^2$, where $k=|\mathbf k|$. Thus

$$
\delta\phi_k''+2\frac{a'}a\delta\phi_k'+k^2\delta\phi_k=0.
$$

Since $a'/a=-1/\tau$, this yields

$$
\boxed{\delta\phi_k''-\frac2\tau\delta\phi_k'=-k^2\delta\phi_k.}
$$

The absence of a curvature-coupling term is material: a [conformally coupled scalar field](../../../quantum-field-theory.md#conformally-coupled-scalar-field) obeys a different mode equation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Denote the comoving box volume by $\mathcal V$, keeping it distinct from the [inflaton](../../../cosmic-inflation.md#inflaton) potential $V(\phi)$. For the [Canonically rescaled de Sitter scalar mode](../../../cosmic-inflation.md#canonically-rescaled-de-sitter-scalar-mode) $u_k=a\delta\phi_k$, the equation in part (b) becomes

$$
u_k''+\left(k^2-\frac2{\tau^2}\right)u_k=0.
$$

Direct differentiation verifies the positive-frequency solution

$$
u_k=\frac{1-i/(k\tau)}{\sqrt{2k\mathcal V}}e^{-ik\tau},\qquad\boxed{\delta\phi_k^{(+)}=\frac{H(-\tau+i/k)}{\sqrt{2k\mathcal V}}e^{-ik\tau}.}
$$

For $|k\tau|\gg1$, $u_k$ tends to $e^{-ik\tau}/\sqrt{2k\mathcal V}$, the positive-frequency flat-space mode. It therefore selects the incoming [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum). The [Bunch-Davies mode normalization in a finite comoving volume](../../../cosmic-inflation.md#bunch-davies-mode-normalization-in-a-finite-comoving-volume) is fixed by the [Wronskian](../../../differential-equation.md#wronskian) condition

$$
a^2\mathcal V\left(\delta\phi_k^{(+)}\delta\phi_k^{(+)*\prime}-\delta\phi_k^{(+)*}\delta\phi_k^{(+)\prime}\right)=i.
$$

After [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $|k\tau|\ll1$, the mode tends to the time-independent value $iH/\sqrt{2k^3\mathcal V}$. The complex mode and its [Hermitian conjugate](../../../hilbert-space.md#hermitian-conjugation) together make the real quantum field.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

In the incoming [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum), only $\langle a_{\mathbf k}a_{\mathbf q}^{\dagger}\rangle=\delta_{\mathbf k\mathbf q}$ contributes to the coincident [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value). Thus

$$
\langle\delta\hat\phi^2\rangle=\sum_{\mathbf k}|\delta\phi_k^{(+)}|^2=\sum_{\mathbf k}\frac1{2k\mathcal V}\left(\frac1{a^2}+\frac{H^2}{k^2}\right).
$$

Replacing the box sum by $\mathcal V\int d^3k/(2\pi)^3$ gives

$$
\boxed{\langle\delta\hat\phi^2\rangle=\int\frac{d^3k}{(2\pi)^3}\frac1{2k}\left(\frac1{a^2}+\frac{H^2}{k^2}\right)=\frac1{4\pi^2}\int_0^\infty dk\left(\frac{k}{a^2}+\frac{H^2}{k}\right).}
$$

The [subhorizon vacuum contribution](../../../cosmic-inflation.md#subhorizon-vacuum-contribution-to-a-de-sitter-scalar-spectrum) is the flat-space zero-point term; at fixed comoving $k$ it redshifts as $a^{-2}$. The other term gives [frozen scalar power](../../../cosmic-inflation.md#frozen-contribution-to-a-de-sitter-scalar-spectrum) on [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale). Specifically, the [dimensionless cosmological power spectrum](../../../cosmic-inflation.md#dimensionless-cosmological-power-spectrum) per logarithmic interval is

$$
\Delta_{\delta\phi}^2(k,\tau)=\frac{k^2/a^2+H^2}{4\pi^2}\ \longrightarrow\ \boxed{\left(\frac H{2\pi}\right)^2}.
$$

Its late-time value is independent of $k$, producing a [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum). Each fixed [Fourier mode](../../../fourier-analysis.md#fourier-mode) freezes separately as $\tau\to0$.

<a id="3/d/image-vacuum-redshifting-and-frozen-power-of-massless-scalar-modes-during-de-sitter-expansion"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62-scalar-freezing.png)

**[Figure 1](#3/d/image-vacuum-redshifting-and-frozen-power-of-massless-scalar-modes-during-de-sitter-expansion). Vacuum redshifting and frozen power of massless scalar modes during de Sitter expansion**.

The coincident integral is formal: the vacuum part diverges at large $k$, and an unlimited scale-invariant part diverges at small $k$. The conclusion concerns the power in each finite logarithmic band. A finite inflationary history supplies a largest generated wavelength, as described by the [infrared qualification of a scale-invariant covariance](../../../cosmic-inflation.md#infrared-qualification-of-a-scale-invariant-covariance); taking the late-time limit inside an unregulated integral would not be justified.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A perturbation of the [inflaton](../../../cosmic-inflation.md#inflaton) shifts its local clock: $\delta\phi\simeq\dot\phi\,\delta t$. Regions with different clock shifts reach the end of inflation at different times and hence undergo different amounts of expansion. The [inflaton clock-shift origin of curvature perturbations](../../../cosmic-inflation.md#inflaton-clock-shift-origin-of-curvature-perturbations) gives a local expansion difference of magnitude $H\delta t=H\delta\phi/\dot\phi$. The sign depends on whether $\delta t$ denotes a clock advance or a delay to a fixed end value.

The [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) has amplitude $\mathcal R\simeq H\delta\phi/\dot\phi$. For adiabatic evolution, [superhorizon conservation of single-field comoving curvature](../../../cosmic-inflation.md#superhorizon-conservation-of-single-field-comoving-curvature) carries this amplitude into the later growing [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast), with the numerical conversion depending on the epoch and the density slice. Thus the approximate density-amplitude statement in the question follows; it does not identify the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) and $\mathcal R$ in every gauge.

The [frozen scalar power](../../../cosmic-inflation.md#frozen-contribution-to-a-de-sitter-scalar-spectrum) per $d\log k$ is $(H/2\pi)^2$, so the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum) is

$$
\boxed{\Delta_{\mathcal R}^2(k)=\left(\frac{H^2}{2\pi\dot\phi}\right)^2_{k\text{ at horizon exit}}.}
$$

Consequently $\langle\mathcal R^2\rangle=\int (dk/k)\Delta_{\mathcal R}^2(k)$, giving the requested approximate growing-density spectrum. Both $H$ and $\dot\phi$ are evaluated separately when each [Fourier mode](../../../fourier-analysis.md#fourier-mode) undergoes [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

At [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $k$ is proportional to $aH$; the convention-dependent factor $2\pi$ has zero logarithmic derivative. Define the [first Hubble slow-roll parameter](../../../cosmic-inflation.md#first-hubble-slow-roll-parameter) $\epsilon_H=-\dot H/H^2$. Then

$$
\frac{d\log k}{d\log a}=1-\epsilon_H,\qquad\frac d{d\log k}=\frac1{1-\epsilon_H}\frac d{d\log a}\simeq\frac d{d\log a}.
$$

The [chain rule](../../../calculus.md#chain-rule) gives $d/d\log a=(\dot\phi/H)d/d\phi$. In [reduced Planck units](../../../physics.md#reduced-planck-units), the [slow-roll equations](../../../cosmic-inflation.md#slow-roll-approximation) are $3H\dot\phi\simeq-V_{,\phi}$ and $3H^2\simeq V$. Therefore the [horizon-exit logarithmic derivative in slow roll](../../../cosmic-inflation.md#horizon-exit-logarithmic-derivative-in-slow-roll) is

$$
\boxed{k\frac d{dk}\simeq a\frac d{da}=\frac{\dot\phi}H\frac d{d\phi}\simeq-\frac{V_{,\phi}}V\frac d{d\phi}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [slow-roll equations](../../../cosmic-inflation.md#slow-roll-approximation) turn the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum) into

$$
\Delta_{\mathcal R}^2\simeq\frac{V^3}{12\pi^2V_{,\phi}^2}=\frac{V}{24\pi^2\epsilon},\qquad\epsilon=\frac12\left(\frac{V_{,\phi}}V\right)^2.
$$

The [spectral tilt](../../../cosmic-inflation.md#scalar-spectral-index) is the logarithmic derivative of this dimensionless spectrum. Apply the [horizon-exit logarithmic derivative in slow roll](../../../cosmic-inflation.md#horizon-exit-logarithmic-derivative-in-slow-roll):

$$
\Delta n=\frac{d\log\Delta_{\mathcal R}^2}{d\log k}\simeq-\frac{V_{,\phi}}V\left(3\frac{V_{,\phi}}V-2\frac{V_{,\phi\phi}}{V_{,\phi}}\right)=-3\left(\frac{V_{,\phi}}V\right)^2+2\frac{V_{,\phi\phi}}V.
$$

With the [potential slow-roll parameter](../../../cosmic-inflation.md#potential-slow-roll-parameter) $\epsilon$ above and the [second potential slow-roll parameter](../../../cosmic-inflation.md#second-potential-slow-roll-parameter) $\eta=V_{,\phi\phi}/V$,

$$
\boxed{\Delta n=-6\epsilon+2\eta.}
$$

This is the first-order departure of the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) from unity, in [reduced Planck units](../../../physics.md#reduced-planck-units).

## 5

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), the [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) gives $\rho_R\propto a^{-4}$. The flat [Friedmann equation](../../../cosmology.md#friedmann-equations) in [conformal time](../../../cosmology.md#conformal-time) is $(a'/a)^2=8\pi Ga^2\rho_R/3$. Hence $a'^2$ is constant, and choosing the [Big Bang](../../../cosmology.md#big-bang) at $\tau=0$ yields

$$
\boxed{a\propto\tau,\qquad8\pi G\rho_Ra^2=\frac3{\tau^2}.}
$$

For the [CDM density equation in a matter-radiation universe](../../../linear-cosmological-density-perturbation.md#cdm-density-equation-in-a-matter-radiation-universe), neglect $\rho_C\delta_C$ while retaining $\delta_C$ itself. The [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) give $\delta_R=4\delta_C/3$, so

$$
\delta_C''+\frac1\tau\delta_C'=\frac4{\tau^2}\delta_C.
$$

This [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation) has powers $\tau^p$ with $p(p-1)+p-4=0$, namely $p=2,-2$. Selecting the growing [superhorizon adiabatic CDM mode in radiation domination](../../../linear-cosmological-density-perturbation.md#superhorizon-adiabatic-cdm-mode-in-radiation-domination) gives

$$
\boxed{\delta_C(\tau,k)=A_R(k)\tau^2.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

After [cosmological horizon entry](../../../linear-cosmological-density-perturbation.md#cosmological-horizon-entry) in [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), the oscillating radiation source averages away. Neglecting both that source and CDM self-gravity in the [CDM density equation in a matter-radiation universe](../../../linear-cosmological-density-perturbation.md#cdm-density-equation-in-a-matter-radiation-universe) gives

$$
\delta_C''+\frac1\tau\delta_C'=0,\qquad(\tau\delta_C')'=0,
$$

so $\delta_C=C_1(k)+C_2(k)\log\tau$. The [superhorizon adiabatic CDM mode in radiation domination](../../../linear-cosmological-density-perturbation.md#superhorizon-adiabatic-cdm-mode-in-radiation-domination) has amplitude $A_R(k)\tau_h^2\sim A_R(k)k^{-2}$ at entry $\tau_h\sim k^{-1}$, fixing this scale for the subsequent [logarithmic CDM growth after radiation-era horizon entry](../../../linear-cosmological-density-perturbation.md#logarithmic-cdm-growth-after-radiation-era-horizon-entry).

More explicitly, in a sharp-transition approximation with $\tau_h=1/k$, continuity of $\delta_C$ and $\delta_C'$ gives

$$
\delta_C=\frac{A_R(k)}{k^2}\,[1+2\log(k\tau)].
$$

The [matching the CDM growing mode at horizon entry](../../../linear-cosmological-density-perturbation.md#matching-the-cdm-growing-mode-at-horizon-entry) therefore yields the late subhorizon scaling

$$
\boxed{\delta_C(\tau,k)\simeq A_R(k)k^{-2}\log(k\tau).}
$$

Here $\simeq$ suppresses order-one coefficients and the nonlogarithmic term, as in the question. A smooth treatment of the radiation forcing through entry changes those coefficients; the factor two is exact only for the sharp matching model just used. This logarithmic growth, rather than growth proportional to $a$, is the [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $\rho_C\propto a^{-3}$. The flat [Friedmann equation](../../../cosmology.md#friedmann-equations) in [conformal time](../../../cosmology.md#conformal-time) implies $a'^2\propto a$, and hence

$$
\boxed{a\propto\tau^2,\qquad8\pi G\rho_Ca^2=\frac{12}{\tau^2}.}
$$

With radiation neglected, the [CDM density equation in a matter-radiation universe](../../../linear-cosmological-density-perturbation.md#cdm-density-equation-in-a-matter-radiation-universe) reduces to

$$
\delta_C''+\frac2\tau\delta_C'-\frac6{\tau^2}\delta_C=0.
$$

For this [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation), $\delta_C\propto\tau^p$ requires $p(p-1)+2p-6=(p-2)(p+3)=0$. Thus the [matter-era growing and decaying density modes](../../../linear-cosmological-density-perturbation.md#matter-era-growing-and-decaying-density-modes) are $\tau^2$ and $\tau^{-3}$, respectively, and

$$
\boxed{\delta_C(\tau,k)\propto\tau^2\propto a.}
$$

There is no explicit $k$ in this pressureless equation, so the result holds on all scales within the stated CDM-comoving [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) description. The amplitude can still depend on $k$ through its earlier evolution; the result does not equate [density contrasts](../../../linear-cosmological-density-perturbation.md#density-contrast) on different time slicings.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
