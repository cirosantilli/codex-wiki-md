# Paper 65

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper65.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper65.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
  - [vii](#4/vii)
    - [Solution](#4/vii/solution)
  - [viii](#4/viii)
    - [Solution](#4/viii/solution)

## 1

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $G$ be the remaining gas [mass](../../../classical-mechanics.md#mass), $S$ the formed stellar [mass](../../../classical-mechanics.md#mass), and $G_0$ the initial gas [mass](../../../classical-mechanics.md#mass); initially $S=0$ and the [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) is zero. Take the [stellar yield](../../../galaxy.md#stellar-yield) $y$ and the [mass-loading factor](../../../galaxy.md#mass-loading-factor) $\nu$ to be constant, with homogeneous mixing and no [galactic gas inflow](../../../galaxy.md#galactic-gas-inflow). With the specified zero bulk return, [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
dG=-(1+\nu)\,dS,\qquad G=G_0-(1+\nu)S.
$$

New metals add $y\,dS$, while [star formation](../../../stellar-astrophysics.md#star-formation) and the [galactic outflow](../../../galaxy.md#galactic-outflow) remove metals at the existing [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) $Z$. Thus

$$
d(GZ)=y\,dS-Z(1+\nu)\,dS,
\qquad G\,dZ=y\,dS=-\frac{y}{1+\nu}\,dG.
$$

The [leaky-box model of galactic chemical evolution](../../../galaxy.md#leaky-box-model-of-galactic-chemical-evolution) therefore gives

$$
Z=\frac{y}{1+\nu}\ln\frac{G_0}{G}.
$$

For the usual [gas fraction of a galaxy](../../../galaxy.md#gas-fraction-of-a-galaxy), $\mu=G/(G+S)$, the denominator is the baryonic [mass](../../../classical-mechanics.md#mass) still in the system, which decreases under the [galactic outflow](../../../galaxy.md#galactic-outflow). Since $G_0=G+(1+\nu)S$, we have $G_0/G=1+(1+\nu)(1-\mu)/\mu$. **In the remaining-mass convention,**

$$
\boxed{Z(\mu)=\frac{y}{1+\nu}\ln\left[\frac{1+\nu(1-\mu)}{\mu}\right].}
$$

If instead $\mu$ denotes $G/G_0$ relative to the fixed initial reservoir, the same calculation gives $\boxed{Z=y\ln(1/\mu)/(1+\nu)}$. Stating the denominator matters: these two [gas fraction of a galaxy](../../../galaxy.md#gas-fraction-of-a-galaxy) conventions coincide for the [closed-box model of galactic chemical evolution](../../../galaxy.md#closed-box-model-of-galactic-chemical-evolution), recovered at $\nu=0$, but differ when gas escapes. Neglecting bulk return while retaining a nonzero [stellar yield](../../../galaxy.md#stellar-yield) is the intended trace-metal approximation.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A star inherits the [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) at its birth. Set $y_e=y/(1+\nu)$; the preceding calculation gives $G(Z)=G_0e^{-Z/y_e}$ and $dS/dZ=G(Z)/y$. If the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) is fixed, let $\kappa$ be the number of the counted stars per unit formed stellar [mass](../../../classical-mechanics.md#mass); this includes any restriction to surviving long-lived tracers. The [metallicity distribution in a leaky box](../../../galaxy.md#metallicity-distribution-in-a-leaky-box) is therefore

$$
\boxed{\frac{dN}{dZ}=\frac{\kappa G_0}{y}\exp\left[-\frac{(1+\nu)Z}{y}\right].}
$$

The total eventual formed stellar [mass](../../../classical-mechanics.md#mass) is $G_0/(1+\nu)$, so $N_\infty=\kappa G_0/(1+\nu)$ and the equivalent normalized [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function) is

$$
\boxed{\frac1{N_\infty}\frac{dN}{dZ}=\frac{1+\nu}{y}e^{-(1+\nu)Z/y}.}
$$

If $N(Z)$ means a cumulative count rather than a count per [stellar metallicity](../../../galaxy.md#stellar-metallicity) interval, [integration](../../../calculus.md#integral) yields

$$
\boxed{N(<Z)=N_\infty\left[1-e^{-(1+\nu)Z/y}\right].}
$$

At a finite observation time these expressions end at the current [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) $Z_f$ and the normalized distribution divides by $1-e^{-Z_f/y_e}$. A distribution per logarithmic [stellar metallicity](../../../galaxy.md#stellar-metallicity) instead multiplies $dN/dZ$ by $(\ln10)Z$; it is not the same shape as the distribution per linear [stellar metallicity](../../../galaxy.md#stellar-metallicity).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

All gas being used or expelled means $G\to0$, so $Z\to\infty$ in the formal [leaky-box model of galactic chemical evolution](../../../galaxy.md#leaky-box-model-of-galactic-chemical-evolution) and the final stellar [mass](../../../classical-mechanics.md#mass) is $S_\infty=G_0/(1+\nu)$. Weight the [stellar metallicity](../../../galaxy.md#stellar-metallicity) by formed stellar [mass](../../../classical-mechanics.md#mass), using $dS/dZ=(G_0/y)e^{-Z/y_e}$:

$$
\langle Z\rangle_*=
\frac{\int_0^\infty Z\,(G_0/y)e^{-Z/y_e}\,dZ}{G_0/(1+\nu)}
=\frac{(G_0/y)y_e^2}{G_0/(1+\nu)}.
$$

Here $\int_0^\infty u e^{-u}du=1$, by [integration by parts](../../../calculus.md#integration-by-parts). **The final mass-weighted mean is**

$$
\boxed{\langle Z\rangle_*=\frac{y}{1+\nu}.}
$$

As a metal-budget check, newly produced metal [mass](../../../classical-mechanics.md#mass) is $yS_\infty$; stars retain $\int Z\,dS=yG_0/(1+\nu)^2$, while the [galactic outflow](../../../galaxy.md#galactic-outflow) carries $\nu\int Z\,dS$. Their sum is exactly $yS_\infty$. An observed luminosity-weighted [stellar metallicity](../../../galaxy.md#stellar-metallicity) need not equal this mass-weighted mean.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Assume the [stellar yield](../../../galaxy.md#stellar-yield) is common to the compared [stellar populations](../../../stellar-astrophysics.md#stellar-population) and compare their mass-weighted [stellar metallicities](../../../galaxy.md#stellar-metallicity). Inverting the [metallicity distribution in a leaky box](../../../galaxy.md#metallicity-distribution-in-a-leaky-box) result gives

$$
\boxed{\nu=\frac{y}{\langle Z\rangle_*}-1.}
$$

For example, with $y=Z_\odot$, a solar-metallicity massive [elliptical galaxy](../../../galaxy.md#elliptical-galaxy) requires $\nu\simeq0$, whereas $\langle Z\rangle_*<0.01Z_\odot$ in a [dwarf galaxy](../../../galaxy.md#dwarf-galaxy) requires $\nu>99$. A supersolar [stellar metallicity](../../../galaxy.md#stellar-metallicity) requires a correspondingly supersolar [stellar yield](../../../galaxy.md#stellar-yield): outflow alone cannot raise $\langle Z\rangle_*$ above $y$. If $y=2Z_\odot$, a massive [elliptical galaxy](../../../galaxy.md#elliptical-galaxy) with $\langle Z\rangle_*$ between $Z_\odot$ and $2Z_\odot$ has $0\le\nu\le1$, while the same low-metallicity [dwarf galaxy](../../../galaxy.md#dwarf-galaxy) needs $\nu>199$.

**For a yield of order solar, the required mass loading runs from order zero or unity in massive spheroids to order one hundred or more in faint dwarfs.** Without a specified [stellar yield](../../../galaxy.md#stellar-yield), the robust comparison is

$$
\frac{1+\nu_{\rm dwarf}}{1+\nu_{\rm giant}}
=\frac{\langle Z\rangle_{*,\rm giant}}{\langle Z\rangle_{*,\rm dwarf}}
\gtrsim100.
$$

This explains the sense of the [galaxy mass--metallicity relation](../../../galaxy.md#galaxy-mass-metallicity-relation); [galactic gas inflow](../../../galaxy.md#galactic-gas-inflow), incomplete depletion, and changes in the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) can also change observed [stellar metallicity](../../../galaxy.md#stellar-metallicity).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The [escape-speed scaling of wind mass loading](../../../galaxy.md#escape-speed-scaling-of-wind-mass-loading) makes the proposed trend dynamically plausible: the shallower [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) of a [dwarf galaxy](../../../galaxy.md#dwarf-galaxy) lets [stellar feedback](../../../galaxy.md#stellar-feedback) expel more gas per unit stellar [mass](../../../classical-mechanics.md#mass). If coupled feedback supplies specific [energy](../../../classical-mechanics.md#energy) $e_*$, escape requires $\nu v_{\rm esc}^2/2\lesssim e_*$; fixed coupling suggests $\nu\propto v_{\rm esc}^{-2}$ for an [energy-driven outflow](../../../astrophysics.md#energy-driven-outflow). Fixed specific momentum $p_*$ instead gives $\nu v_{\rm esc}\lesssim p_*$, or $\nu\propto v_{\rm esc}^{-1}$ for a [momentum-driven outflow](../../../astrophysics.md#momentum-driven-outflow).

Since [escape velocity](../../../classical-mechanics.md#escape-velocity) has $v_{\rm esc}^2\sim GM/R$, galaxies whose characteristic radius grows more slowly than their gravitating [mass](../../../classical-mechanics.md#mass) have increasing binding energy per unit [mass](../../../classical-mechanics.md#mass) with increasing [mass](../../../classical-mechanics.md#mass). For $R\propto M^a$ with $a<1$, the [energy-driven outflow](../../../astrophysics.md#energy-driven-outflow) estimate gives $\nu\propto M^{a-1}$. Equivalently, greater [velocity dispersion](../../../galaxy.md#velocity-dispersion) in massive spheroids implies greater escape energy and more effective retention of metals.

For scale, one [core-collapse supernova](../../../stellar-astrophysics.md#core-collapse-supernova) of $10^{51}\,\mathrm{erg}$ per $100M_\odot$ formed supplies about $5\times10^{15}\,\mathrm{cm^2\,s^{-2}}$ before coupling losses. At ten percent coupling the energetic upper estimate $2e_*/v_{\rm esc}^2$ is about $110$ for $v_{\rm esc}=30\,\mathrm{km\,s^{-1}}$, but about $0.4$ for $500\,\mathrm{km\,s^{-1}}$. **Efficient loss from shallow potentials and retention in deep potentials can span the required range.** These are illustrative energetics rather than a unique prediction: cooling, entrainment, fallback and the actual [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) determine the escaping [mass-loading factor](../../../galaxy.md#mass-loading-factor).

## 2

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use a steady, isotropic, self-gravitating [dark matter halo](../../../large-scale-structure-of-the-universe.md#dark-matter-halo), with $V$ its constant one-dimensional [velocity dispersion](../../../galaxy.md#velocity-dispersion). The [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation) and spherical [mass conservation](../../../continuum-mechanics.md#mass-conservation) read

$$
V^2\frac{d\rho}{dr}=-\rho\frac{GM(r)}{r^2},\qquad
\frac{dM}{dr}=4\pi r^2\rho.
$$

For the scale-free outer region, put $\rho=A r^{-p}$. Its enclosed [mass](../../../classical-mechanics.md#mass) scales as $r^{3-p}$, so $GM(r)/r$ is constant only if $p=2$; the [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation) then gives $2V^2=GM(r)/r=4\pi GA$. Thus the [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere) has

$$
\boxed{\rho(r)=\frac{V^2}{2\pi Gr^2},\qquad M(<r)=\frac{2V^2r}{G}.}
$$

Its [circular speed](../../../galaxy.md#circular-speed) is $v_c=\sqrt2V$. If a speed denoted $V$ were instead the [circular speed](../../../galaxy.md#circular-speed), the coefficient would be $V^2/(4\pi G)$, but the printed variable is a [velocity dispersion](../../../galaxy.md#velocity-dispersion).

The assumptions matter. A constant [velocity dispersion](../../../galaxy.md#velocity-dispersion) and spherical shape alone do not specify a unique central [mass density](../../../fluid-mechanics.md#density) or orbital distribution. Even with isotropy, the [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation) integrates to $\rho=\rho_0\exp[-(\Phi-\Phi_0)/V^2]$, and the self-gravitating [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) gives

$$
\frac1{r^2}\frac{d}{dr}\left(r^2\frac{d\ln\rho}{dr}\right)
=-\frac{4\pi G}{V^2}\rho.
$$

There are finite-central-density isothermal solutions as well as the singular one; the $r^{-2}$ expression is the intended outer scale-free halo approximation. A finite halo must also end or steepen at large radius, since the untruncated [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere) has infinite total [mass](../../../classical-mechanics.md#mass).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $m_\chi$ be the [dark matter](../../../cosmology.md#dark-matter) particle [mass](../../../classical-mechanics.md#mass), so its number density is $n_\chi=\rho/m_\chi$. Interpret $\epsilon$ as total emitted power per particle, and assume isotropic optically thin [dark-matter decay radiation](../../../cosmology.md#dark-matter-decay-radiation); volume emissivity is $j_d=\epsilon\rho/m_\chi$. At projected radius $R$, a line-of-sight coordinate $z$ has $r^2=R^2+z^2$. Writing $A=V^2/(2\pi G)$, the [surface brightness](../../../astrophysics.md#surface-brightness) is

$$
I_d(R)=\frac1{4\pi}\int_{-\infty}^\infty j_d\,dz
=\frac{\epsilon A}{4\pi m_\chi}
\int_{-\infty}^\infty\frac{dz}{R^2+z^2}
=\frac{\epsilon A}{4m_\chi R}.
$$

Here $z=R\tan\theta$ turns the [integral](../../../calculus.md#integral) into $\pi/R$. **For the isothermal outer halo,**

$$
\boxed{I_d(R)=\frac{\epsilon V^2}{8\pi Gm_\chi R}\propto R^{-1}.}
$$

If emissivity was defined per unit solid angle, the factor $1/(4\pi)$ is already included in $\epsilon$; this only changes the normalization. The radial law holds between any core and outer truncation. For example, a phenomenological cored profile $\rho=A/(r^2+r_c^2)$ gives $I_d=\epsilon A/[4m_\chi\sqrt{R^2+r_c^2}]$: finite central [surface brightness](../../../astrophysics.md#surface-brightness), but the same $R^{-1}$ outer law. This cored interpolation is not being asserted to be the exact isotropic constant-dispersion equilibrium.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

A two-body annihilation requires two nearby particles, so the [dark-matter annihilation radiation](../../../cosmology.md#dark-matter-annihilation-radiation) has emissivity proportional to the square of the [mass density](../../../fluid-mechanics.md#density). With a spatially constant rate coefficient, write

$$
j_a=C_a\rho^2,\qquad
C_a=\frac{E_a\langle\sigma v_{\rm rel}\rangle}{2m_\chi^2}
$$

for identical self-conjugate particles, where $E_a$ is the radiated [energy](../../../classical-mechanics.md#energy) per annihilation; the factor one-half counts unordered pairs. Particle and antiparticle populations instead require their respective number densities, without that identical-pair factor. For the [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere), the [surface brightness](../../../astrophysics.md#surface-brightness) becomes

$$
I_a(R)=\frac{C_aA^2}{4\pi}\int_{-\infty}^\infty
\frac{dz}{(R^2+z^2)^2}.
$$

The substitution $z=R\tan\theta$ gives $R^{-3}\int_{-\pi/2}^{\pi/2}\cos^2\theta\,d\theta=\pi/(2R^3)$. Hence **annihilation gives the steeper projected profile**

$$
\boxed{I_a(R)=\frac{C_aA^2}{8R^3}
=\frac{C_aV^4}{32\pi^2G^2R^3}\propto R^{-3}.}
$$

For the illustrative cored profile used above, $I_a=C_aA^2/[8(R^2+r_c^2)^{3/2}]$. These expressions assume a smooth [dark matter halo](../../../large-scale-structure-of-the-universe.md#dark-matter-halo), negligible absorption and constant $C_a$; unresolved density clumps or a velocity-dependent annihilation coefficient change the projected shape. The [projection of a spherical power-law emissivity](../../../astrophysics.md#projection-of-a-spherical-power-law-emissivity) summarizes why three-dimensional powers $r^{-2}$ and $r^{-4}$ produce $R^{-1}$ and $R^{-3}$.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Measure the logarithmic [surface brightness](../../../astrophysics.md#surface-brightness) slope in resolved radial annuli after accounting for instrumental blurring and foreground emission. Between a halo core and its outer boundary, [dark-matter decay radiation](../../../cosmology.md#dark-matter-decay-radiation) predicts $d\ln I/d\ln R=-1$, whereas [dark-matter annihilation radiation](../../../cosmology.md#dark-matter-annihilation-radiation) predicts $-3$; doubling radius therefore reduces the respective [surface brightness](../../../astrophysics.md#surface-brightness) by factors $2$ and $8$. These are quantitative templates to compare with independently mapped stellar and gaseous components.

An [exponential galactic disk](../../../galaxy.md#exponential-galactic-disk) has $I_*(R)\propto e^{-R/R_d}$, so $d\ln I_*/d\ln R=-R/R_d$ and $I_*(2R)/I_*(R)=e^{-R/R_d}$. At $R=5R_d$ the latter is about $0.0067$, much faster decline than either halo template, and the projected emission should also be flattened along the [galactic disk](../../../galaxy.md#galactic-disk). A [galactic bulge](../../../galaxy.md#galactic-bulge) described by a [Sérsic profile](../../../astrophysics.md#sersic-profile) has $d\ln I_*/d\ln R=-(b_n/n)(R/R_e)^{1/n}$; for $n=4$ and $b_4\simeq7.67$, this is about $-3.4$ at $10R_e$ and continues to steepen, whereas a pure halo power law keeps a fixed slope.

For a [stellar halo](../../../galaxy.md#stellar-halo) with outer luminosity density proportional to $r^{-p_*}$, the [projection of a spherical power-law emissivity](../../../astrophysics.md#projection-of-a-spherical-power-law-emissivity) gives $I_*\propto R^{1-p_*}$. Illustratively, $p_*=3$--$4$ gives projected slopes $-2$--$-3$: then $I_d/I_*\propto R^{p_*-2}$ rises strongly outward, but annihilation can resemble the steeper stellar template. Gas-related gamma emission must be compared with observed gas columns and the [cosmic ray](../../../galaxy.md#cosmic-ray) distribution; it is not always proportional to optical light.

**A shallow, extended, approximately spherical $R^{-1}$ component is particularly distinctive; an $R^{-3}$ component needs additional evidence.** Fit the stellar, gas and halo templates together over a broad radial range, including morphology and emission spectra. A measured slope alone cannot uniquely identify [dark matter](../../../cosmology.md#dark-matter), since stellar or gas profiles can coincide with a halo slope over a limited interval.

## 3

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write $x=m/M_\odot$ and absorb units into the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) normalization, $dN=A x^{-3}dx$. The specified [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation) is $L(x)=L_\odot x^3$, normalized to the Sun. Therefore the total stellar [mass](../../../classical-mechanics.md#mass) and [luminosity](../../../astrophysics.md#luminosity) are

$$
\frac{M_*}{M_\odot}=A\int_{0.1}^1x^{-2}dx=9A,
\qquad
\frac{L_*}{L_\odot}=A\int_{0.1}^1x^0dx=0.9A.
$$

The unknown normalization cancels. **The mass-to-light ratio is**

$$
\boxed{\Upsilon_* = 10\,\frac{M_\odot}{L_\odot}.}
$$

Low-mass [main sequence](../../../stellar-astrophysics.md#main-sequence) stars dominate the stellar [mass](../../../classical-mechanics.md#mass), while equal intervals of $x$ contribute equal [luminosity](../../../astrophysics.md#luminosity) under these particular exponents. More generally the [mass-to-light ratio of a power-law stellar population](../../../galaxy.md#mass-to-light-ratio-of-a-power-law-stellar-population) with these exponents on $a<x<b$ is $(M_\odot/L_\odot)/(ab)$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The result is in the broad range expected for an old, relatively faint [stellar population](../../../stellar-astrophysics.md#stellar-population), but is high compared with many observed stellar [mass-to-light ratios](../../../galaxy.md#mass-to-light-ratio) of a few solar units in optical bands. The comparison must specify the band and whether the measured [mass](../../../classical-mechanics.md#mass) includes [dark matter](../../../cosmology.md#dark-matter): for example, [early-type galaxy dynamical measurements](https://arxiv.org/abs/astro-ph/0505042) find an $I$-band normalization near $3.8$ solar units at [velocity dispersion](../../../galaxy.md#velocity-dispersion) $200\,\mathrm{km\,s^{-1}}$, including a contribution from [dark matter](../../../cosmology.md#dark-matter). That is an illustrative observational comparison, not a direct equality with a bolometric stellar calculation.

For an old [stellar population](../../../stellar-astrophysics.md#stellar-population), an upper surviving [main sequence](../../../stellar-astrophysics.md#main-sequence) mass near $M_\odot$ is reasonable because more massive stars have shorter lifetimes; low-mass [main sequence](../../../stellar-astrophysics.md#main-sequence) stars also contain much of the surviving stellar [mass](../../../classical-mechanics.md#mass). However, [red giants](../../../stellar-astrophysics.md#red-giant) and other evolved stars can contribute a large fraction of the light despite their small numbers, so omitting them generally makes this calculated [mass-to-light ratio](../../../galaxy.md#mass-to-light-ratio) too large. Omitting [stellar remnants](../../../stellar-astrophysics.md#stellar-remnant) has the opposite effect on the inferred [mass](../../../classical-mechanics.md#mass), and a single cubic [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation) is only approximate across the stated range. Finally, a single $m^{-3}$ [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) down to $0.1M_\odot$ is steeper and more low-mass-heavy than commonly adopted distributions, which flatten at low [mass](../../../classical-mechanics.md#mass). **Ten solar units is a useful toy-model estimate, not a precision stellar-population prediction.**

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Let the extrapolated lower limit be $a=m_{\min}/M_\odot$ and keep the upper surviving limit at $x=1$. If the same cubic [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation) is formally continued, the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) gives

$$
\frac{M_*}{M_\odot}=A\left(\frac1a-1\right),\qquad
\frac{L_*}{L_\odot}=A(1-a),\qquad
\frac{\Upsilon_*}{M_\odot/L_\odot}=\frac1a.
$$

Matching $1000$ therefore requires **a planetary-scale cutoff**

$$
\boxed{m_{\min}=10^{-3}M_\odot\simeq1M_{\rm Jupiter}.}
$$

The [mass](../../../classical-mechanics.md#mass) per logarithmic interval is proportional to $m^{-1}$ for this [initial mass function](../../../stellar-astrophysics.md#initial-mass-function), so most of the added [mass](../../../classical-mechanics.md#mass) is near the cutoff. Substellar objects do not actually obey the unevolved cubic [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation): they cool, and their [luminosity](../../../astrophysics.md#luminosity) depends strongly on age. If they are approximated as entirely dark while only the original $0.1$--$1M_\odot$ stars supply light, then $\Upsilon_*=(1/a-1)/0.9$ instead, giving $a=1/901\simeq1.11\times10^{-3}$. Both conventions lead to the same order-of-magnitude conclusion; the exact $10^{-3}$ result uses the question's formal power-law extrapolation.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Objects near the derived cutoff are too faint for their absence in ordinary star counts alone to exclude a massive [dark matter halo](../../../large-scale-structure-of-the-universe.md#dark-matter-halo). The decisive test is [gravitational microlensing](../../../general-relativity.md#gravitational-microlensing): compact objects passing in front of background stars produce transient magnification even if they emit no detectable light. For a lens at distance $D_l$ and a source at $D_s$, the physical [Einstein radius](../../../general-relativity.md#einstein-radius) and event timescale are

$$
R_E=\sqrt{\frac{4Gm}{c^2}\frac{D_l(D_s-D_l)}{D_s}},\qquad
 t_E=R_E/v_\perp\propto\sqrt m.
$$

For $D_l=10\,\mathrm{kpc}$, $D_s=50\,\mathrm{kpc}$ and $v_\perp=200\,\mathrm{km\,s^{-1}}$, a $10^{-3}M_\odot$ lens gives $t_E\simeq2.2$ days, within the regime tested by suitably sampled [gravitational microlensing](../../../general-relativity.md#gravitational-microlensing) surveys. The [microlensing optical depth](../../../general-relativity.md#microlensing-optical-depth) is

$$
\tau=\frac{4\pi G}{c^2}\int_0^{D_s}\rho_l(D_l)\frac{D_l(D_s-D_l)}{D_s}\,dD_l,
$$

so at fixed compact-object [mass density](../../../fluid-mechanics.md#density) it is independent of the individual lens [mass](../../../classical-mechanics.md#mass): reducing individual [mass](../../../classical-mechanics.md#mass) changes the event durations rather than hiding the total lensing probability.

[EROS observations of the Magellanic Clouds](https://arxiv.org/abs/astro-ph/0607207) found far fewer candidate events than a halo dominated by compact objects would predict and excluded such objects as the principal Galactic halo component over $6\times10^{-8}<m/M_\odot<15$, under their tested halo models. Their often-quoted eight-percent bound is specifically near $0.4M_\odot$, not a uniform bound at every lens [mass](../../../classical-mechanics.md#mass). **A halo dominated by the approximately Jupiter-mass objects needed here is incompatible with those microlensing constraints.** Deep optical and [infrared](../../../optics.md#infrared) counts also restrict a large population of luminous low-mass stars and [brown dwarfs](../../../stellar-astrophysics.md#brown-dwarf), while the [cosmic baryon fraction](../../../cosmology.md#cosmic-baryon-fraction) provides a separate constraint on explaining all cosmological [dark matter](../../../cosmology.md#dark-matter) with baryonic objects.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

First specify the dynamical estimate: assume an initially isolated virialized system, stars of different [masses](../../../classical-mechanics.md#mass) well mixed with the same velocity distribution, and ejecta escaping rapidly compared with a [stellar crossing time](../../../galaxy.md#stellar-crossing-time), without imparting kicks to surviving stars. If $f$ is the retained stellar [mass](../../../classical-mechanics.md#mass) fraction, the original [virial theorem](../../../classical-mechanics.md#virial-theorem) gives $2T+W=0$, where $T$ is [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and $W<0$ is [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy). Immediately after loss, positions and velocities are unchanged, so

$$
T'=fT,\qquad W'=f^2W,\qquad
E'=fT+f^2W=|W|f\left(\frac12-f\right).
$$

Thus [impulsive disruption by stellar mass loss](../../../galaxy.md#impulsive-disruption-by-stellar-mass-loss) makes the energy of the whole remaining system nonnegative when at least half the initial [mass](../../../classical-mechanics.md#mass) is removed.

For the power-law [initial mass function](../../../stellar-astrophysics.md#initial-mass-function), the fraction removed is a mass fraction, not a number fraction:

$$
F(\alpha)=\frac{\int_{10}^{100}x^{1-\alpha}dx}{\int_{0.1}^{100}x^{1-\alpha}dx}
=\frac{100^{2-\alpha}-10^{2-\alpha}}{100^{2-\alpha}-0.1^{2-\alpha}}
\quad(\alpha\ne2),\qquad F(2)=\frac{\ln10}{\ln1000}=\frac13.
$$

For integer slopes, $F(0)\simeq0.990$, $F(1)\simeq0.901$, $F(2)=0.333$, and $F(3)\simeq0.009$. Interpolating between $\alpha=1$ and $2$ puts the threshold around $1.7$--$1.8$. Solving $F=1/2$ more accurately gives

$$
2\,10^{2-\alpha}=100^{2-\alpha}+0.1^{2-\alpha},\qquad
\boxed{\alpha_{\rm crit}\simeq1.7910.}
$$

The rearranged equation has a spurious root at $\alpha=2$ introduced when the vanishing denominator was cleared; the logarithmic limit $F(2)=1/3$ excludes it. Increasing $\alpha$ shifts the mass distribution towards lower [masses](../../../classical-mechanics.md#mass), so **the top-heavy side, $\alpha<\alpha_{\rm crit}$, has nonnegative remnant energy in the impulsive model**; equality is marginal. One can see strict monotonicity from the [covariance](../../../variance.md#covariance) obtained by differentiating $F$: $F'=-\operatorname{Cov}(\mathbf1_{x>10},\ln x)<0$ under the normalized mass-weighted distribution.

The [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) alone does not guarantee complete disruption. If losses occur slowly, the [adiabatic mass-loss expansion law](../../../galaxy.md#adiabatic-mass-loss-expansion-law) gives expansion rather than the instantaneous half-mass threshold, and positive total energy can still leave a bound core after selective escape. The stated value is therefore the conventional global impulsive estimate, with no external confining [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential).

## 4

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A typical [globular cluster](../../../galaxy.md#globular-cluster) has undergone appreciable [two-body relaxation](../../../galaxy.md#two-body-relaxation), since its [stellar relaxation time](../../../galaxy.md#stellar-relaxation-time) is $t_{\rm rel}\sim0.1(N/\ln N)t_{\rm cross}$: for $N\sim10^5$ and [stellar crossing time](../../../galaxy.md#stellar-crossing-time) $t_{\rm cross}\sim10^6\,\mathrm{yr}$ this is about $10^9\,\mathrm{yr}$, shorter than its age, allowing a relatively relaxed, tidally limited structure. A [galaxy](../../../galaxy.md) with $N\sim10^{11}$ and $t_{\rm cross}\sim10^8\,\mathrm{yr}$ instead has $t_{\rm rel}\sim4\times10^{16}\,\mathrm{yr}$ and behaves as a [collisionless stellar system](../../../galaxy.md#collisionless-stellar-system), retaining differences from formation, [galaxy mergers](../../../galaxy.md#galaxy-merger), and [star formation](../../../stellar-astrophysics.md#star-formation). **Relaxation erases more memory in clusters than in galaxies**, although real [globular clusters](../../../galaxy.md#globular-cluster) also differ in concentration and evolutionary state, so structural similarity is approximate.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

At small separations the extended [dark-matter haloes](../../../large-scale-structure-of-the-universe.md#dark-matter-halo) overlap, and [Chandrasekhar dynamical friction](../../../galaxy.md#chandrasekhar-dynamical-friction) transfers orbital [energy](../../../classical-mechanics.md#energy) to gravitational wakes while tidal interactions also redistribute orbital [energy](../../../classical-mechanics.md#energy). A characteristic decay time scales as $t_{\rm df}\sim v r^2/(Gm\ln\Lambda)$, so sufficiently massive close pairs evolve rapidly towards a [galaxy merger](../../../galaxy.md#galaxy-merger) and spend relatively little time at small separation. **Short residence time depletes the close-pair population**; the quoted separation scale is characteristic of the population, not a universal exclusion radius.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The [stellar population](../../../stellar-astrophysics.md#stellar-population) has appreciable random [velocity dispersion](../../../galaxy.md#velocity-dispersion), and its declining radial density creates an outward stress gradient that supplies some support against gravity; cold gas has much less random-motion support and follows nearly the local [circular speed](../../../galaxy.md#circular-speed). Neglecting velocity-ellipsoid tilt, the radial [Jeans equation](../../../galaxy.md#jeans-equation) gives $v_c^2-\overline v_\phi^2=\sigma_R^2[-d\ln(n_*\sigma_R^2)/d\ln R-1+\sigma_\phi^2/\sigma_R^2]$, generally positive for the stellar disk. **The slower mean stellar rotation is [asymmetric drift](../../../galaxy.md#stellar-asymmetric-drift).**

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

A nonrotating [elliptical galaxy](../../../galaxy.md#elliptical-galaxy) need not have an isotropic [velocity ellipsoid](../../../galaxy.md#velocity-ellipsoid): unequal random-motion stresses in different directions can support an oblate or triaxial shape without substantial mean rotation. The [tensor virial theorem](../../../galaxy.md#tensor-virial-theorem), $2T_{ij}+W_{ij}=0$ for a stationary isolated system with appropriate boundary terms, balances this directional kinetic stress against the directional gravitational stress. **Anisotropic random motions can supply the flattening**, whereas an isotropic nonrotating equilibrium has much stronger restrictions on its shape.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

A [flux-limited galaxy selection](../../../astrophysics.md#flux-limited-galaxy-selection) samples a much larger volume for bright [galaxies](../../../galaxy.md): in the nearby Euclidean limit $d_{\max}\propto\sqrt L$, hence $V_{\max}\propto L^{3/2}$, so very numerous faint [dwarf galaxies](../../../galaxy.md#dwarf-galaxy) are usually detectable only nearby. With a [Schechter function](../../../galaxy.md#schechter-function) $\phi(L)\propto L^{\alpha_S}e^{-L/L_*}$, detected counts per logarithmic [luminosity](../../../astrophysics.md#luminosity) interval scale as $L^{\alpha_S+5/2}e^{-L/L_*}$ and, for $\alpha_S\sim-1$ to $-1.3$, peak near $L\sim(1.2\text{--}1.5)L_*$ rather than at the numerous faint end. **The competition between increasing survey volume and the bright-end cutoff concentrates detected luminosities near $L_*$**, with the precise width depending on the selection and survey depth.

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

The differential gravitational field of the [Milky Way](../../../galaxy.md#milky-way) removes loosely bound outer material by [tidal stripping](../../../galaxy.md#tidal-stripping), giving [globular clusters](../../../galaxy.md#globular-cluster) and satellite [dwarf galaxies](../../../galaxy.md#dwarf-galaxy) a characteristic [tidal radius](../../../galaxy.md#tidal-radius). For a low-mass satellite of [mass](../../../classical-mechanics.md#mass) $m$ on a circular orbit of radius $R$ in a spherical host, the [Jacobi tidal radius](../../../galaxy.md#jacobi-tidal-radius) is $r_t\simeq R\{m/[(3-d\ln M_h/d\ln R)M_h(<R)]\}^{1/3}$; eccentric orbits often make the strongest restriction near pericentre. **Tidal limitation explains the sharp outer falloff**, although escaping stars can form extended [tidal tails](../../../galaxy.md#tidal-tail), so a fitted luminosity cutoff is not an exact boundary of all associated material.

<h3 id="4/vii">vii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#4/vii)

Massive stars rapidly return oxygen, magnesium, neon and other [alpha elements](../../../galaxy.md#alpha-element) through [core-collapse supernovae](../../../stellar-astrophysics.md#core-collapse-supernova), whereas [Type Ia supernovae](../../../stellar-astrophysics.md#type-ia-supernova) supply a substantial delayed iron contribution. If the [galactic bulge](../../../galaxy.md#galactic-bulge) and [stellar halo](../../../galaxy.md#stellar-halo) formed much of their stellar [mass](../../../classical-mechanics.md#mass) rapidly, their stars locked in enhanced alpha-element to iron ratios before much [delayed iron enrichment](../../../galaxy.md#delayed-iron-enrichment), while prolonged [star formation](../../../stellar-astrophysics.md#star-formation) in the local [galactic disk](../../../galaxy.md#galactic-disk) included more iron-rich gas. **The abundance contrast chiefly records different enrichment timescales**, with the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) and gas exchange also affecting the ratios.

<h3 id="4/viii">viii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#4/viii)

In a compact [starburst galaxy](../../../galaxy.md#starburst-galaxy), [stellar feedback](../../../galaxy.md#stellar-feedback) can approach the [radiation-pressure limit of a dusty starburst](../../../galaxy.md#radiation-pressure-limit-of-a-dusty-starburst), $\kappa F/c\sim g$, so stronger luminosity drives a [galactic outflow](../../../galaxy.md#galactic-outflow) rather than allowing indefinitely increasing [star formation rate](../../../galaxy.md#star-formation-rate). [Optically thick starburst-disk calculations](https://arxiv.org/abs/astro-ph/0503027) give a characteristic infrared [flux](../../../physics.md#flux) near $10^{13}L_\odot\,\mathrm{kpc}^{-2}$; with $L_{\rm IR}\sim10^{10}L_\odot[\dot M_*/(M_\odot\,\mathrm{yr}^{-1})]$ and an emitting area of order $1\,\mathrm{kpc}^2$, this corresponds to $\dot M_*\sim10^3M_\odot\,\mathrm{yr}^{-1}$ and would consume $10^{10}M_\odot$ of gas in only $10^7\,\mathrm{yr}$. **Feedback and a finite fuel supply produce a characteristic upper scale for compact bursts**, rather than a universal ceiling on the total rate independent of star-forming area and gas supply.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
