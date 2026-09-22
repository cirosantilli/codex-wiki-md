# Paper 315

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_315.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_315.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
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

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the plane-parallel [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation)

$$
\mu\frac{dI_\nu}{d\tau_\nu}=I_\nu-S_\nu,
$$

angular integration gives the zeroth [radiation-field moment](../../../astrophysics.md#radiation-field-moment) equation

$$
\frac{dH_\nu}{d\tau_\nu}=J_\nu-S_\nu.
$$

The net radiative heating per unit volume is therefore

$$
4\pi\int_0^\infty\alpha_\nu(J_\nu-S_\nu)\,d\nu.
$$

[Radiative equilibrium](../../../thermodynamics.md#radiative-equilibrium) requires it to vanish, equivalently that the frequency-integrated [radiative flux](../../../astrophysics.md#radiative-flux) be independent of depth:

$$
\boxed{\int_0^\infty\alpha_\nu(J_\nu-S_\nu)\,d\nu=0}.
$$

In [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium) with [coherent isotropic scattering](../../../astrophysics.md#coherent-isotropic-scattering),

$$
S_\nu=(1-\omega_\nu)B_\nu(T)+\omega_\nu J_\nu,
$$

where $\omega_\nu$ is the [single-scattering albedo](../../../astrophysics.md#single-scattering-albedo). Since $\alpha_\nu(1-\omega_\nu)=\alpha_{\nu,\rm abs}$, the condition becomes

$$
\boxed{\int_0^\infty\alpha_{\nu,\rm abs}
[J_\nu-B_\nu(T)]\,d\nu=0}.
$$

Conservative scattering redistributes directions but contributes no net material heating.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $\mu=\cos\theta$. For $I_\nu=A_\nu+B_\nu\mu^3$, the [mean intensity](../../../astrophysics.md#mean-intensity) is

$$
J_\nu=\frac12\int_{-1}^{1}I_\nu\,d\mu=A_\nu,
$$

because the cubic term is odd. The K-integral, or second angular moment, is

$$
K_\nu=\frac12\int_{-1}^{1}\mu^2I_\nu\,d\mu
=\frac{A_\nu}{3},
$$

because the $\mu^5$ contribution is also odd. Hence

$$
\boxed{K_\nu=\frac13J_\nu}.
$$

This intensity obeys the [Eddington closure approximation](../../../astrophysics.md#eddington-closure-approximation) even though it is not isotropic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Deep in an optically thick [grey atmosphere](../../../astrophysics.md#grey-atmosphere), write $I_\nu=B_\nu+\delta I_\nu$ and retain the first spatial-gradient correction in the transfer equation:

$$
\delta I_\nu\simeq-\frac{\mu}{\kappa\rho}
\frac{dB_\nu}{dz}.
$$

Angular and frequency integration then gives the [radiative diffusion](../../../astrophysics.md#radiative-diffusion) flux

$$
F=-\frac{16\sigma T^3}{3\kappa\rho}\frac{dT}{dz}.
$$

For a thin [plane-parallel atmosphere](../../../astrophysics.md#plane-parallel-atmosphere), constant [Rosseland mean opacity](../../../astrophysics.md#rosseland-mean-opacity) $\kappa$, negligible external irradiation, and radius nearly equal to $R$, radiative equilibrium gives $F=L/(4\pi R^2)$. Therefore

$$
\boxed{\frac{dT}{dz}
=-\frac{3\kappa\rho L}{64\pi\sigma R^2T^3}}.
$$

With hydrostatic balance $dP/dz=-\rho g$, the equivalent pressure form is

$$
\boxed{\frac{dT}{dP}=\frac{3\kappa L}{64\pi\sigma GM\,T^3}},
$$

where $g=GM/R^2$.

## 2

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let brackets denote number densities and impose a local [photochemical steady state](../../../exoplanet.md#photochemical-steady-state). The atomic-oxygen and ozone balances are

$$
2J_1[{\rm O}_2]+J_3[{\rm O}_3]
=K_2[{\rm O}][{\rm O}_2][{\rm M}]
+K_4[{\rm O}][{\rm O}_3],
$$



$$
K_2[{\rm O}][{\rm O}_2][{\rm M}]
=J_3[{\rm O}_3]+K_4[{\rm O}][{\rm O}_3].
$$

Subtracting gives $J_1[{\rm O}_2]=K_4[{\rm O}][{\rm O}_3]$. If photodissociation is the dominant direct ozone loss, $J_3[{\rm O}_3]\gg K_4[{\rm O}][{\rm O}_3]$, the second balance becomes $K_2[{\rm O}][{\rm O}_2][{\rm M}]\simeq J_3[{\rm O}_3]$. Eliminating atomic oxygen yields the [Chapman ozone equilibrium](../../../exoplanet.md#chapman-ozone-equilibrium)

$$
\boxed{[{\rm O}_3]\simeq[{\rm O}_2]
\left(\frac{K_2J_1[{\rm M}]}{K_4J_3}\right)^{1/2}}.
$$

High in the atmosphere ultraviolet photons make $J_1$ large but the third-body density is small; low down, $[{\rm M}]$ is large but O2-dissociating ultraviolet radiation has been absorbed. Their product peaks at intermediate altitude, producing an [ozone layer](../../../exoplanet.md#ozone-layer).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Comparable hydrostatic thermal escape requires comparable [Jeans escape parameter](../../../exoplanet.md#jeans-escape-parameter) $\lambda=GM_pm/(k_BTR_{\rm exo})$. For the same escaping species and $R_{\rm exo}\simeq R_p$,

$$
\frac{T_{\rm J}}{T_\oplus}
\gtrsim\frac{M_{\rm J}/R_{\rm J}}{M_\oplus/R_\oplus}
\simeq\frac{318}{11.2}\simeq28.
$$

Thus Jupiter at 5 au needs an exobase temperature at least about thirty times Earth's at the same irradiation to have comparable [Jeans escape flux](../../../exoplanet.md#jeans-escape-flux).

For the inner planet, the usable EUV power is $\eta\pi R_{\rm exo}^2F_{\rm EUV}$. If the binding energy per unit escaping mass is $GM_p/R_p$, [energy-limited atmospheric escape](../../../exoplanet.md#energy-limited-atmospheric-escape) gives

$$
\dot M=\frac{\eta\pi R_{\rm exo}^2F_{\rm EUV}R_p}{GM_p}.
$$

The time to lose a fraction $x$ of the planetary mass is therefore

$$
\boxed{t_x=\frac{xGM_p^2}
{\eta\pi R_{\rm exo}^2R_pF_{\rm EUV}}}.
$$

This neglects Roche-lobe reduction, radiative cooling, changes in radius and flux, and the planet's orbital evolution. If the gas is lifted only from $R_{\rm exo}$, replace $R_p$ in the denominator by $R_{\rm exo}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

At [exoplanet secondary eclipse](../../../exoplanet.md#exoplanet-secondary-eclipse), the full-phase planet-star flux ratio is the sum of reflected and thermal light. Approximating both bodies as unresolved blackbodies and taking wavelength-independent [geometric albedo](../../../exoplanet.md#geometric-albedo),

$$
\boxed{
\frac{F_{p,\lambda}}{F_{*,\lambda}}
=A_g\left(\frac{R_p}{a}\right)^2
+\left(\frac{R_p}{R_*}\right)^2
\frac{B_\lambda(T_p)}{B_\lambda(T_*)}}.
$$

The first term is a flat reflected-light level under the stated constant-albedo assumption. At short wavelength the cool planet lies in the [Wien limit](../../../astrophysics.md#wien-approximation), so thermal emission is exponentially suppressed and reflection dominates. At long wavelength both spectra enter the [Rayleigh-Jeans law](../../../astrophysics.md#rayleigh-jeans-law), giving

$$
\frac{F_{p,\lambda}}{F_{*,\lambda}}
\longrightarrow A_g\left(\frac{R_p}{a}\right)^2
+\left(\frac{R_p}{R_*}\right)^2\frac{T_p}{T_*}.
$$

The sketch therefore starts on the reflected plateau, rises where planetary [blackbody radiation](../../../statistical-physics.md#black-body-radiation) becomes important, and asymptotically approaches the long-wavelength plateau. This neglects spectral albedo features, phase dependence, stellar lines, and a nonisothermal planetary photosphere.

<a id="2/c/image-schematic-wavelength-dependence-of-a-planet-star-flux-ratio-at-secondary-eclipse"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-315-planet-star-flux-ratio.png)

**[Figure 1](#2/c/image-schematic-wavelength-dependence-of-a-planet-star-flux-ratio-at-secondary-eclipse). Schematic wavelength dependence of a planet-star flux ratio at secondary eclipse**. Reflected light sets a short-wavelength plateau, planetary blackbody emission produces a thermal rise, and the sum approaches its Rayleigh--Jeans plateau at long wavelength. The temperatures and radii are illustrative rather than a fit to a particular planet.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

At fixed temperature and pressure, [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium) minimizes the [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy) subject to elemental conservation. For every independent reaction with stoichiometric coefficients $\nu_i$,

$$
\boxed{\Delta_rG=\sum_i\nu_i\mu_i=0}.
$$

Equivalently, forward and reverse rates satisfy detailed balance. For ideal gases,

$$
\boxed{\prod_i\left(\frac{p_i}{p^\circ}\right)^{\nu_i}
=K_p(T)=\exp\left[-\frac{\Delta_rG^\circ(T)}{RT}\right]}.
$$

## 3

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a spherical [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) with $P=K\rho^{1+1/n}$, the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation) gives

$$
R\propto K^{1/2}\rho_c^{(1-n)/(2n)},
\qquad
M\propto K^{3/2}\rho_c^{(3-n)/(2n)}.
$$

Eliminating the central density at fixed composition and entropy gives the [polytropic mass-radius relation](../../../stellar-structure.md#polytropic-mass-radius-relation)

$$
\boxed{R\propto M^\beta,\qquad
\beta=\frac{1-n}{3-n}}.
$$

An incompressible rocky body has $n=0$ and $\beta=1/3$. A moderately massive gas giant is approximately an $n=1$ polytrope and has $\beta=0$, explaining its weak radius dependence on mass. In a more strongly degenerate nonrelativistic regime, $n=3/2$ gives $\beta=-1/3$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assemble a uniform-density sphere from shells. Since $m(r)=M(r/R)^3$ and $dm=3Mr^2dr/R^3$,

$$
U=-\int_0^R\frac{Gm(r)}r\,dm
=-\frac{3GM^2}{R^6}\int_0^Rr^4dr
=\boxed{-\frac{3GM^2}{5R}}.
$$

Hydrostatic equilibrium gives its central pressure

$$
\boxed{P_c=\frac{3GM^2}{8\pi R^4}}.
$$

Thus, relative to the same uniform-density estimate for Earth,

$$
\frac{P_{c,p}}{P_{c,\oplus}}
=\left(\frac{M_p}{M_\oplus}\right)^2
\left(\frac{R_p}{R_\oplus}\right)^{-4}.
$$

Using $(M,R)_{\rm N}\simeq(17.1,3.88)$ gives $P_{c,\rm N}/P_{c,\oplus}\simeq1.3$, while $(M,R)_{\rm J}\simeq(318,11.2)$ gives $P_{c,\rm J}/P_{c,\oplus}\simeq6.4$. Real central pressures differ because all three planets are compressible and compositionally stratified.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For uniform density, [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) releases binding energy $|U|=3GM^2/(5R)$. If mass and luminosity are constant and stellar heating is negligible at 90 au, the contraction age is

$$
\boxed{t_{\rm KH}\simeq\frac{3GM^2}{5RL}}.
$$

Energy conservation, $L=-dU/dt$, gives

$$
\boxed{\dot R=-\frac{5LR^2}{3GM^2}}.
$$

The [virial theorem](../../../classical-mechanics.md#virial-theorem) places roughly half of the released gravitational energy into internal heat. Including that effect gives $t_{\rm KH}\simeq3GM^2/(10RL)$ and $\dot R\simeq-10LR^2/(3GM^2)$.

## 4

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In an infrared-opaque [single-layer greenhouse model](../../../exoplanet.md#single-layer-greenhouse-model), the atmospheric layer obeys $2\sigma T_a^4=\sigma T_s^4$. The outgoing planetary flux is $\sigma T_a^4$, while the globally averaged absorbed stellar flux is $(1-A_B)L/(16\pi a^2)$. [Radiative equilibrium](../../../thermodynamics.md#radiative-equilibrium) therefore gives

$$
\frac{\sigma T_s^4}{2}
=\frac{(1-A_B)At^{-\beta}}{16\pi a^2}.
$$

Hence the orbit at which the prescribed surface temperature can be maintained is

$$
\boxed{
a(t)=\left[\frac{(1-A_B)A}
{8\pi\sigma T_s^4}\right]^{1/2}t^{-\beta/2}}.
$$

This assumes uniform redistribution, constant [Bond albedo](../../../exoplanet.md#bond-albedo), unit longwave emissivity, a transparent atmosphere to starlight, and no internal heat. Without the greenhouse layer, replace $8\pi$ by $16\pi$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In an isothermal hydrostatic atmosphere, pressure falls as $P(z)=P_0e^{-z/H}$. If a water-band line core becomes optically thick at pressure $P_{\rm line}$ and an opaque cloud fixes the nearby continuum at $P_{\rm cl}$, the [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) feature spans

$$
\frac{\Delta z}{H}=\log\frac{P_{\rm cl}}{P_{\rm line}}.
$$

A two-scale-height feature therefore requires

$$
\boxed{P_{\rm cl}=e^2P_{\rm line}}.
$$

Taking a representative near-infrared water-band pressure $P_{\rm line}\sim1\,{\rm mbar}$ gives $P_{\rm cl}\sim7\,{\rm mbar}$, so the appropriate estimate is an [exoplanet cloud deck](../../../exoplanet.md#exoplanet-cloud-deck) top near $10\,{\rm mbar}$. The numerical value scales directly with the assumed line-core pressure.

Other explanations include a high [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight), subsolar water abundance, a colder terminator, [atmospheric haze](../../../exoplanet.md#haze), patchy two-limb clouds, stellar contamination, or instrumental systematics. Optical scattering slopes, broader [James Webb Space Telescope](../../../exoplanet.md#james-webb-space-telescope) molecular coverage, repeated transits, secondary-eclipse spectra, phase curves, and precise mass and radius measurements can distinguish these possibilities.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Hydrostatic balance and the ideal-gas [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient) imply

$$
\left|\frac{dT}{dz}\right|_{\rm ad}
=\frac{g}{c_p}.
$$

The radiative region is stable while $K\rho/T^3<g/c_p$. Equality at the [radiative-convective boundary](../../../exoplanet.md#radiative-convective-boundary), together with $\rho=\mu P/(\mathcal RT)$, gives

$$
\boxed{P_{\rm rc}
=\frac{g\mathcal R}{K\mu c_p}T_{\rm rc}^4
=\frac{g\nabla_{\rm ad}}{K}T_{\rm rc}^4}.
$$

For radiative diffusion carrying intrinsic flux $F_{\rm int}=\sigma T_{\rm int}^4$, $K=3\kappa F_{\rm int}/(16\sigma)$, so

$$
\boxed{P_{\rm rc}
=\frac{16g\nabla_{\rm ad}}{3\kappa}
\left(\frac{T_{\rm rc}}{T_{\rm int}}\right)^4}.
$$

For an irradiated hot Jupiter with $g\simeq10\,{\rm m\,s^{-2}}$, $\nabla_{\rm ad}\simeq2/7$, $\kappa\simeq10^{-2}\,{\rm m^2\,kg^{-1}}$, $T_{\rm rc}\simeq1500\,{\rm K}$, and $T_{\rm int}\simeq150$--$200\,{\rm K}$, this gives roughly $P_{\rm rc}\sim50$--$200\,{\rm bar}$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Approximate the atmosphere above $R_p$ as isothermal with constant gravity and [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) $H$, so

$$
P(z)=P_0e^{-z/H}.
$$

Vertical transport over one scale height has [eddy mixing time](../../../exoplanet.md#eddy-mixing-time)

$$
\tau_{\rm mix}\simeq\frac{H^2}{K_{zz}}.
$$

The [chemical quench level](../../../exoplanet.md#chemical-quench-level) satisfies $\tau_{\rm chem}(z_q)=\tau_{\rm mix}$. Since $\tau_{\rm chem}=\eta z$,

$$
z_q=\frac{H^2}{\eta K_{zz}},
\qquad
\boxed{P_q=P_0\exp\left(-\frac{H}{\eta K_{zz}}\right)}.
$$

Above this level, mixing is faster than reaction and freezes the deeper abundance of A. Larger $K_{zz}$ moves the quench level deeper and raises $P_q$. Important examples are [carbon monoxide–methane quenching](../../../exoplanet.md#carbon-monoxide-methane-quenching) and [nitrogen–ammonia quenching](../../../exoplanet.md#nitrogen-ammonia-quenching); phosphine destruction is another tracer of vertical quenching.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

[Exoplanet clouds](../../../exoplanet.md#exoplanet-cloud) and [atmospheric haze](../../../exoplanet.md#haze) add scattering and absorption opacity to an [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum). A high opaque deck truncates the slant path and mutes molecular bands, while small aerosol particles can produce a blue scattering slope; patchiness creates mixtures of clear and cloudy limbs. In an [exoplanet emission spectrum](../../../exoplanet.md#exoplanet-emission-spectrum), aerosols move the photosphere to lower pressure, weaken or reshape molecular features, alter the [geometric albedo](../../../exoplanet.md#geometric-albedo), and can heat or cool layers depending on their shortwave and longwave absorption.

Observed aspects of [exoplanet atmospheric dynamics](../../../exoplanet.md#exoplanet-atmospheric-dynamics) include eastward equatorial [atmospheric superrotation](../../../exoplanet.md#atmospheric-super-rotation) inferred from shifted thermal hot spots, day-night heat transport measured by phase-curve amplitude, and high-altitude winds measured from Doppler shifts of resolved spectral lines. Time-variable phase curves and eclipse maps also reveal changing cloud patterns and storms.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
