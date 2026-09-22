# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper62.pdf)

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
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
    - [a](#3/v/a)
      - [Solution](#3/v/a/solution)
    - [b](#3/v/b)
      - [Solution](#3/v/b/solution)
    - [c](#3/v/c)
      - [Solution](#3/v/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use units with $c=1$. For the flat [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), the [Friedmann equation](../../../cosmology.md#friedmann-equations) is $H^2=8\pi G\rho/3+\Lambda/3$, where $H=\dot a/a$ is the [Hubble parameter](../../../cosmology.md#hubble-parameter). The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) for a separately conserved component with constant [equation of state](../../../thermodynamics.md#equation-of-state) $P=w\rho$ gives $\rho\propto a^{-3(1+w)}$. Consequently [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) scales as $a^{-4}$, [pressureless matter](../../../cosmology.md#pressureless-matter) as $a^{-3}$, and [cosmological constant energy](../../../cosmology.md#cosmological-constant) is constant. With $a_0=1$, define the present [critical density](../../../cosmology.md#critical-density) and [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) by

$$
\rho_{\mathrm{crit},0}=\frac{3H_0^2}{8\pi G},\qquad
\Omega_r=\frac{\rho_{r,0}}{\rho_{\mathrm{crit},0}},\quad
\Omega_m=\frac{\rho_{m,0}}{\rho_{\mathrm{crit},0}},\quad
\Omega_\Lambda=\frac{\Lambda}{3H_0^2}.
$$

The [Hubble constant](../../../cosmology.md#hubble-constant) $H_0$ measures the expansion rate today. Here $\Omega_r$ includes [photons](../../../quantum-mechanics.md#photon) and relativistic [neutrinos](../../../standard-model.md#neutrino), $\Omega_m$ includes [baryons](../../../physics.md#baryon) and [cold dark matter](../../../cosmology.md#cold-dark-matter), and $\Omega_\Lambda$ measures the vacuum contribution. Spatial flatness implies $\Omega_r+\Omega_m+\Omega_\Lambda=1$. Thus

$$
H^2=H_0^2(\Omega_r a^{-4}+\Omega_m a^{-3}+\Omega_\Lambda).
$$

Since [conformal time](../../../cosmology.md#conformal-time) satisfies $d\tau=dt/a$, we have $a'=a\dot a=a^2H$. Multiplication by $a^4$ proves

$$
\boxed{a'^2=H_0^2(\Omega_r+\Omega_m a+\Omega_\Lambda a^4).}
$$

For an exam-level estimate, $H_0=100h\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$ with $h\simeq0.7$, $\Omega_m\simeq0.3$, $\Omega_\Lambda\simeq0.7$, and the specified [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) gives $\Omega_r=4.2\times10^{-5}h^{-2}\simeq8.6\times10^{-5}$. These are rounded illustrative flat-universe values; precision [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) depend on the fitted model. For comparison, the base flat-model fit in [Planck 2018 cosmological parameters](https://www.aanda.org/articles/aa/abs/2020/09/aa33910-18/aa33910-18.html) gives $H_0\simeq67.4\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$ and $\Omega_m\simeq0.315$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On the expanding branch of the [Friedmann equation](../../../cosmology.md#friedmann-equations), dropping the vacuum term gives the [conformal time](../../../cosmology.md#conformal-time)

$$
\tau(a)\simeq\frac1{H_0}\int_0^a\frac{du}{\sqrt{\Omega_r+\Omega_m u}}
=\frac{2}{H_0\Omega_m}\left(\sqrt{\Omega_r+\Omega_m a}-\sqrt{\Omega_r}\right).
$$

The lower limit sets $\tau=0$ at the [Big Bang](../../../cosmology.md#big-bang). The approximation requires $\Omega_\Lambda a^4\ll\Omega_m a$, and remains safe earlier when [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) dominates. At [matter-radiation equality](../../../cosmology.md#matter-radiation-equality), $\rho_{m,0}a^{-3}=\rho_{r,0}a^{-4}$, so $a_{\rm eq}=\Omega_r/\Omega_m$. Substitution yields

$$
\boxed{\tau_{\rm eq}=\frac{2\sqrt{\Omega_r}}{H_0\Omega_m}(\sqrt2-1).}
$$

In conformal coordinates the radial [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) is $ds^2=a^2(-d\tau^2+dr^2)$. A radial light ray therefore travels a comoving distance $d r=d\tau$. The maximum distance traversed since the [Big Bang](../../../cosmology.md#big-bang) is $\int_0^{t_{\rm eq}}dt/a=\tau_{\rm eq}$: this is the [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon), rather than the instantaneous [comoving Hubble radius](../../../cosmology.md#comoving-hubble-radius) or the acoustic horizon. Restoring $c$ in the numerical conversion gives

$$
\tau_{\rm eq}\simeq
\frac{2(3000/h)\sqrt{4.2\times10^{-5}/h^2}(\sqrt2-1)}{\Omega_m}\,\mathrm{Mpc}
=\frac{16.1}{\Omega_m h^2}\,\mathrm{Mpc}.
$$

For $\Omega_m=0.3$ and $h=0.7$, the [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) at [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) is **about $110\,\mathrm{Mpc}$**. The corresponding [scale factor](../../../cosmology.md#scale-factor-cosmology) is $a_{\rm eq}\simeq2.9\times10^{-4}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Dropping [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) in the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\tau_0\simeq H_0^{-1}\int_0^1\frac{da}{\sqrt{\Omega_m a+\Omega_\Lambda a^4}}.
$$

To evaluate this [matter-vacuum conformal age integral](../../../cosmology.md#matter-vacuum-conformal-age-integral), put $a=(\Omega_m/\Omega_\Lambda)^{1/3}y$. The square root in the denominator becomes $\Omega_m^{2/3}\Omega_\Lambda^{-1/6}\sqrt{y(1+y^3)}$, whereas $da=\Omega_m^{1/3}\Omega_\Lambda^{-1/3}dy$. Therefore

$$
\boxed{\tau_0\simeq H_0^{-1}\Omega_m^{-1/3}\Omega_\Lambda^{-1/6}
\int_0^{(\Omega_\Lambda/\Omega_m)^{1/3}}\frac{dy}{\sqrt{y(1+y^3)}}.}
$$

The radiation-free approximation is not valid arbitrarily close to the lower limit. Its extension to zero nevertheless gives a good leading [conformal time](../../../cosmology.md#conformal-time) estimate: the early-time correction has size $O(H_0^{-1}\sqrt{\Omega_r}/\Omega_m)$, small compared with the total age when [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) occurs sufficiently early. The apparent $y^{-1/2}$ endpoint singularity is integrable.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

An object at [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) lies at comoving radial distance $\chi=\tau_0-\tau_{\rm eq}$ in the flat [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric). Its [angular diameter distance](../../../cosmology.md#angular-diameter-distance) is $D_A=a_{\rm eq}\chi$, while one [particle horizon](../../../cosmology.md#particle-horizon) radius has physical size $a_{\rm eq}\tau_{\rm eq}$. Its small angular radius is consequently

$$
\theta\simeq\frac{\tau_{\rm eq}}{\tau_0-\tau_{\rm eq}}
\simeq\frac{\tau_{\rm eq}}{\tau_0}.
$$

The last step uses $\tau_{\rm eq}\ll\tau_0$. If $\Omega_\Lambda/\Omega_m\gg1$, the [matter-vacuum conformal age integral](../../../cosmology.md#matter-vacuum-conformal-age-integral) tends to $I$: its integrand behaves as $y^{-1/2}$ at zero and $y^{-2}$ at infinity. Inserting the two [conformal times](../../../cosmology.md#conformal-time) gives

$$
\boxed{\theta\simeq\frac{2(\sqrt2-1)}I\,
\Omega_r^{1/2}\Omega_\Lambda^{1/6}\Omega_m^{-2/3}.}
$$

The negative matter exponent follows directly from $\Omega_m^{-1}/\Omega_m^{-1/3}$. This agrees with the original PDF; the TeX transcription drops the minus sign. If desired, $z=y^3$ evaluates the constant through the [beta function](../../../complex-analysis.md#beta-function) and [gamma function](../../../complex-analysis.md#gamma-function):

$$
I=\frac13\int_0^\infty z^{-5/6}(1+z)^{-1/2}dz
=\frac13B\left(\frac16,\frac13\right)
=\frac{\Gamma(1/6)\Gamma(1/3)}{3\sqrt\pi}.
$$

The infinite-upper-limit approximation requires vacuum dominance much stronger than in the illustrative parameters of part (a), so it is an asymptotic formula rather than a precision angular prediction for those values.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\mathcal L=-\tfrac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi-V$. In the [metric variation](../../../general-relativity.md#metric-variation) specified here, the covariant [metric tensor](../../../general-relativity.md#metric-tensor) $g_{\mu\nu}$ is varied while the [scalar field](../../../quantum-field-theory.md#scalar-field) is held fixed. Differentiating the inverse and the determinant gives

$$
\delta g^{\alpha\beta}=-g^{\alpha\mu}g^{\beta\nu}\delta g_{\mu\nu},\qquad
\delta\sqrt{-g}=\frac12\sqrt{-g}\,g^{\mu\nu}\delta g_{\mu\nu}.
$$

Thus $\delta\mathcal L=\tfrac12\partial^\mu\phi\partial^\nu\phi\,\delta g_{\mu\nu}$, and the [action](../../../classical-mechanics.md#action) varies as

$$
\delta S_M=\frac12\int d^4x\sqrt{-g}
\left(\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L\right)\delta g_{\mu\nu}.
$$

The functional derivative therefore gives $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L$. Lowering both indices yields the [stress-energy tensor of a canonical scalar field](../../../general-relativity.md#stress-energy-tensor-of-a-canonical-scalar-field):

$$
\boxed{T_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi
-g_{\mu\nu}\left(\frac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi+V\right).}
$$

The determinant variation has a positive sign because the variable is $g_{\mu\nu}$; varying the inverse [metric tensor](../../../general-relativity.md#metric-tensor) instead would reverse that intermediate sign.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the flat [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), $g^{00}=-1$, $g^{0i}=0$, and $g^{ij}=a^{-2}\delta^{ij}$. Consequently the kinetic contraction of the [scalar field](../../../quantum-field-theory.md#scalar-field) is

$$
g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi
=-\dot\phi^2+a^{-2}|\nabla\phi|^2,
\qquad
\mathcal L=\frac12\dot\phi^2-\frac12a^{-2}|\nabla\phi|^2-V.
$$

Inserting this in $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L$, with $\partial^0\phi=-\dot\phi$ and $\partial^i\phi=a^{-2}\partial_i\phi$, gives

$$
\boxed{T^{00}=\frac12\dot\phi^2+\frac12a^{-2}|\nabla\phi|^2+V,}
$$



$$
\boxed{T^{0i}=-a^{-2}\dot\phi\,\partial_i\phi,}
$$



$$
\boxed{T^{ij}=a^{-4}\partial_i\phi\partial_j\phi+
 a^{-2}\delta^{ij}\left(\frac12\dot\phi^2-\frac12a^{-2}|\nabla\phi|^2-V\right).}
$$

These are contravariant coordinate components of the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor); spatial components in an orthonormal frame carry different powers of $a$. In particular $T^{00}$ is the [energy density](../../../statistical-physics.md#energy-density) seen by the comoving observer.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Vary the [scalar field](../../../quantum-field-theory.md#scalar-field) with compactly supported variation, leaving the [metric tensor](../../../general-relativity.md#metric-tensor) fixed. The [action](../../../classical-mechanics.md#action) variation is

$$
\delta S_M=\int d^4x\sqrt{-g}
\left[-g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\delta\phi-V_{,\phi}\delta\phi\right].
$$

[Integration by parts](../../../calculus.md#integration-by-parts) moves the derivative from $\delta\phi$ and gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\Box_g\phi-V_{,\phi}=0,\qquad
\Box_g\phi=\frac1{\sqrt{-g}}\partial_\mu\left(\sqrt{-g}\,g^{\mu\nu}\partial_\nu\phi\right).
$$

For the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), $\sqrt{-g}=a^3$, so the [covariant wave operator](../../../quantum-field-theory.md#covariant-wave-operator) becomes

$$
\Box_g\phi=-a^{-3}\partial_t(a^3\dot\phi)+a^{-2}\nabla^2\phi
=-\ddot\phi-3H\dot\phi+a^{-2}\nabla^2\phi.
$$

Rearranging gives the requested [scalar field](../../../quantum-field-theory.md#scalar-field) evolution:

$$
\boxed{\ddot\phi+3\frac{\dot a}{a}\dot\phi-a^{-2}\nabla^2\phi=-V_{,\phi}.}
$$

The damping term is [Hubble friction](../../../cosmology.md#hubble-friction); it comes from the expanding volume factor $a^3$, not from a microscopic dissipative force.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a homogeneous [scalar field](../../../quantum-field-theory.md#scalar-field), every spatial derivative vanishes. The [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) consequently has no [momentum density](../../../general-relativity.md#momentum-density) or directional stress:

$$
T^{0i}=0,\qquad T^{ij}=Pa^{-2}\delta^{ij},\qquad
\rho=\frac12\dot\phi^2+V,\quad P=\frac12\dot\phi^2-V.
$$

The only spatial tensor left is $\delta^{ij}$, so the stress is isotropic. This is the [perfect fluid](../../../general-relativity.md#perfect-fluid) form in its comoving frame. Now expand the time component of [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) using the [covariant derivative](../../../general-relativity.md#covariant-derivative):

$$
0=\nabla_\mu T^{\mu0}
=\partial_\mu T^{\mu0}+\Gamma^\mu{}_{\mu\lambda}T^{\lambda0}
+\Gamma^0{}_{\mu\lambda}T^{\mu\lambda}.
$$

The first term is $\dot\rho$. In the second, only $\lambda=0$ contributes, and $\sum_i\Gamma^i{}_{i0}=3H$, giving $3H\rho$. The third is

$$
\sum_{i,j}(a\dot a\delta_{ij})(Pa^{-2}\delta^{ij})=3HP.
$$

Here the quoted [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) include their lower-index symmetry $\Gamma^i{}_{j0}=\Gamma^i{}_{0j}$. Therefore the [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) is

$$
\boxed{\dot\rho=-3\frac{\dot a}{a}(\rho+P).}
$$

As a check using the [scalar field](../../../quantum-field-theory.md#scalar-field) equation, $\dot\rho=\dot\phi(\ddot\phi+V_{,\phi})=-3H\dot\phi^2=-3H(\rho+P)$, with exactly the same sign.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

With zero [scalar potential](../../../quantum-field-theory.md#scalar-potential) and a homogeneous [scalar field](../../../quantum-field-theory.md#scalar-field), the preceding [perfect fluid](../../../general-relativity.md#perfect-fluid) identification gives

$$
\boxed{P=\rho=\frac12\dot\phi^2.}
$$

This [equation of state](../../../thermodynamics.md#equation-of-state) is that of a [stiff fluid](../../../general-relativity.md#stiff-fluid). The field equation integrates to $a^3\dot\phi=K$, since $\partial_t(a^3\dot\phi)=0$. Hence $\rho=K^2/(2a^6)$, agreeing with the [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) for $w=1$. If this nonzero component dominates a flat universe, the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\left(\frac{\dot a}{a}\right)^2=\frac{4\pi G K^2}{3a^6},\qquad
\dot a=\sqrt{\frac{4\pi G}{3}}\,|K|a^{-2}
$$

on the expanding branch. Integrating once more, $a^3=3\sqrt{4\pi G/3}\,|K|(t-t_B)$. Choosing the [Big Bang](../../../cosmology.md#big-bang) at $t_B=0$ yields

$$
\boxed{a(t)\propto t^{1/3}.}
$$

The [homogeneous free scalar as a stiff fluid](../../../general-relativity.md#homogeneous-free-scalar-as-a-stiff-fluid) construction requires $K\ne0$; a constant zero-potential field has zero [energy density](../../../statistical-physics.md#energy-density) and cannot dominate this expansion.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Work in [natural units](../../../physics.md#natural-units) $\hbar=c=k_B=1$, at [temperatures](../../../thermodynamics.md#temperature) far below the $W$-boson mass but of order or above the [Electron](../../../physics.md#electron) mass. The [Fermi interaction](../../../quantum-field-theory.md#fermi-interaction) then supplies a local four-fermion amplitude. The [Fermi constant](../../../quantum-field-theory.md#fermi-constant) has dimension energy$^{-2}$. In scattering of a thermal lepton from a nonrelativistic nucleon, the nucleon current matrix element has size $m_N$, while the lepton current has size $T$. Thus $\mathcal M\sim G_Fm_NT$. The two-body [relativistic scattering cross-section](../../../quantum-mechanics.md#relativistic-scattering-cross-section) contains the kinematic factor $s^{-1}\sim m_N^{-2}$; when the final and initial lepton energies are comparable, their momentum ratio is of order one. Consequently $\sigma\sim|\mathcal M|^2/m_N^2\sim G_F^2T^2$. This estimates [temperatures](../../../thermodynamics.md#temperature) above the [Electron](../../../physics.md#electron) mass and mass-splitting thresholds; those scales only affect the dimensionless rate function near freeze-out.

The light leptons in the thermal bath have [number density](../../../statistical-physics.md#number-density) $n\sim T^3$ and speed of order unity. Their conversion rate per nucleon is therefore

$$
\boxed{\Gamma_{n\leftrightarrow p}\sim n\langle\sigma v\rangle\sim G_F^2T^5.}
$$

For example, $n+\nu_e\leftrightarrow p+e^-$ and $n+e^+\leftrightarrow p+\bar\nu_e$ change the [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio). The bath density here is the lepton density, not the much smaller [baryon](../../../physics.md#baryon) density. Dimensionless weak couplings, phase-space integrals and the several reaction channels set a numerical coefficient. [Electron](../../../physics.md#electron) masses and the neutron-proton splitting also become important for a precision rate near [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), the [effective number of relativistic energy degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-energy-degrees-of-freedom), denoted $g_*$, gives the [energy density](../../../statistical-physics.md#energy-density)

$$
\rho_R=\frac{\pi^2}{30}g_*T^4.
$$

The paper's $\mathcal N_{\rm eff}$ is this $g_*$; it is not the conventionally normalized effective number of [neutrino](../../../standard-model.md#neutrino) species. With the specified [reduced Planck mass](../../../physics.md#reduced-planck-mass), the [Friedmann equation](../../../cosmology.md#friedmann-equations) reads $H^2=\rho_R/(3M_{\rm Pl}^2)$, whence

$$
H=\sqrt{\frac{\pi^2g_*}{90}}\frac{T^2}{M_{\rm Pl}}.
$$

Write the [weak interaction](../../../standard-model.md#weak-interaction) conversion rate as $\Gamma=A G_F^2T^5$. The ratio $\Gamma/H$ scales as $T^3$, so it falls during cooling: conversion eventually becomes too slow to maintain [neutron-proton chemical equilibrium](../../../cosmology.md#neutron-proton-chemical-equilibrium). Equating the conversion and expansion rates gives

$$
T_F=\left[\frac{\sqrt{\pi^2g_*/90}}{A G_F^2M_{\rm Pl}}\right]^{1/3}.
$$

On suppressing the numerical coefficient, the [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out) [temperature](../../../thermodynamics.md#temperature) is consequently

$$
\boxed{T_F\sim G_F^{-2/3}\mathcal N_{\rm eff}^{1/6}M_{\rm Pl}^{-1/3}.}
$$

The one-sixth power reflects a balance between a conversion rate proportional to $T^5$ and a [Hubble parameter](../../../cosmology.md#hubble-parameter) proportional to $\sqrt{g_*}\,T^2$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Before [electron-positron annihilation in cosmology](../../../cosmology.md#electron-positron-annihilation-in-cosmology), [photons](../../../quantum-mechanics.md#photon) contribute two [helicity](../../../special-relativity.md#helicity) states; [Electrons](../../../physics.md#electron) and positrons contribute two spin states each. Each of the three light [neutrino](../../../standard-model.md#neutrino) flavours contributes one active [neutrino](../../../standard-model.md#neutrino) [helicity](../../../special-relativity.md#helicity) and one antineutrino [helicity](../../../special-relativity.md#helicity). At a common [temperature](../../../thermodynamics.md#temperature) the [effective number of relativistic energy degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-energy-degrees-of-freedom) is therefore

$$
\boxed{g_*=2+\frac78(4+6)=\frac{43}{4}=10.75.}
$$

Using $G_F=1.17\times10^{-5}\,\mathrm{GeV}^{-2}$ and $M_{\rm Pl}\simeq2.435\times10^{18}\,\mathrm{GeV}$ in the scaling formula alone gives $T_F\sim2\,\mathrm{MeV}$. Including the explicit expansion coefficient from (ii), but setting the unknown rate coefficient $A$ to one, gives $T_F\simeq1.5\,\mathrm{MeV}$. Thus the warranted conclusion is **a freeze-out [temperature](../../../thermodynamics.md#temperature) of order $1\,\mathrm{MeV}$**, above the $0.511\,\mathrm{MeV}$ [Electron](../../../physics.md#electron) mass. The omitted weak-rate coefficient prevents a more precise prediction from this estimate.

[Neutrino decoupling](../../../cosmology.md#neutrino-decoupling) occurs before most electron-positron pairs annihilate. Afterwards [neutrinos](../../../standard-model.md#neutrino) redshift freely, $T_\nu a=\mathrm{constant}$, while the [photons](../../../quantum-mechanics.md#photon) receive the pair [entropy](../../../thermodynamics.md#entropy). For the still-coupled photon-pair gas, [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) gives $g_{*s}T_\gamma^3a^3=\mathrm{constant}$. Its [entropy](../../../thermodynamics.md#entropy) degrees of freedom drop from $2+(7/8)4=11/2$ to $2$. Comparing this with the freely cooling [neutrinos](../../../standard-model.md#neutrino) gives

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac4{11}\right)^{1/3},\qquad
\frac{T_\gamma}{T_\nu}=\left(\frac{11}{4}\right)^{1/3}.}
$$

After annihilation, [photon](../../../quantum-mechanics.md#photon) and [neutrino](../../../standard-model.md#neutrino) [temperatures](../../../thermodynamics.md#temperature) differ. To write the total [energy density](../../../statistical-physics.md#energy-density) as $(\pi^2/30)g_*T_\gamma^4$, the [neutrino](../../../standard-model.md#neutrino) contribution must include that [temperature](../../../thermodynamics.md#temperature) ratio:

$$
\boxed{g_*=2+\frac78\,6\left(\frac4{11}\right)^{4/3}\simeq3.36.}
$$

This is the paper's post-annihilation $\mathcal N_{\rm eff}$. Merely deleting the [Electron](../../../physics.md#electron) term while keeping all species at the same [temperature](../../../thermodynamics.md#temperature) would be incorrect. For comparison the [entropy](../../../thermodynamics.md#entropy) count, normalized to $T_\gamma^3$, is $g_{*s}=2+(7/8)6(4/11)=43/11\simeq3.91$. These results assume instantaneous [neutrino decoupling](../../../cosmology.md#neutrino-decoupling) and relativistic [neutrinos](../../../standard-model.md#neutrino); the two counts represent different thermal moments.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The nucleons are nonrelativistic, so the [Maxwell-Boltzmann distribution](../../../statistical-physics.md#maxwell-boltzmann-distribution) gives

$$
n_i=g_i\left(\frac{m_iT}{2\pi}\right)^{3/2}e^{(\mu_i-m_i)/T},\qquad i=n,p.
$$

Both spin degeneracies are two. Taking the ratio and using the specified negligible [chemical potentials](../../../thermodynamics.md#chemical-potential) yields the [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio)

$$
r_F=\left(\frac{m_n}{m_p}\right)^{3/2}e^{-(m_n-m_p)/T_F}
\simeq\boxed{e^{-Q/T_F}}.
$$

The mass prefactor differs from unity only at the per-mille level. The dependence on $T_F$ is much stronger: $d\ln r_F/d\ln T_F=Q/T_F>0$. Thus **earlier, hotter weak freeze-out leaves more [neutrons](../../../physics.md#neutron) relative to [protons](../../../physics.md#proton)**. For illustration, $T_F=1\,\mathrm{MeV}$ gives $r_F\simeq0.28$; $T_F=0.8\,\mathrm{MeV}$ gives $r_F\simeq0.20$. [Free-neutron decay after freeze-out](../../../cosmology.md#free-neutron-decay-after-freeze-out) lowers the ratio further before most [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) takes place.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

The small [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) suppresses nuclear equilibrium abundances through the factor $\eta^{A-1}$. Cooling eventually makes the binding-energy exponential favourable, but the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck) delays substantial nuclear burning until well after [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out). In ordinary [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), nearly every [neutron](../../../physics.md#neutron) surviving that delay ends up in helium-4. This makes the final [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) chiefly a [neutron](../../../physics.md#neutron) budget rather than an unrestricted equilibrium abundance.

Let $r_F$ be the [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio) at freeze-out, let $\Delta t$ be the delay until effective nuclear burning, and let $\tau_n$ be the [neutron](../../../physics.md#neutron) mean lifetime. The initial fraction of [baryons](../../../physics.md#baryon) which are [neutrons](../../../physics.md#neutron) is $x_{n,F}=r_F/(1+r_F)$. Because [neutron](../../../physics.md#neutron) decay converts a [neutron](../../../physics.md#neutron) into a [proton](../../../physics.md#proton), total [baryon number](../../../standard-model.md#baryon-number) remains constant, while the [neutron](../../../physics.md#neutron) fraction becomes $x_{n,B}=x_{n,F}e^{-\Delta t/\tau_n}$. Each helium nucleus uses two [neutrons](../../../physics.md#neutron) and four [baryons](../../../physics.md#baryon). Hence [neutron-limited helium synthesis](../../../cosmology.md#neutron-limited-helium-synthesis) gives

$$
\boxed{Y_4\simeq\frac{2r_F}{1+r_F}e^{-\Delta t/\tau_n},\qquad
\tau_n=\frac{\tau_{1/2}(n)}{\ln2}.}
$$

Equivalently, $Y_4=2r_B/(1+r_B)$ with $r_B=x_{n,B}/(1-x_{n,B})$. This accounts for the extra [protons](../../../physics.md#proton) produced by [neutron](../../../physics.md#neutron) decay; multiplying $r_F$ alone by the survival factor would miss their contribution. The following responses refer to ordinary neutron-limited burning, without exotic particle injection or a change to the nuclear network.

<h4 id="3/v/a">a</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/a/solution">Solution</h5>

↑ **Parent:** [A](#3/v/a)

Extra relativistic [neutrino](../../../standard-model.md#neutrino) species increase the [effective number of relativistic energy degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-energy-degrees-of-freedom). At fixed [temperature](../../../thermodynamics.md#temperature) the [Hubble parameter](../../../cosmology.md#hubble-parameter) rises as $g_*^{1/2}$, while the standard conversion rate is unchanged. Consequently [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out) moves to higher [temperature](../../../thermodynamics.md#temperature), $T_F\propto g_*^{1/6}$, and the [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio) $r_F=e^{-Q/T_F}$ increases. The initial [neutron](../../../physics.md#neutron) fraction $r_F/(1+r_F)$ therefore increases as well.

The quicker expansion also reduces the cosmic time required to cool to the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck) [temperature](../../../thermodynamics.md#temperature): during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $t\propto g_*^{-1/2}T^{-2}$ while the thermal count is roughly constant. Fewer [neutrons](../../../physics.md#neutron) decay before burning. Both factors in the [neutron](../../../physics.md#neutron) budget increase, giving **a larger final helium-4 mass fraction**. This is the [primordial helium response to extra relativistic species](../../../cosmology.md#primordial-helium-response-to-extra-relativistic-species), under the assumption that the additional species contribute mainly to expansion rather than independently changing the conversion rates.

<h4 id="3/v/b">b</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/b/solution">Solution</h5>

↑ **Parent:** [B](#3/v/b)

A longer [neutron](../../../physics.md#neutron) [half-life](../../../analysis.md#half-life) means a larger mean lifetime $\tau_n=\tau_{1/2}/\ln2$. Holding the initial [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio) and the nuclear-burning delay fixed, the derivative of the [neutron](../../../physics.md#neutron) survival factor is positive:

$$
\frac{\partial\ln Y_4}{\partial\tau_n}=\frac{\Delta t}{\tau_n^2}>0.
$$

Thus fewer [neutrons](../../../physics.md#neutron) disappear during the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck), and **the final helium-4 mass fraction increases**.

There can be a second effect if the increased lifetime represents a uniform reduction of the relevant [weak interaction](../../../standard-model.md#weak-interaction) strength. With fixed masses and other couplings, [neutron](../../../physics.md#neutron) decay and the conversion reactions both scale as $G_F^2$. Thus $\tau_n\propto G_F^{-2}$, whereas $T_F\propto G_F^{-2/3}\propto\tau_n^{1/3}$. Weaker conversion then freezes out earlier and increases $r_F$, reinforcing the survival effect. The survival argument alone already establishes the requested [neutron half-life effect on primordial helium](../../../cosmology.md#neutron-half-life-effect-on-primordial-helium); linking lifetime to all conversion rates additionally requires this microscopic assumption.

<h4 id="3/v/c">c</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/c/solution">Solution</h5>

↑ **Parent:** [C](#3/v/c)

A larger [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) favours bound nuclei at a fixed [temperature](../../../thermodynamics.md#temperature) through the equilibrium factor $\eta^{A-1}$. In particular it helps deuterium survive photodissociation sooner: there are fewer energetic [photons](../../../quantum-mechanics.md#photon) per [baryon](../../../physics.md#baryon), and nuclear reaction rates per [baryon](../../../physics.md#baryon) also rise. A schematic [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck) condition is $\eta e^{B_D/T_B}\sim\mathrm{constant}$, suppressing slowly varying powers of [temperature](../../../thermodynamics.md#temperature). It gives

$$
\frac{B_D}{T_B}\simeq\mathrm{constant}-\ln\eta,\qquad
\frac{dT_B}{d\ln\eta}\simeq\frac{T_B^2}{B_D}>0.
$$

Thus higher $\eta$ permits burning at a higher [temperature](../../../thermodynamics.md#temperature). During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) that means earlier cosmic time, $t_B\propto T_B^{-2}$, leaving less time for [free-neutron decay after freeze-out](../../../cosmology.md#free-neutron-decay-after-freeze-out). More [neutrons](../../../physics.md#neutron) enter helium, so **the final helium-4 mass fraction increases**, ordinarily rather weakly. This is the [baryon-density effect on primordial helium](../../../cosmology.md#baryon-density-effect-on-primordial-helium).

The equilibrium helium factor $\eta^3$ indicates the direction of the change but is not a prediction that the final helium abundance grows without bound as $\eta^3$. Once almost all surviving [neutrons](../../../physics.md#neutron) are captured, the final [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) is limited by their supply, as the shared [neutron](../../../physics.md#neutron) budget shows.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $\delta=\delta_{C,\mathbf k}$ and $\mathcal H=a'/a$, the [conformal Hubble parameter](../../../cosmology.md#conformal-hubble-parameter). The flat [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\mathcal H^2=\frac{8\pi G}{3}a^2(\rho_C+\rho_R).
$$

Outside the horizon, the stated [adiabatic cosmological perturbation](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) relation is $\delta_R=(4/3)\delta$. It expresses equality of $\delta_i/(1+w_i)$ for dust and radiation in the density convention of the supplied equations. During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $a\propto\tau$, so $\mathcal H=1/\tau$ and $\rho_C$ is negligible. Consequently $8\pi Ga^2\rho_R=3/\tau^2$, and the [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md) equation becomes

$$
\delta''+\frac1\tau\delta'=\frac4{\tau^2}\delta.
$$

The trial solution $\delta\propto\tau^q$ gives $q(q-1)+q=4$, hence $q=2,-2$.

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $a\propto\tau^2$, so $\mathcal H=2/\tau$. Now the radiation source is negligible and $4\pi Ga^2\rho_C=(3/2)\mathcal H^2=6/\tau^2$. The equation becomes

$$
\delta''+\frac2\tau\delta'=\frac6{\tau^2}\delta,
$$

whose exponents satisfy $q(q-1)+2q=6$, or $(q-2)(q+3)=0$. Thus the growing solutions in both eras are

$$
\boxed{\delta_{C,\mathbf k}\propto\tau^2.}
$$

The other modes are $\tau^{-2}$ in the radiation limit and $\tau^{-3}$ in the matter limit. These are statements in the density and gauge convention of the supplied evolution equation; a density contrast outside the horizon is not a gauge-independent observable by itself.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

After [cosmological horizon crossing](../../../linear-cosmological-density-perturbation.md#cosmological-horizon-crossing), the rapidly oscillating radiation source can be averaged away as specified. Well inside [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), the remaining [cold dark matter](../../../cosmology.md#cold-dark-matter) self-gravity is also subleading because $\rho_C/\rho_R\ll1$. To leading order the [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md) equation is therefore

$$
\delta''+\frac1\tau\delta'\simeq0,
\qquad (\tau\delta')'\simeq0.
$$

Two integrations give

$$
\boxed{\delta(\tau)\simeq A+B\ln\left(\frac{\tau}{\tau_H}\right),\qquad \tau_H\sim k^{-1}.}
$$

The reference time makes the logarithm dimensionless. A growing superhorizon mode reaches entry with a nonzero derivative, so matching generally excites $B\ne0$. For example, an abrupt leading-order match from $\delta\propto\tau^2$ gives $B=\tau_H\delta'_H\simeq2\delta_H$, whereas its exact numerical coefficient depends on the transition and the radiation forcing.

This logarithmic growth is the [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect). It is an asymptotic radiation-era result: after dropping the oscillating radiation perturbation, the original equation still contains $4\pi Ga^2\rho_C\delta$. Retaining that term and the changing background leads to the [Mészáros equation](../../../linear-cosmological-density-perturbation.md#meszaros-equation), which provides the interpolation near [matter-radiation equality](../../../cosmology.md#matter-radiation-equality). It would be incorrect to claim that a pure logarithm solves the complete mixed-background equation exactly.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), the radiation source can be neglected irrespective of whether the mode is inside or outside the horizon in the supplied [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md) equation. The [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $\mathcal H=2/\tau$ and $4\pi Ga^2\rho_C=6/\tau^2$, just as in part (a). Therefore

$$
\delta''+\frac2\tau\delta'-\frac6{\tau^2}\delta=0.
$$

Substituting $\tau^q$ gives $(q-2)(q+3)=0$, so for every [Fourier mode](../../../fourier-analysis.md#fourier-mode)

$$
\delta_{C,\mathbf k}=A_{\mathbf k}\tau^2+B_{\mathbf k}\tau^{-3}.
$$

Thus the [matter-era growing and decaying density modes](../../../linear-cosmological-density-perturbation.md#matter-era-growing-and-decaying-density-modes) have **growing behaviour $\delta_{C,\mathbf k}\propto\tau^2\propto a$ for all $k$**. There is no pressure-gradient term introducing a $k$-dependent growth rate for [cold dark matter](../../../cosmology.md#cold-dark-matter). The coefficients retain their different earlier histories; common growth does not erase the spectral shape. A specially chosen pure decaying solution is of course possible, so the growing-mode statement does not assert that every initial condition grows.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $P(k,\tau)=\langle|\delta_{C,\mathbf k}|^2\rangle$ be the [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) in the normalization of the question. The [Harrison-Peebles-Zeldovich spectrum](../../../linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum) gives $P\sim\mathcal C\tau^4k$ before entry. Using the order-of-magnitude [cosmological horizon crossing](../../../linear-cosmological-density-perturbation.md#cosmological-horizon-crossing) criterion $k\tau_H\sim1$, rather than tracking a wavelength factor of $2\pi$, gives

$$
P(k,\tau_H)\sim\mathcal C k^{-3}.
$$

The mass-fluctuation [variance](../../../variance.md) on radius $k^{-1}$ is therefore

$$
\boxed{\left\langle\left(\frac{\delta M}{M}\right)_k^2\right\rangle_H
\sim k^3P(k,\tau_H)\sim\mathcal C,}
$$

independent of [wavenumber](../../../wave-equation.md#wavenumber). Equal logarithmic ranges of scales enter with comparable dimensionless fluctuation strength. This is the [scale invariance](../../../mathematics.md#scale-invariance) encoded by the [HPZ spectrum](../../../linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum); it is not the claim that the dimensional [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) is independent of $k$ at a fixed time.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

First consider $k\tau_{\rm eq}<1$. Such a mode remains outside the horizon through [matter-radiation equality](../../../cosmology.md#matter-radiation-equality), grows as $\tau^2$ on both sides, and keeps the same matter-era growth after entry. Squaring this growth preserves the shape of the [HPZ spectrum](../../../linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum):

$$
P(k,\tau)\sim\mathcal C\tau^4 k,\qquad k\tau_{\rm eq}<1,
$$

up to a scale-independent matching coefficient.

For $k\tau_{\rm eq}\gg1$, entry occurs in [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) at $\tau_H\sim k^{-1}$, with $P_H\sim\mathcal C k^{-3}$. The density amplitude then grows only logarithmically until equality. Thus

$$
\delta_{\rm eq}\sim\delta_H\ln(k\tau_{\rm eq}),\qquad
P_{\rm eq}\sim\mathcal C k^{-3}\ln^2(k\tau_{\rm eq}).
$$

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), the [matter-era linear growth factor](../../../linear-cosmological-density-perturbation.md#matter-era-linear-growth-factor) of the density is $(\tau/\tau_{\rm eq})^2$, so its square multiplies the [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum):

$$
\boxed{P(k,\tau)\sim\mathcal C
\left(\frac{\tau}{\tau_{\rm eq}}\right)^4
k^{-3}\ln^2(k\tau_{\rm eq}),\qquad k\tau_{\rm eq}\gg1.}
$$

The turnover at $k\sim\tau_{\rm eq}^{-1}$ records whether a mode entered during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination). Earlier-entering small-scale modes miss the rapid $\tau^2$ growth and receive only the logarithmic [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect). This is the origin of the [logarithmic small-scale matter transfer](../../../linear-cosmological-perturbation-theory.md#logarithmic-small-scale-matter-transfer). The formula is a large-$k$ asymptote: the additive constant in the logarithmic solution and smooth equality matching must be retained near $k\tau_{\rm eq}=1$, where the spectrum does not vanish.

Multiplying by $k^3$ gives the small-scale mass-fluctuation [variance](../../../variance.md)

$$
\boxed{\left\langle\left(\frac{\delta M}{M}\right)_k^2\right\rangle
\sim\mathcal C\left(\frac{\tau}{\tau_{\rm eq}}\right)^4
\ln^2(k\tau_{\rm eq}).}
$$

This gives the requested estimate for modes entering before equality, with the logarithm replaced by a smooth order-one factor in the transition region. On comoving scale $L\sim k^{-1}$, unit variance today requires

$$
\boxed{\mathcal C\sim
\frac{(\tau_{\rm eq}/\tau_0)^4}{\ln^2(\tau_{\rm eq}/L)}.}
$$

For a numerical illustration faithful to this question's flat, matter-plus-radiation background, take $h=0.7$ and $\Omega_r=4.2\times10^{-5}h^{-2}$, hence $\Omega_C=1-\Omega_r\simeq1$ rather than the $0.3$ appropriate to a vacuum-dominated model. Part 1(b), now with $\Omega_m=\Omega_C$, gives $\tau_{\rm eq}\simeq33\,\mathrm{Mpc}$. In this two-component model the same integral is valid all the way to today, giving

$$
\tau_0=\frac{2}{H_0\Omega_C}
\left(\sqrt{\Omega_r+\Omega_C}-\sqrt{\Omega_r}\right)
\simeq8.5\times10^3\,\mathrm{Mpc}.
$$

With $L=3\,\mathrm{Mpc}$, $\tau_0/\tau_{\rm eq}\simeq258$ and $\ln(\tau_{\rm eq}/L)\simeq2.39$. Therefore $\mathcal C\sim[258^4(2.39)^2]^{-1}\simeq4\times10^{-11}$, corresponding to a horizon-entry root-mean-square fluctuation of roughly $6\times10^{-6}$. **A very small primordial amplitude, of order $10^{-10}$ in this schematic normalization, can reach unit small-scale variance by today.** Factors from the Fourier convention, smoothing window and equality matching preclude a precise normalization here. The calculation marks the onset of nonlinear structure formation, where extrapolating the linear solution ceases to be valid. For a universe with late vacuum domination, one must replace the matter-only growth law by its actual growth factor before making a numerical inference.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
