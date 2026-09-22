# Paper 315

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_315.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_315.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
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
  - [f](#4/f)
    - [Solution](#4/f/solution)
  - [g](#4/g)
    - [Solution](#4/g/solution)
  - [h](#4/h)
    - [Solution](#4/h/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [j](#4/j)
    - [Solution](#4/j/solution)

## 1

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Take $P_0>0$, real $\alpha$, and the real branch $T\ge T_0$, with physical [temperature](../../../thermodynamics.md#temperature) $T>0$. In [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) the [pressure](../../../thermodynamics.md#pressure) decreases with height $z$:

$$
\frac{dP}{dz}=-\rho g<0.
$$

Thus an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) means $dT/dz>0$, equivalently $dT/dP<0$. For $\alpha\ne0$, the [logarithm](../../../calculus.md#logarithm) of the given relation yields

$$
T(P)=T_0+\frac{\log^2(P/P_0)}{\alpha^2},\qquad
\frac{\log(P/P_0)}{\alpha}=\sqrt{T-T_0}\ge0.
$$

The sign restriction must be retained after squaring. In particular, the inverted branch has $0<P\le P_0$, whereas the non-inverted branch has $P\ge P_0$. By [differentiation](../../../calculus.md#differentiation), on the interior of either branch,

$$
\frac{dT}{d\log P}=\frac{2\log(P/P_0)}{\alpha^2}
=\frac{2\sqrt{T-T_0}}{\alpha},\qquad
\frac{dT}{dz}=-\frac{2\rho g\sqrt{T-T_0}}{\alpha P}.
$$

Consequently,

$$
\boxed{\alpha<0:\ \text{thermal inversion};\qquad
\alpha>0:\ \text{temperature decreases outward}.}
$$

At $T=T_0$, the inverse [temperature gradient](../../../thermodynamics.md#temperature-gradient) vanishes at the branch endpoint, rather than producing a finite isothermal interval. If $\alpha=0$, the relation becomes $P=P_0$ independently of $T$; it is not a nontrivial vertical [atmospheric pressure-temperature profile](../../../exoplanet.md#atmospheric-pressure-temperature-profile) under [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium). These distinctions prevent the two sides of the squared parabola from being interpreted as one permissible atmosphere.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Assume a homogeneous [ideal gas](../../../thermodynamics.md#ideal-gas), constant [specific-heat ratio](../../../thermodynamics.md#heat-capacity-ratio) $\gamma>1$, and an upward displacement that is an [adiabatic process](../../../thermodynamics.md#adiabatic-process) and maintains pressure balance with its surroundings. If the ambient [temperature](../../../thermodynamics.md#temperature) falls faster with decreasing [pressure](../../../thermodynamics.md#pressure) than the parcel's [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient), the parcel becomes hotter and less dense than its surroundings; [buoyancy](../../../fluid-mechanics.md#buoyancy) amplifies the displacement. This is the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion):

$$
\nabla\equiv\frac{d\log T}{d\log P}>\nabla_{\rm ad}
=\frac{\gamma-1}{\gamma}\equiv A.
$$

The [square-root exponential atmospheric profile](../../../exoplanet.md#square-root-exponential-atmospheric-profile) has

$$
\boxed{\nabla=\frac{2\sqrt{T-T_0}}{\alpha T};\qquad
\text{instability requires }\frac{2\sqrt{T-T_0}}{\alpha T}>A.}
$$

An [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) with $\alpha<0$ has $\nabla<0$ and is stable to these ordinary adiabatic displacements. For $\alpha>0$, put $s=\sqrt{T-T_0}$. The condition becomes the [quadratic inequality](../../../polynomial.md#quadratic-inequality)

$$
A\alpha s^2-2s+A\alpha T_0<0,
$$

intersected with $s\ge0$ and $T_0+s^2>0$. In the usual case $T_0>0$, the maximum gradient occurs at $s=\sqrt{T_0}$, namely $T=2T_0$, and is $1/(\alpha\sqrt{T_0})$. Hence a convectively unstable interval exists precisely when

$$
\boxed{A\alpha\sqrt{T_0}<1,\qquad
s_-<\sqrt{T-T_0}<s_+,\quad
s_\pm=\frac{1\pm\sqrt{1-(A\alpha)^2T_0}}{A\alpha}.}
$$

Equality in the existence condition gives a single neutrally stable point. A molecular-hydrogen-dominated [hot Jupiter](../../../exoplanet.md#hot-jupiter) with rotational modes active but vibrational excitation and dissociation negligible has approximately $\gamma=7/5$, so $A=2/7$. The existence condition is then $\alpha\sqrt{T_0}<7/2$. For $T_0\le0$ the general inequality above remains valid, but its roots must be intersected with the positive-[temperature](../../../thermodynamics.md#temperature) domain; the positive-$T_0$ maximum formula must not be reused. Composition gradients require the [Ledoux criterion](../../../stellar-structure.md#ledoux-criterion), and dissociation or variable heat capacities change $A$. Sustained [convection](../../../fluid-mechanics.md#convection) normally adjusts a superadiabatic profile toward an [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Use the usual atmospheric plotting convention: [temperature](../../../thermodynamics.md#temperature) on the horizontal axis, logarithmic [pressure](../../../thermodynamics.md#pressure) increasing downward. To illustrate a physically plausible local range for a [hot Jupiter](../../../exoplanet.md#hot-jupiter), set $T_0=1000\,\mathrm K$ and $|\alpha|=0.05\,\mathrm K^{-1/2}$. The sign is not fixed by the fact that the planet is a [hot Jupiter](../../../exoplanet.md#hot-jupiter); irradiation and [opacity](../../../stellar-structure.md#opacity) determine whether an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) is present.

The original sketch shows both admissible branches of the [square-root exponential atmospheric profile](../../../exoplanet.md#square-root-exponential-atmospheric-profile), with separate assumed normalizations $P_0=0.01\,\mathrm{bar}$ for the outward-cooling example and $P_0=1\,\mathrm{bar}$ for the inverted example. Each extends from $1000$ to $2600\,\mathrm K$ and has $|\log(P/P_0)|\le2$. For $\alpha>0$, increasing depth increases both [pressure](../../../thermodynamics.md#pressure) and [temperature](../../../thermodynamics.md#temperature), so the curve bends rightward downward. For $\alpha<0$, moving upward lowers [pressure](../../../thermodynamics.md#pressure) and raises [temperature](../../../thermodynamics.md#temperature), so the curve bends rightward upward. Each branch meets $T_0$ with $dT/d\log P=0$; it must not be continued through that endpoint onto the other branch.

<a id="1/a/iii/image-illustrative-branches-of-an-atmospheric-pressure-temperature-profile"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315-pt-profile.png)

**[Figure 1](#1/a/iii/image-illustrative-branches-of-an-atmospheric-pressure-temperature-profile). Illustrative branches of an atmospheric pressure-temperature profile**.

For the outward-cooling example, $\alpha\sqrt{T_0}=1.58<3.5$, so a section of the imposed profile is unstable for a homogeneous diatomic [ideal gas](../../../thermodynamics.md#ideal-gas). It should be interpreted as an illustrative retrieved radiative profile that would be modified by [convection](../../../fluid-mechanics.md#convection) if realised, rather than a self-consistent deep convective atmosphere. The inverted branch is stable under the same assumptions.

**The sketch must show only the sign-allowed pressure branch; either an inverted or an outward-cooling local profile is possible.**

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

The functional form is not specific to [exoplanets](../../../exoplanet.md). With positive [pressure](../../../thermodynamics.md#pressure) normalization and physical [temperature](../../../thermodynamics.md#temperature), a [square-root exponential atmospheric profile](../../../exoplanet.md#square-root-exponential-atmospheric-profile) can approximate a monotone interval of the [terrestrial atmosphere](../../../planetary-science.md#terrestrial-atmosphere). An outward-cooling interval, such as part of the [troposphere](../../../planetary-science.md#troposphere) or [mesosphere](../../../planetary-science.md#mesosphere), requires $\alpha>0$. An upward-warming interval, such as part of the [stratosphere](../../../planetary-science.md#stratosphere) heated by ultraviolet absorption or the [thermosphere](../../../planetary-science.md#thermosphere) heated by high-energy radiation, requires $\alpha<0$.

The local [atmospheric lapse rate](../../../exoplanet.md#lapse-rate-atmosphere) follows from the [ideal gas](../../../thermodynamics.md#ideal-gas) relation $P=\rho k_BT/(\mu m_H)$ and [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium):

$$
\Gamma\equiv-\frac{dT}{dz}
=\frac{\mu m_Hg}{k_B}\frac{2\sqrt{T-T_0}}{\alpha T}
=\frac{\mu m_Hg}{k_B}\nabla.
$$

For dry terrestrial air, approximately $\gamma=1.4$ and $\mu\simeq29$ give the dry-adiabatic lapse rate $g/c_p\simeq9.8\,\mathrm{K\,km^{-1}}$. The familiar mean tropospheric value near $6.5\,\mathrm{K\,km^{-1}}$ is less steep; a local fit must satisfy $\nabla\lesssim2/7$ to be dry-convectively stable. Moist [convection](../../../fluid-mechanics.md#convection) needs the moist parcel thermodynamics instead, and the [terrestrial atmosphere](../../../planetary-science.md#terrestrial-atmosphere) is not uniformly dry or chemically homogeneous at all heights.

The squared-[logarithm](../../../calculus.md#logarithm) shape cannot reproduce an exactly constant nonzero lapse rate over an arbitrary thick region, all the alternating atmospheric layers, or a finite exactly isothermal region. It is a local parametrization with a fixed sign of the [temperature gradient](../../../thermodynamics.md#temperature-gradient); it has no terrestrial universality.

$$
\boxed{\alpha>0\text{ can fit an outward-cooling interval};\quad
\alpha<0\text{ can fit an upward-warming interval}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Take $R_p$ to be the [radius](../../../topology.md#radius) of an opaque planetary disc and $H$ the geometric thickness of the model atmosphere, not necessarily one [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height). Assume a uniform stellar [specific intensity](../../../astrophysics.md#specific-intensity), a fully projected non-grazing transit, negligible planetary emission in the measured band, and no scattering or refraction returning light to the beam. The cylindrical approximation assigns the same slant [optical depth](../../../astrophysics.md#optical-depth) $\tau_\lambda$ to every ray through the annulus.

The opaque disc blocks area $\pi R_p^2$. The annulus has projected area $\pi[(R_p+H)^2-R_p^2]$, and the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) transmits fraction $e^{-\tau_\lambda}$ through it. Its blocked fraction is therefore $1-e^{-\tau_\lambda}$. Dividing the missing light by the unobscured stellar-disc light gives the [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum)

$$
\boxed{D_\lambda=\frac{R_p^2+[(R_p+H)^2-R_p^2](1-e^{-\tau_\lambda})}{R_s^2}.}
$$

For $H\ll R_p$, the [annulus model for transmission spectroscopy](../../../exoplanet.md#annulus-model-for-transmission-spectroscopy) becomes

$$
D_\lambda\simeq\left(\frac{R_p}{R_s}\right)^2
+\frac{2R_pH}{R_s^2}(1-e^{-\tau_\lambda}).
$$

The [optically thin](../../../astrophysics.md#optically-thin-medium) excess is $2R_pH\tau_\lambda/R_s^2$; the [optically thick](../../../astrophysics.md#optically-thick-medium) limit is the area ratio $(R_p+H)^2/R_s^2$ before the thin-annulus approximation. For a realistic atmosphere, the slant [optical depth](../../../astrophysics.md#optical-depth) varies with the ray's impact parameter $b$, giving instead

$$
D_\lambda=\frac{R_p^2+2\int_{R_p}^{R_p+H}b[1-e^{-\tau_\lambda(b)}]\,db}{R_s^2}.
$$

[Limb darkening](../../../astrophysics.md#limb-darkening) replaces the simple area weighting by the local stellar [specific intensity](../../../astrophysics.md#specific-intensity). The constant-depth model is therefore an explicit geometric approximation, not the slant-depth law of a spherical hydrostatic atmosphere.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A natural interpretation of the short-wavelength peak is reflected starlight, while the longer-wavelength peak is planetary [thermal radiation](../../../electromagnetism.md#thermal-radiation). A reflected spectrum approximately follows the stellar spectrum multiplied by the wavelength-dependent [geometric albedo](../../../exoplanet.md#geometric-albedo); thermal [radiative flux](../../../astrophysics.md#radiative-flux) approximately follows the planet's [Planck function](../../../astrophysics.md#planck-function), modulated by molecular [opacity](../../../stellar-structure.md#opacity). Thus two peaks need not represent two planetary surface [temperatures](../../../thermodynamics.md#temperature).

For a quantitative estimate assume both are broad $F_\lambda$ peaks, reflection has a slowly varying [geometric albedo](../../../exoplanet.md#geometric-albedo), and star and planet have approximately [blackbody](../../../astrophysics.md#blackbody) spectral envelopes. [Wien's displacement law](../../../astrophysics.md#wien-s-displacement-law) then gives

$$
T_*\simeq\frac{2898\,\mu\mathrm m\,\mathrm K}{0.7\,\mu\mathrm m}
\simeq4140\,\mathrm K,\qquad
T_p\simeq\frac{2898\,\mu\mathrm m\,\mathrm K}{1.5\,\mu\mathrm m}
\simeq1930\,\mathrm K.
$$

The stellar estimate is compatible at order of magnitude with an old, relatively small main-sequence star; equal age does not mean equal [temperature](../../../thermodynamics.md#temperature) to the [Sun](../../../stellar-astrophysics.md#sun). Assume the far-infrared signal is thermal and sufficiently long-wavelength that the [Rayleigh-Jeans law](../../../astrophysics.md#rayleigh-jeans-law) applies to both bodies. The [planet-star radius estimate in the Rayleigh-Jeans limit](../../../exoplanet.md#planet-star-radius-estimate-in-the-rayleigh-jeans-limit) gives

$$
\frac{F_p}{F_*}=\left(\frac{R_p}{R_*}\right)^2\frac{T_p}{T_*},\qquad
R_p=\frac{R_\odot}{2}\sqrt{10^{-3}\frac{4140}{1930}},
$$

and therefore

$$
\boxed{R_p\simeq0.023\,R_\odot\simeq1.6\times10^7\,\mathrm m
\simeq2.5\,R_\oplus.}
$$

This is a small volatile-rich-planet-sized estimate, not a Jupiter-sized one. It is conditional: peaks caused by molecular windows, strongly chromatic reflection, or a spectrum expressed as $F_\nu$ rather than $F_\lambda$ do not support those two Wien estimates. Without $T_p/T_*$, the far-infrared ratio only fixes $R_p^2T_p/T_*$.

For a close-in hot planet around a small star, transit-based atmospheric observations are the natural route if the orbital geometry allows them. [Exoplanet transmission spectra](../../../exoplanet.md#exoplanet-transmission-spectrum) gain from the small stellar [radius](../../../topology.md#radius), with a limb signal scaling as $2R_pH/R_*^2$; they probe composition at the [day-night terminator](../../../exoplanet.md#day-night-terminator). The stated $10^{-3}$ thermal contrast also makes [exoplanet secondary eclipse](../../../exoplanet.md#exoplanet-secondary-eclipse) measurements a particularly useful route to the dayside [exoplanet emission spectrum](../../../exoplanet.md#exoplanet-emission-spectrum). Resolving such a close-in small planet by [exoplanet direct imaging](../../../exoplanet.md#exoplanet-direct-imaging) is much harder. **Transit and secondary-eclipse spectroscopy are favoured for a transiting close-in interpretation; the supplied spectrum alone does not determine the orbital geometry or a unique best technique.**

## 2

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

In the collisionless [exosphere](../../../exoplanet.md#exosphere), an atom escapes if its outward trajectory has positive total mechanical [energy](../../../classical-mechanics.md#energy). Neglect tides and stellar forces and use [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) at exobase [radius](../../../topology.md#radius) $r_e$:

$$
\frac12mv^2>\frac{GM_pm}{r_e},\qquad
v>v_{\rm esc}=\sqrt{\frac{2GM_p}{r_e}}.
$$

With thermal speed $v_{\rm th}=\sqrt{2k_BT_e/m}$, the [Jeans escape parameter](../../../exoplanet.md#jeans-escape-parameter) is

$$
\lambda_e=\frac{v_{\rm esc}^2}{v_{\rm th}^2}
=\frac{GM_pm}{k_BT_er_e}.
$$

A thermal distribution always has an escaping tail; [Jeans escape](../../../exoplanet.md#jeans-escape) is exponentially suppressed for $\lambda_e\gg1$, with [Jeans escape flux](../../../exoplanet.md#jeans-escape-flux) proportional to $(1+\lambda_e)e^{-\lambda_e}$. Efficient escape requires $\lambda_e$ of order a few or smaller, with an order-unity energetic estimate $k_BT_e\sim GM_pm/r_e$.

Assume a [Neptune](../../../planetary-science.md#neptune)-like [mass](../../../classical-mechanics.md#mass) and [radius](../../../topology.md#radius), $r_e\simeq R_p$, and atomic [hydrogen](../../../chemistry.md#hydrogen). Using the supplied rounded constants gives

$$
g\simeq17.5\,\mathrm{m\,s^{-2}},\qquad
v_{\rm esc}\simeq2.65\times10^4\,\mathrm{m\,s^{-1}},\qquad
\frac{GM_pm_H}{k_BR_p}\simeq3.5\times10^4\,\mathrm K.
$$

Hence

$$
\boxed{T_e\sim10^4\text{--}4\times10^4\,\mathrm K
\text{ for a few-to-unity Jeans parameter at }r_e\simeq R_p.}
$$

Using the mean kinetic energy $3k_BT/2$ instead gives an order-unity coefficient and $T\simeq2.3\times10^4\,\mathrm K$. An expanded [exobase](../../../exoplanet.md#exobase) has weaker binding and lowers the estimate by $R_p/r_e$. A comet-like tail can also be shaped by [radiation pressure](../../../thermodynamics.md#radiation-pressure) and stellar-wind interactions; it does not by itself measure $T_e$ or prove that a hydrostatic Jeans model is valid. At $\lambda_e\sim1$, $H/r_e\sim1$ and [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) fails as a global description: substantial mass loss must usually be treated as [hydrodynamic atmospheric escape](../../../exoplanet.md#hydrodynamic-escape).

The [exobase](../../../exoplanet.md#exobase) is defined by [mean free path](../../../thermodynamics.md#mean-free-path) $\ell\sim H$, not by a universal [pressure](../../../thermodynamics.md#pressure). For a neutral hydrostatic gas with [collision cross-section](../../../classical-mechanics.md#collision-cross-section) $\sigma_c$,

$$
\ell\sim\frac1{n_e\sigma_c},\quad H\simeq\frac{k_BT_e}{m_Hg},\quad
\boxed{P_e=n_ek_BT_e\sim\frac{m_Hg}{\sigma_c}.}
$$

For example, explicitly assuming $\sigma_c\sim10^{-19}\text{--}10^{-20}\,\mathrm{m^2}$ gives $P_e\sim2\times10^{-7}\text{--}2\times10^{-6}\,\mathrm{Pa}$, or $2\times10^{-12}\text{--}2\times10^{-11}\,\mathrm{bar}$. These are representative extremely dilute neutral-exobase pressures, with orders of magnitude varying with composition, cross-sections and expansion. The supplied constants contain no collision information, so they cannot uniquely determine an exobase [pressure](../../../thermodynamics.md#pressure); ionization or a non-hydrostatic density profile changes this estimate.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Three physically distinct mechanisms are as follows.

- [Jeans escape](../../../exoplanet.md#jeans-escape): particles in the high-speed tail of the local thermal distribution escape collisionlessly from the [exobase](../../../exoplanet.md#exobase). The [Jeans escape parameter](../../../exoplanet.md#jeans-escape-parameter) determines the exponentially small tail fraction when binding is strong. Light atoms escape more readily at fixed [temperature](../../../thermodynamics.md#temperature).
- [Hydrodynamic atmospheric escape](../../../exoplanet.md#hydrodynamic-escape): stellar extreme-ultraviolet or X-ray heating raises atmospheric [pressure](../../../thermodynamics.md#pressure) and drives an expanding bulk wind. A sufficiently strong wind entrains heavier species. An approximate [energy-limited atmospheric escape](../../../exoplanet.md#energy-limited-atmospheric-escape) estimate equates useful absorbed power to gravitational work, $\dot M\sim\eta\pi R_{\rm abs}^2F_{\rm XUV}R_p/(GM_p)$, but radiative losses, recombination and tides can invalidate this scaling.
- [Nonthermal atmospheric escape](../../../exoplanet.md#nonthermal-atmospheric-escape): photodissociation or charge exchange produces fast atoms, while stellar-wind ion pickup and sputtering transfer energy to ions or neutrals independently of the local gas [temperature](../../../thermodynamics.md#temperature). Magnetic geometry and stellar activity affect these channels. [Radiation pressure](../../../thermodynamics.md#radiation-pressure) can accelerate escaping neutral [hydrogen](../../../chemistry.md#hydrogen) into a tail.

**Thermal-tail escape, a bulk hydrodynamic wind, and nonthermal particle energization are three distinct channels; a detected tail need not distinguish them alone.** [Jeans escape](../../../exoplanet.md#jeans-escape) and [hydrodynamic atmospheric escape](../../../exoplanet.md#hydrodynamic-escape) are both thermal mechanisms in the broad sense, but have different distribution functions and dynamical assumptions.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let the closed atmospheric parcel exchange [heat](../../../thermodynamics.md#heat) and volume work with reservoirs at fixed [temperature](../../../thermodynamics.md#temperature) $T$ and [pressure](../../../thermodynamics.md#pressure) $P$, while reactions rearrange its conserved elemental inventory. For a reversible differential between equilibrium states, the [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics), with chemical work included, is

$$
dU=T\,dS-P\,dV+\sum_i\mu_i\,dN_i.
$$

The [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy) $G=U+PV-TS$ therefore obeys

$$
dG=-S\,dT+V\,dP+\sum_i\mu_i\,dN_i.
$$

The [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) supplies this differential but does not alone choose the direction of a reaction. The [Second law of thermodynamics](../../../thermodynamics.md#second-law-of-thermodynamics) does: for the parcel plus its reservoirs, at fixed $T,P$ and with no non-volume work,

$$
dS_{\rm total}=dS-\frac{dU+P\,dV}{T}=-\frac{dG}{T}\ge0.
$$

Thus spontaneous reactions decrease [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy), and stable [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium) is its constrained minimum. For an allowed reaction of extent $d\xi$, let $dN_i=\nu_i\,d\xi$, with positive [stoichiometric vector](../../../mathematical-biology.md#stoichiometric-vector) entries for products and negative entries for reactants. At an interior minimum,

$$
\boxed{\left(\frac{\partial G}{\partial\xi}\right)_{T,P}
=\sum_i\nu_i\mu_i=0,\qquad
\delta^2G\ge0\text{ on allowed variations}.}
$$

The condition must hold for every independent allowed reaction, with fixed total atoms of each element and any relevant charge constraint. At a boundary with absent species, only feasible one-sided variations are permitted. These are the hypotheses of [constrained Gibbs minimization for chemical equilibrium](../../../thermodynamics.md#constrained-gibbs-minimization-for-chemical-equilibrium).

For an [ideal gas](../../../thermodynamics.md#ideal-gas) mixture, $\mu_i=\mu_i^\circ(T)+\mathcal RT\log(x_iP/P^\circ)$, where $x_i$ is the [volume mixing ratio](../../../mathematical-biology.md#volume-mixing-ratio) and $\mathcal R$ the molar gas constant. Therefore

$$
\prod_i\left(\frac{x_iP}{P^\circ}\right)^{\nu_i}
=\exp\left(-\frac{\Delta_rG^\circ}{\mathcal RT}\right)\equiv K_p(T).
$$

This is a dimensionless activity-based equilibrium constant, not a bare product of dimensional pressures.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Assume a single-phase [ideal gas](../../../thermodynamics.md#ideal-gas) mixture in a closed parcel, with common [temperature](../../../thermodynamics.md#temperature) $T$, total [pressure](../../../thermodynamics.md#pressure) $P$, and molar species amounts $N_i$. Define $N=\sum_iN_i$ and [volume mixing ratios](../../../mathematical-biology.md#volume-mixing-ratio) $x_i=N_i/N$, so $\sum_i x_i=1$. Ideal mixing makes partial [pressure](../../../thermodynamics.md#pressure) $P_i=x_iP$.

For a pure ideal species, $d\mu_i=-\bar S_i\,dT+\bar V_i\,dP_i$, with molar volume $\bar V_i=\mathcal RT/P_i$. At fixed [temperature](../../../thermodynamics.md#temperature), integration from standard [pressure](../../../thermodynamics.md#pressure) $P^\circ$ gives

$$
\mu_i(T,P_i)=\mu_i^\circ(T)+\mathcal RT\log(P_i/P^\circ).
$$

The same logarithmic composition term follows from the ideal mixing [entropy](../../../thermodynamics.md#entropy) $\Delta S_{\rm mix}=-\mathcal R\sum_iN_i\log x_i$. Extensivity gives $G=\sum_iN_i\mu_i$. Hence the [Gibbs free energy of an ideal-gas mixture](../../../thermodynamics.md#gibbs-free-energy-of-an-ideal-gas-mixture) is

$$
\boxed{G(T,P,\{N_i\})=N\sum_i x_i\mu_i^\circ(T)
+N\mathcal RT\left[\log(P/P^\circ)+\sum_i x_i\log x_i\right].}
$$

Equivalently, write each standard chemical term as $\mu_i^\circ=h_i^\circ-Ts_i^\circ$, using molar [enthalpy](../../../thermodynamics.md#enthalpy) and [entropy](../../../thermodynamics.md#entropy). For zero abundance the limit $x\log x\to0$ defines the extensive expression continuously.

The fractions alone do not specify the extensive [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy): the total amount $N$ or an equivalent elemental inventory must also be fixed. Moreover, in a chemically closed reacting system $N$ need not remain constant; for example, hydrogenation of [carbon monoxide](../../../chemistry.md#carbon-monoxide) changes the total molecular count while conserving atoms. Minimization is therefore over species amounts subject to elemental constraints, rather than over fractions with an artificially fixed molecular count. Nonideal gases require activities or fugacities; condensates contribute separate phase terms.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Assume an isothermal terminator, constant gravity and [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight), and use the stated nightside [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) as the terminator value. [Hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives $P(z)=P_{\rm ref}e^{-(z-z_{\rm ref})/H}$. A band radius three [atmospheric scale heights](../../../exoplanet.md#atmospheric-scale-height) above a measured continuum at $0.1\,\mathrm{bar}$ therefore corresponds to

$$
\boxed{P_{\rm band}=0.1e^{-3}\,\mathrm{bar}
\simeq5.0\times10^{-3}\,\mathrm{bar}.}
$$

This is the band's characteristic [pressure](../../../thermodynamics.md#pressure), not automatically the top of an [exoplanet cloud deck](../../../exoplanet.md#exoplanet-cloud-deck). The distinction matters because an opaque cloud generally raises the continuum and removes the lower part of a molecular feature; it does not cap the height of a strong molecular line above the cloud.

If the quoted $0.1\,\mathrm{bar}$ is the actual observed continuum and the cloud dominates its [opacity](../../../stellar-structure.md#opacity), the consistent estimate is instead

$$
\boxed{P_c\simeq P_{\rm cont}\simeq0.1\,\mathrm{bar},\qquad
P_{\rm band}\simeq5\,\mathrm{mbar}.}
$$

If $0.1\,\mathrm{bar}$ refers to a clear-atmosphere reference continuum, an additional clear band height is necessary. Let that height be $NH$. A cloud at height $z_c$ leaves a residual feature of $3H$ when $NH-z_c=3H$. Thus the [cloud pressure degeneracy of a transmission feature](../../../exoplanet.md#cloud-pressure-degeneracy-of-a-transmission-feature) gives

$$
P_c=0.1e^{-(N-3)}\,\mathrm{bar}.
$$

For example, **a $5\,\mathrm{mbar}$ cloud estimate requires the extra assumption that the clear band spans six scale heights**, so the cloud raises the continuum by three. Identifying the cloud with the level three scale heights above the original continuum gives the same numerical value, but is not justified by the observed band height alone. Without a clear-band [opacity](../../../stellar-structure.md#opacity) or equivalent reference radius, there is no unique cloud-top [pressure](../../../thermodynamics.md#pressure). A strong dayside emission feature also does not supply that missing terminator information.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

The two measurements sample different atmospheric regions and different [radiative transfer](../../../astrophysics.md#radiative-transfer) geometries. An [exoplanet emission spectrum](../../../exoplanet.md#exoplanet-emission-spectrum) probes the dayside; an [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) probes the morning and evening limbs of the [day-night terminator](../../../exoplanet.md#day-night-terminator). Several alternatives to an [exoplanet cloud deck](../../../exoplanet.md#exoplanet-cloud-deck) can therefore suppress the transmission feature.

- A cooler terminator has a smaller [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) $H=k_BT/(\mu m_Hg)$, so the same change in slant [optical depth](../../../astrophysics.md#optical-depth) produces a smaller transit-area change. A larger [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) has the same geometric effect. The assumption that the nightside [temperature](../../../thermodynamics.md#temperature) sets both limbs may itself be wrong.
- Genuine chemical heterogeneity can reduce terminator [carbon monoxide](../../../chemistry.md#carbon-monoxide). At lower [temperature](../../../thermodynamics.md#temperature), [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium) can favour [methane](../../../chemistry.md#methane) through $\mathrm{CO}+3\mathrm{H}_2\rightleftharpoons\mathrm{CH}_4+\mathrm{H}_2\mathrm O$, if local reaction times are sufficiently short. [Atmospheric photochemistry](../../../exoplanet.md#atmospheric-photochemistry), elemental abundance differences, and [horizontal chemical quenching](../../../exoplanet.md#horizontal-chemical-quenching) can modify this simple picture.
- The feature depends on a band-to-continuum [opacity](../../../stellar-structure.md#opacity) ratio, not abundance alone. A continuum enhanced by other gas absorption or a partly covered heterogeneous limb can mute the feature; the [two-limb transmission spectrum](../../../exoplanet.md#two-limb-transmission-spectrum) illustrates this averaging. Stellar surface heterogeneity and measurement systematics can also bias an inferred feature amplitude.
- A strong CO emission feature can be amplified by an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology), because the line forms in hotter gas than the continuum. It is consequently not an unambiguous abundance measurement without a simultaneous [atmospheric pressure-temperature profile](../../../exoplanet.md#atmospheric-pressure-temperature-profile) fit.

**Temperature, mean molecular weight, limb chemistry, continuum opacity and the dayside temperature gradient are alternatives or degeneracies to test.** In particular, the three-scale-height amplitude alone cannot establish different CO abundances between the hemispheres.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

[Convection](../../../fluid-mechanics.md#convection) mixes material vertically where the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion) or [Ledoux criterion](../../../stellar-structure.md#ledoux-criterion) allows it. Its chemical effect is controlled by competition between transport and reaction, rather than by a direct alteration of the equilibrium constant. Parametrize vertical transport by a [vertical eddy diffusion coefficient](../../../exoplanet.md#vertical-eddy-diffusion-coefficient) $K_{zz}$; the [eddy mixing time](../../../exoplanet.md#eddy-mixing-time) over a scale height is

$$
\tau_{\rm mix}\sim\frac{H^2}{K_{zz}}.
$$

Let $\tau_{\rm chem}$ be the [chemical relaxation time](../../../thermodynamics.md#chemical-relaxation-time) of the relevant interconversion. If reactions are faster, the gas follows local [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium). If transport becomes faster, composition can be carried upward faster than it re-equilibrates. A [chemical quench level](../../../exoplanet.md#chemical-quench-level) is approximately where the two times match:

$$
\boxed{\tau_{\rm mix}\sim\tau_{\rm chem}\text{ at quenching};\qquad
\tau_{\rm mix}\ll\tau_{\rm chem}\text{ favours transported abundances}.}
$$

For example, hot deep gas may contain abundant [carbon monoxide](../../../chemistry.md#carbon-monoxide). Strong mixing can maintain it in cooler layers where equilibrium would favour [methane](../../../chemistry.md#methane); this is [carbon monoxide–methane quenching](../../../exoplanet.md#carbon-monoxide-methane-quenching). Similar reasoning applies to [nitrogen–ammonia quenching](../../../exoplanet.md#nitrogen-ammonia-quenching). The cooler nightside commonly has slower reaction rates and can preserve such quenched composition more readily, whereas sufficiently rapid dayside chemistry can restore local equilibrium. Neither statement is universal without the actual reaction network and [temperature](../../../thermodynamics.md#temperature).

The observable atmosphere of a strongly irradiated [hot Jupiter](../../../exoplanet.md#hot-jupiter) may be radiative and stable even if the deeper interior is convective. Deep [convection](../../../fluid-mechanics.md#convection) influences the photosphere only if some mixing crosses the intervening radiative region, for example through overshoot or other dynamical transport. Moreover, transport from day to night is horizontal circulation, not vertical [convection](../../../fluid-mechanics.md#convection); its relevant competition is [atmospheric advection time](../../../exoplanet.md#atmospheric-advection-time) versus [chemical relaxation time](../../../thermodynamics.md#chemical-relaxation-time), giving [horizontal chemical quenching](../../../exoplanet.md#horizontal-chemical-quenching). **Convection can affect either hemisphere indirectly through connected vertical transport; strong deep convection alone does not guarantee a quenched observable composition.**

## 3

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

For a quasi-static self-gravitating object of fixed [mass](../../../classical-mechanics.md#mass), negligible surface [pressure](../../../thermodynamics.md#pressure), and no accretion, nuclear source or additional deep heating, [conservation of energy](../../../physics.md#conservation-of-energy) gives the [intrinsic planetary luminosity](../../../stellar-astrophysics.md#intrinsic-planetary-luminosity)

$$
L_{\rm int}=-\frac{d}{dt}(U+\Omega),\qquad
\Omega=-\int_0^M\frac{Gm}{r(m)}\,dm.
$$

Here $U$ is internal [energy](../../../classical-mechanics.md#energy), and $\Omega$ is negative gravitational [potential energy](../../../classical-mechanics.md#potential-energy). Gravitational contraction makes $\Omega$ more negative and releases power $L_{\rm grav}\equiv-d\Omega/dt>0$. Some of that release raises the internal [energy](../../../classical-mechanics.md#energy); it cannot all be radiated while the object maintains [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium).

To quantify the split assume thermal gas pressure with constant [specific-heat ratio](../../../thermodynamics.md#heat-capacity-ratio) $\gamma>4/3$ and negligible rotation or magnetic support. This excludes the dynamically unstable gas-supported regime. The [stellar virial theorem](../../../stellar-structure.md#stellar-virial-theorem) gives

$$
\Omega+3\int P\,dV=0,\qquad
U=\frac1{\gamma-1}\int P\,dV=-\frac{\Omega}{3(\gamma-1)}.
$$

It follows that

$$
\boxed{L_{\rm int}=\frac{3\gamma-4}{3(\gamma-1)}L_{\rm grav}.}
$$

For a monatomic [ideal gas](../../../thermodynamics.md#ideal-gas), $\gamma=5/3$, so $L_{\rm int}=L_{\rm grav}/2$: half the released gravitational [energy](../../../classical-mechanics.md#energy) heats the gas and half escapes. If the density profile remains homologous, write $\Omega=-qGM^2/R$, with $q>0$ a fixed structure constant. Then

$$
L_{\rm grav}=-q\frac{GM^2}{R^2}\dot R,\qquad
L_{\rm int}\sim\frac{GM^2}{R\tau_{\rm KH}},
$$

up to the structure and virial coefficients, where $\tau_{\rm KH}$ is the [Kelvin-Helmholtz cooling time](../../../stellar-astrophysics.md#kelvin-helmholtz-cooling-time).

For a diatomic gas with $\gamma=7/5$ the idealized fraction is $1/6$, already demonstrating that the half-factor is not universal. Partial [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure), dissociation, changing structure, accretion and deep heating require the full energy equation. The general link between luminosity and [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) is $L_{\rm int}=-d(U+\Omega)/dt$, with any genuine source terms added explicitly.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Assume the planet and present-day [Jupiter](../../../planetary-science.md#jupiter) have the same [mass](../../../classical-mechanics.md#mass), comparable composition and initial cooling normalization, and both can be described by the supplied [power-law planetary cooling](../../../stellar-astrophysics.md#power-law-planetary-cooling) over the relevant ages. Take the age of present-day [Jupiter](../../../planetary-science.md#jupiter) to be $t_J\simeq4.5\,\mathrm{Gyr}$ and the young planet's age to be $0.050\,\mathrm{Gyr}$. The normalization cancels:

$$
\boxed{\frac{L_{\rm int}(50\,\mathrm{Myr})}{L_{\rm int,J}}
=\left(\frac{4.5}{0.050}\right)^{3/2}
=90^{3/2}\simeq8.5\times10^2.}
$$

The 5-AU orbit is used to regard stellar irradiation as modest compared with a hot-Jupiter orbit; the ratio is specifically intrinsic cooling, not the sum of intrinsic and reradiated [luminosity](../../../astrophysics.md#luminosity). Initial [entropy](../../../thermodynamics.md#entropy) and irradiation can change the assumed normalization, so this estimate is not independent of formation conditions.

Such a young self-luminous giant is a favourable target for near-infrared [exoplanet direct imaging](../../../exoplanet.md#exoplanet-direct-imaging). The increased intrinsic [luminosity](../../../astrophysics.md#luminosity) improves its contrast with the host star, and a wide physical orbit is more readily separated on the sky than a hot-Jupiter orbit. Two essential observing considerations are:

- **Angular separation:** at distance $d$ parsecs, a projected 5-AU separation is at most roughly $5/d$ arcseconds. It must exceed the instrumental inner working angle; orbital projection can make it smaller. Nearby targets and [adaptive optics](../../../optics.md#adaptive-optics) help.
- **Planet-star contrast and wavelength:** the band must balance the young planet's [thermal radiation](../../../electromagnetism.md#thermal-radiation), stellar leakage, detector sensitivity and thermal background. Suppression with a [coronagraph](../../../optics.md#coronagraph) and stable calibration are required; a large intrinsic bolometric ratio to old [Jupiter](../../../planetary-science.md#jupiter) is not itself the measured contrast with the star.

Thus **direct imaging of a nearby young system, with sufficient angular resolution and contrast, is the natural discovery method**, subject to the actual stellar brightness and instrumental limits.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Assume the present epoch has the same age as present-day [Jupiter](../../../planetary-science.md#jupiter), the host now has solar [luminosity](../../../astrophysics.md#luminosity), and moving inward did not change the stipulated intrinsic cooling law or its normalization. This neglects persistent tidal heating and irradiation-induced suppression of cooling. The [intrinsic planetary luminosity](../../../stellar-astrophysics.md#intrinsic-planetary-luminosity) is then approximately $L_{\rm int,J}$, not its value at the migration epoch.

Define incident irradiation as intercepted power before reflection,

$$
L_{\rm irr}=\pi R_p^2\frac{L_*}{4\pi a^2}
=\frac{R_p^2L_*}{4a^2}.
$$

Comparing with present-day [Jupiter](../../../planetary-science.md#jupiter) at $a_J\simeq5\,\mathrm{AU}$ gives

$$
\frac{L_{\rm irr}}{L_{\rm irr,J}}
=\left(\frac{R_p}{R_J}\right)^2\left(\frac{L_*}{L_\odot}\right)
\left(\frac{a_J}{0.05\,\mathrm{AU}}\right)^2
\simeq10^4\left(\frac{R_p}{R_J}\right)^2.
$$

For equal [radii](../../../topology.md#radius),

$$
\boxed{\frac{L_{\rm int}}{L_{\rm irr}}
\simeq10^{-4}\frac{L_{\rm int,J}}{L_{\rm irr,J}}.}
$$

Retaining unequal [radii](../../../topology.md#radius) multiplies the right side by $(R_J/R_p)^2$. If irradiation instead denotes incident [radiative flux](../../../astrophysics.md#radiative-flux) per area, the orbital factor is still $10^4$, but it must be compared with an intrinsic flux consistently. Absorbed power also includes $1-A_B$, so comparisons of absorbed irradiation require the two [Bond albedos](../../../exoplanet.md#bond-albedo).

Close-in gas giants motivate [planetary migration](../../../planetary-science.md#planetary-migration) when compared with formation models. Two useful observational diagnostics are then orbital eccentricities and spin-orbit geometry. An eccentric population of wider potential progenitors together with circular short-period orbits supports eccentricity excitation followed by [tidal dissipation](../../../planetary-science.md#tidal-dissipation). The second diagnostic is [stellar obliquity](../../../planetary-science.md#stellar-obliquity), including misaligned or retrograde orbits measured through the [Rossiter-McLaughlin effect](../../../planetary-science.md#rossiter-mclaughlin-effect); these can favour scattering or secular pathways over smooth coplanar migration. Conversely, aligned resonant architectures are compatible with disc-driven migration. None is unique: primordial disc tilt or alternative formation can mimic some signatures. **The expected present-day ratio is suppressed by the inverse-square orbital factor, while eccentricities and spin-orbit geometry test migration pathways.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume a Newtonian, spherically symmetric, nonrotating body in [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium), supported by a [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) $P=K\rho^{1+1/n}$ with constant $K>0$ and $n>0$. The [enclosed mass](../../../stellar-structure.md#enclosed-mass) and [hydrostatic pressure support equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) are

$$
\frac{dm}{dr}=4\pi r^2\rho,\qquad
\frac{dP}{dr}=-\frac{Gm\rho}{r^2}.
$$

Eliminate $m$ by first writing $r^2\rho^{-1}dP/dr=-Gm$ and then differentiating:

$$
\frac1{r^2}\frac{d}{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)
=-4\pi G\rho.
$$

Let $\rho_c$ be central [mass density](../../../fluid-mechanics.md#density), and introduce the [Lane-Emden variables for a stellar polytrope](../../../stellar-structure.md#lane-emden-variables-for-a-stellar-polytrope)

$$
\rho=\rho_c\theta^n,\qquad
P=K\rho_c^{1+1/n}\theta^{n+1},\qquad
r=a\xi,
$$

where

$$
a^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

Then $(1/\rho)dP/dr=(n+1)K\rho_c^{1/n}d\theta/dr$. Substitution cancels the dimensional factors and yields the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation)

$$
\boxed{\frac1{\xi^2}\frac{d}{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)
=-\theta^n,\qquad \theta(0)=1,\quad\theta'(0)=0.}
$$

The central conditions enforce the chosen central [mass density](../../../fluid-mechanics.md#density) and regular [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry). The local regular expansion is $\theta=1-\xi^2/6+n\xi^4/120+\cdots$. If a finite first zero $\xi_1$ exists and surface [pressure](../../../thermodynamics.md#pressure) is negligible, the physical [radius](../../../topology.md#radius) is $R=a\xi_1$, and the [Lane-Emden mass formula](../../../stellar-structure.md#lane-emden-mass-formula) is $M=4\pi a^3\rho_c[-\xi_1^2\theta'(\xi_1)]$. For $0<n<5$ the standard isolated solution has a finite surface; $n=5$ has infinite extent, so a finite surface must not be assumed for all indices. Irradiation, composition stratification and non-polytropic equations of state require more general structure equations.

## 4

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Three complementary methods available in the setting of this 2017 paper are:

- [Exoplanet transmission spectra](../../../exoplanet.md#exoplanet-transmission-spectrum) during primary transit. The planet's atmosphere filters stellar light at the [day-night terminator](../../../exoplanet.md#day-night-terminator). Its advantages are a bright background source and sensitivity to atomic, molecular and aerosol [opacity](../../../stellar-structure.md#opacity); its limitations are the need for a transit, a small annular signal, [exoplanet cloud](../../../exoplanet.md#exoplanet-cloud) masking, and degeneracies among abundance, reference [pressure](../../../thermodynamics.md#pressure), [temperature](../../../thermodynamics.md#temperature) and [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight). The useful physical range is ultraviolet through near- and mid-infrared, subject to instrumentation. The [Hubble Space Telescope](../../../exoplanet.md#hubble-space-telescope) is an appropriate example, with ultraviolet/optical instruments and near-infrared transit spectroscopy, particularly around $1.1$--$1.7\,\mu\mathrm m$ with WFC3.
- [Exoplanet secondary eclipse](../../../exoplanet.md#exoplanet-secondary-eclipse) spectroscopy or photometry. Subtracting the stellar-only light in eclipse from the combined light outside eclipse isolates the dayside thermal and reflected spectrum. It measures dayside [brightness temperature](../../../exoplanet.md#brightness-temperature) and composition and can reveal an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology). Limitations include eclipse geometry, a weak planet-star contrast, and the joint dependence of features on [opacity](../../../stellar-structure.md#opacity) and the [atmospheric pressure-temperature profile](../../../exoplanet.md#atmospheric-pressure-temperature-profile). Reflection is most useful in the optical, and thermal emission in the near- to mid-infrared. The [Spitzer Space Telescope](../../../exoplanet.md#spitzer-space-telescope) is a major example: earlier cryogenic observations included infrared spectroscopy, while in 2017 the warm mission provided 3.6- and 4.5-micrometre photometry.
- [Exoplanet direct imaging](../../../exoplanet.md#exoplanet-direct-imaging). Spatial separation isolates the planet's own spectrum without requiring a transit, and favours young hot giants on wide orbits. Limitations are small angular separation, overwhelming stellar leakage, restricted inner working angle and instrument contrast. Near-infrared spectra of young giants are especially useful, with optical reflected light and thermal infrared also possible for suitable targets. The [Very Large Telescope](../../../exoplanet.md#very-large-telescope), for example with its SPHERE imager, provides optical/near-infrared high-contrast observations using [adaptive optics](../../../optics.md#adaptive-optics) and stellar-light suppression.

**Transmission probes the limb, eclipses probe the dayside, and direct imaging isolates spatially resolved planetary light.** Radial velocities alone measure orbital motion rather than atmospheric composition; high-resolution planetary Doppler spectroscopy can instead detect atmospheric spectral lines if planetary light is isolated statistically.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Take an unresolved spherical planet at [Euclidean distance](../../../topological-analysis.md#euclidean-distance) $d\gg R$, with uniform surface [temperature](../../../thermodynamics.md#temperature) $T$, stationary isotropic emission, and no intervening extinction. Isothermality does not by itself imply [blackbody](../../../astrophysics.md#blackbody) radiation; first derive the geometric result for a uniform emergent [specific intensity](../../../astrophysics.md#specific-intensity) $I_\lambda$.

The observer sees the projected disc with apparent [solid angle](../../../geometry-and-topology.md#solid-angle) $\Omega_p\simeq\pi R^2/d^2$. Integrating its [specific intensity](../../../astrophysics.md#specific-intensity) over that angle gives the observed spectral [radiative flux](../../../astrophysics.md#radiative-flux)

$$
f_\lambda=\int_{\rm disc}I_\lambda\cos\theta_{\rm obs}\,d\Omega
\simeq\pi I_\lambda\frac{R^2}{d^2},
$$

where $\theta_{\rm obs}$ is the small angle to the detector normal. For a [blackbody](../../../astrophysics.md#blackbody), $I_\lambda=B_\lambda(T)$, and the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) gives $\int_0^\infty\pi B_\lambda(T)\,d\lambda=\sigma_{\rm SB}T^4$. Hence

$$
\boxed{f_\lambda=\pi B_\lambda(T)(R/d)^2,\qquad
f=\sigma_{\rm SB}T^4(R/d)^2=\frac{L}{4\pi d^2}.}
$$

Equivalently, the surface [radiative flux](../../../astrophysics.md#radiative-flux) is $\sigma_{\rm SB}T^4$ and the [luminosity of a spherical blackbody](../../../astrophysics.md#luminosity-of-a-spherical-blackbody) is $L=4\pi R^2\sigma_{\rm SB}T^4$, leading to the same result by inverse-square dilution. A uniform wavelength-dependent [emissivity](../../../thermodynamics.md#emissivity) $\epsilon_\lambda$ multiplies the spectral formula; an atmospheric spectrum can require a full angular [radiative transfer](../../../astrophysics.md#radiative-transfer) integral rather than a single [Planck function](../../../astrophysics.md#planck-function).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Consider a narrow bundle of rays between two surface elements $dA_1,dA_2$ separated by $s$ in a transparent, stationary Euclidean vacuum. Let the ray make angles $\theta_1,\theta_2$ to the respective surface normals. The receiving element subtends [solid angle](../../../geometry-and-topology.md#solid-angle) $d\Omega_1=\cos\theta_2dA_2/s^2$ at the emitter. By the definition of [specific intensity](../../../astrophysics.md#specific-intensity), the beam power in frequency interval $d\nu$ is

$$
d\mathcal P_\nu=I_{\nu,1}\cos\theta_1dA_1\,d\Omega_1\,d\nu
=I_{\nu,1}\frac{\cos\theta_1\cos\theta_2dA_1dA_2}{s^2}\,d\nu.
$$

At the receiving end the source subtends $d\Omega_2=\cos\theta_1dA_1/s^2$, so the identical power is

$$
d\mathcal P_\nu=I_{\nu,2}\frac{\cos\theta_1\cos\theta_2dA_1dA_2}{s^2}\,d\nu.
$$

In the absence of absorption, emission or frequency shifts, [conservation of energy](../../../physics.md#conservation-of-energy) equates these expressions:

$$
\boxed{I_{\nu,2}=I_{\nu,1}.}
$$

This [vacuum conservation of specific intensity](../../../astrophysics.md#vacuum-conservation-of-specific-intensity) also follows directly from the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) $dI_\nu/ds=0$. The apparent [solid angle](../../../geometry-and-topology.md#solid-angle) of an unresolved source shrinks as $s^{-2}$, so its integrated observed [radiative flux](../../../astrophysics.md#radiative-flux) still follows the inverse-square law. Specific intensity and unresolved flux are different quantities.

The vacuum and frequency assumptions are essential: absorption and emission change [specific intensity](../../../astrophysics.md#specific-intensity), and gravitational or cosmological redshift conserves $I_\nu/\nu^3$ along a ray instead of $I_\nu$ itself. A fixed telescope aperture observing an unresolved object also cannot infer constant total received power from intensity conservation.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let an isothermal non-scattering atmospheric layer of [temperature](../../../thermodynamics.md#temperature) $T_a$ lie above an optically thick continuum source with [brightness temperature](../../../exoplanet.md#brightness-temperature) $T_b$. Assume [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium), so the layer emits with [Planck function](../../../astrophysics.md#planck-function) $B_\lambda(T_a)$. Its vertical [optical depth](../../../astrophysics.md#optical-depth) is $\tau_\lambda$; a ray with direction cosine $\mu$ has slant depth $t_\lambda=\tau_\lambda/\mu$.

The [formal solution of the radiative transfer equation](../../../astrophysics.md#formal-solution-of-the-radiative-transfer-equation) gives

$$
\boxed{I_\lambda=B_\lambda(T_b)e^{-t_\lambda}
+B_\lambda(T_a)(1-e^{-t_\lambda}).}
$$

The two terms are attenuated background and layer emission. Compare a line and nearby continuum at the same wavelength to adequate approximation, with $t_{\rm line}>t_{\rm cont}$. The [one-layer spectral contrast](../../../astrophysics.md#one-layer-spectral-contrast) is

$$
I_{\rm line}-I_{\rm cont}
=[B_\lambda(T_a)-B_\lambda(T_b)]
[e^{-t_{\rm cont}}-e^{-t_{\rm line}}].
$$

The second bracket is positive, and $B_\lambda(T)$ increases with [temperature](../../../thermodynamics.md#temperature). Therefore a cooler upper layer produces absorption, a hotter upper layer produces emission, and an isothermal source-plus-layer produces no line contrast:

$$
\boxed{T_a<T_b:\ \text{absorption};\quad
T_a>T_b:\ \text{emission};\quad T_a=T_b:\ \text{no contrast}.}
$$

This is why higher [opacity](../../../stellar-structure.md#opacity) sampling a cooler altitude creates absorption in an outward-cooling atmosphere, whereas an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) can create emission. If both line and continuum are very optically thick in the same layer, their contrast tends to vanish even with a different deeper [temperature](../../../thermodynamics.md#temperature). Scattering, non-LTE excitation, and nonuniform layers require a more general [radiative transfer](../../../astrophysics.md#radiative-transfer) treatment.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The three parameter groups are **local temperature, local pressure, and elemental composition**. The elemental composition includes both [atmospheric metallicity of a giant planet](../../../exoplanet.md#atmospheric-metallicity-of-a-giant-planet) and [atmospheric carbon-to-oxygen ratio](../../../exoplanet.md#atmospheric-carbon-to-oxygen-ratio); these are independent compositional controls, so a specification by $T$ and $P$ alone is incomplete. Given these inputs, [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium) minimizes [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy) with element conservation.

Three useful chemical observables in a hydrogen-rich [hot Jupiter](../../../exoplanet.md#hot-jupiter) are:

- The [carbon monoxide](../../../chemistry.md#carbon-monoxide)-to-[methane](../../../chemistry.md#methane) partition. For $\mathrm{CO}+3\mathrm H_2\rightleftharpoons\mathrm{CH}_4+\mathrm H_2\mathrm O$, cooler gas and, at fixed mole fractions, larger [pressure](../../../thermodynamics.md#pressure) favour the side with fewer molecules, whereas hotter gas generally favours CO. Thus relatively hot photospheres commonly show CO near $2.3$ and $4.6\,\mu\mathrm m$, while cooler conditions favour [methane](../../../chemistry.md#methane) bands near $3.3\,\mu\mathrm m$. The exact boundary depends on composition and [pressure](../../../thermodynamics.md#pressure); [carbon monoxide–methane quenching](../../../exoplanet.md#carbon-monoxide-methane-quenching) can invalidate an equilibrium diagnosis.
- [Water](../../../chemistry.md#water) absorption, for example around $1.4$ and $2.7\,\mu\mathrm m$, traces the oxygen left after CO forms. In oxygen-rich gas with $\mathrm{C/O}<1$, water is often prominent; carbon-rich gas can have much less water and relatively more [methane](../../../chemistry.md#methane) or [hydrogen cyanide](../../../chemistry.md#hydrogen-cyanide). Condensation and high-temperature dissociation are exceptions to a simple elemental bookkeeping argument.
- [Carbon dioxide](../../../chemistry.md#carbon-dioxide), with a strong band near $4.3\,\mu\mathrm m$, is sensitive to enrichment and oxidation chemistry. In a hydrogen-dominated trace-species regime, $\mathrm{CO}+\mathrm H_2\mathrm O\rightleftharpoons\mathrm{CO}_2+\mathrm H_2$ gives $x_{\rm CO_2}\propto x_{\rm CO}x_{\rm H_2O}/x_{\rm H_2}$ at fixed $T$, so CO2 can grow roughly quadratically with heavy-element enrichment before the trace approximation fails.

**CO/CH4, H2O, and CO2 bands provide complementary temperature and elemental-abundance diagnostics**, but their observed strengths also depend on the [atmospheric pressure-temperature profile](../../../exoplanet.md#atmospheric-pressure-temperature-profile), [exoplanet clouds](../../../exoplanet.md#exoplanet-cloud) and observing geometry. A spectral feature is not by itself a direct equilibrium abundance.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Three routes away from local [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium) are:

- Vertical transport and quenching. When the [eddy mixing time](../../../exoplanet.md#eddy-mixing-time) becomes shorter than the [chemical relaxation time](../../../thermodynamics.md#chemical-relaxation-time), gas retains a deeper composition. In cool, directly imaged giant [exoplanets](../../../exoplanet.md), [carbon monoxide–methane quenching](../../../exoplanet.md#carbon-monoxide-methane-quenching) can preserve CO and suppress the methane expected in cool equilibrium layers. In [Jupiter](../../../planetary-science.md#jupiter), CO carried from deeper hot layers, and [phosphine](../../../chemistry.md#phosphine) maintained against upper-atmosphere chemical loss, are examples of transported disequilibrium species.
- Horizontal transport and quenching. [Atmospheric advection time](../../../exoplanet.md#atmospheric-advection-time) shorter than the local [chemical relaxation time](../../../thermodynamics.md#chemical-relaxation-time) carries abundances between regions of different [temperature](../../../thermodynamics.md#temperature). A [hot Jupiter](../../../exoplanet.md#hot-jupiter) can carry CO-rich dayside gas into cooler nightside gas that would otherwise favour [methane](../../../chemistry.md#methane). In the Solar System, upper-atmosphere CO produced on the illuminated side of [Venus](../../../planetary-science.md#venus) can be redistributed to its dark side by circulation; this is an example of nonlocal production and transport, rather than local dark-side thermochemical equilibrium.
- [Atmospheric photochemistry](../../../exoplanet.md#atmospheric-photochemistry). Ultraviolet photons dissociate or ionize molecules and initiate reaction networks. Models of irradiated hydrogen-rich [exoplanet atmospheres](../../../exoplanet.md#exoplanet-atmosphere) can produce enhanced [hydrogen cyanide](../../../chemistry.md#hydrogen-cyanide) and hydrocarbon precursors from methane/nitrogen chemistry; whether these products accumulate depends on ultraviolet flux and transport. The [terrestrial atmosphere](../../../planetary-science.md#terrestrial-atmosphere) gives a clear Solar-System example: oxygen photodissociation and subsequent reactions maintain the [ozone layer](../../../exoplanet.md#ozone-layer), which is not a purely thermochemical-equilibrium abundance.

**Vertical mixing, horizontal advection, and photochemistry supply three mechanisms and examples in both exoplanets and Solar-System atmospheres.** A photochemical steady state balances production and loss; it is different from a [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy) minimum. These examples describe mechanisms and model expectations rather than asserting unique observational attribution for every planet.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

One approach uses [exoplanet transmission spectra](../../../exoplanet.md#exoplanet-transmission-spectrum). Three aerosol signatures are:

- Muted molecular-band amplitudes in the near-infrared, for example weak [water](../../../chemistry.md#water) structure around $1.4\,\mu\mathrm m$: an [optically thick](../../../astrophysics.md#optically-thick-medium) [exoplanet cloud deck](../../../exoplanet.md#exoplanet-cloud-deck) raises the continuum and hides part of the gas column.
- A nearly grey transit-radius continuum across optical/near-infrared wavelengths, roughly $0.5$--$2\,\mu\mathrm m$, when particles are large relative to the wavelengths. Suppressed optical atomic-line wings provide a related indication that deep high-[pressure](../../../thermodynamics.md#pressure) layers are hidden.
- A radius increasing toward blue/ultraviolet wavelengths, roughly $0.3$--$1\,\mu\mathrm m$, for small-particle [scattering of light](../../../optics.md#scattering-of-light). In a simple [Rayleigh scattering](../../../electromagnetism.md#rayleigh-scattering) limit, $\sigma\propto\lambda^{-4}$, and the [scattering slope of a transmission spectrum](../../../exoplanet.md#scattering-slope-of-a-transmission-spectrum) is $dR_p/d\log\lambda=-4H$.

A second approach uses the dayside spectrum and brightness obtained with [exoplanet secondary eclipses](../../../exoplanet.md#exoplanet-secondary-eclipse), optionally supported by orbital phase variations. Its three useful aerosol signatures are:

- Enhanced reflected-light [geometric albedo](../../../exoplanet.md#geometric-albedo) or characteristic colour in the visible, roughly $0.4$--$0.9\,\mu\mathrm m$, for a scattering [exoplanet cloud](../../../exoplanet.md#exoplanet-cloud). Absorbing [atmospheric haze](../../../exoplanet.md#haze) can instead lower the reflected flux, so high albedo is not a universal aerosol rule.
- Weak near-/mid-infrared gas features and a cloud-set continuum [brightness temperature](../../../exoplanet.md#brightness-temperature), roughly $1$--$10\,\mu\mathrm m$, when an opaque cloud moves the thermal photosphere to a different [pressure](../../../thermodynamics.md#pressure). Changes in the [exoplanet thermal phase curve](../../../exoplanet.md#exoplanet-thermal-phase-curve) can support a spatially patchy cloud interpretation, though circulation also affects it.
- Broad condensate-dependent infrared spectral structure, for example a silicate resonance around $10\,\mu\mathrm m$, if particles are sufficiently small and the optical-depth/temperature geometry permits the feature. Its presence and sign depend on particle composition, size and vertical thermal structure.

**Transmission measures aerosol extinction along the limb; eclipse/reflection measurements test dayside scattering and emission.** No single flattened feature proves clouds: small [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height), low molecular abundances, stellar heterogeneity and thermal-gradient degeneracies must be considered. Joint wavelength coverage and geometries make the inference stronger.

<h3 id="4/h">h</h3>

↑ **Parent:** [4](#4)

<h4 id="4/h/solution">Solution</h4>

↑ **Parent:** [H](#4/h)

[Hot-Jupiter radius inflation](../../../exoplanet.md#hot-jupiter-radius-inflation) is the excess [radius](../../../topology.md#radius) of many irradiated gas giants relative to standard cooling models of the same [mass](../../../classical-mechanics.md#mass), composition and age. A young gas giant starts with high [entropy](../../../thermodynamics.md#entropy) and a large [radius](../../../topology.md#radius), but ordinarily contracts through [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism). An old inflated object must either retain that thermal reservoir unusually well or receive power that affects the deep interior.

The first class is [delayed cooling of an inflated giant planet](../../../exoplanet.md#delayed-cooling-of-an-inflated-giant-planet). Two specific mechanisms are increased atmospheric [opacity](../../../stellar-structure.md#opacity), which makes internal radiation escape less readily, and inhibited interior [convection](../../../fluid-mechanics.md#convection) caused by composition gradients, potentially with layered transport. Both slow entropy loss. Stellar irradiation can also maintain an outer radiative blanket, but an appropriate irradiated boundary is already included in many baseline models and does not alone explain every extreme [radius](../../../topology.md#radius).

The second class is [heating of an inflated giant planet](../../../exoplanet.md#heating-of-an-inflated-giant-planet). Two mechanisms are [tidal heating](../../../planetary-science.md#tidal-heating) from eccentricity, obliquity or other time-dependent tidal forcing, and [Joule heating](../../../electromagnetism.md#joule-heating) from wind-driven electric currents in an ionized atmosphere coupled to the [magnetic field](../../../electromagnetism.md#magnetic-field). Mechanical energy carried inward from atmospheric circulation is another candidate. Heating must be deposited sufficiently deeply and with sufficient power; superficial absorption that is promptly reradiated is not equivalent to deep interior heating. A circular synchronized isolated orbit does not automatically provide a persistent tidal source.



$$
\boxed{\text{Retain heat: higher opacity or inhibited convection;}\qquad
\text{add deep heat: tides or electrical dissipation}.}
$$

The classes can coexist and are tested through radius-age-irradiation trends, orbital properties and the required energy budget. Merely changing an observed transit altitude by a few [atmospheric scale heights](../../../exoplanet.md#atmospheric-scale-height) is generally distinct from inflating the bulk giant-planet interior.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

At fixed [mass](../../../classical-mechanics.md#mass), three broad controls of a super-Earth-sized body's observed [radius](../../../topology.md#radius) are:

- Bulk composition and material compressibility. A larger iron-core fraction usually makes an [exoplanet interior](../../../exoplanet.md#exoplanet-interior) denser and smaller, whereas silicate or water-rich interiors are larger. The [planetary mass-radius relation](../../../exoplanet.md#planetary-mass-radius-relation) therefore differs among compositions; mass and radius alone retain an [exoplanet interior-composition degeneracy](../../../exoplanet.md#exoplanet-interior-composition-degeneracy).
- A gaseous envelope and its retention. Even a modest [hydrogen](../../../chemistry.md#hydrogen)-[helium](../../../chemistry.md#helium) mass fraction can substantially increase [radius](../../../topology.md#radius) through the [transit-radius contribution of a gaseous envelope](../../../exoplanet.md#transit-radius-contribution-of-a-gaseous-envelope). Its [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight), total atmospheric mass and [opacity](../../../stellar-structure.md#opacity) determine how far the slant-optical-depth surface lies above the condensed interior. [Atmospheric escape](../../../exoplanet.md#atmospheric-escape) can strip that envelope, producing a much smaller object without a comparable loss of core mass.
- Thermal and irradiation history. Higher interior [entropy](../../../thermodynamics.md#entropy), youth and stellar heating tend to expand an envelope; [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) reduces its size over time. Stellar high-energy exposure affects the envelope through [atmospheric escape](../../../exoplanet.md#atmospheric-escape). [Exoplanet clouds](../../../exoplanet.md#exoplanet-cloud) and wavelength-dependent [opacity](../../../stellar-structure.md#opacity) shift the measured transit radius even when the deep interior is unchanged.

**Bulk composition, envelope fraction/composition, and thermal/irradiation history are three independent controls.** If mass is not fixed, the [mass](../../../classical-mechanics.md#mass) itself is an additional major variable. The label [super-Earth](../../../exoplanet.md#super-earth) does not ensure a rocky composition or an Earth-like atmosphere, and a radius alone does not determine which of these effects dominates.

<h3 id="4/j">j</h3>

↑ **Parent:** [4](#4)

<h4 id="4/j/solution">Solution</h4>

↑ **Parent:** [J](#4/j)

Three research directions natural in the 2017 setting are:

- Atmospheric characterization of small planets, extending beyond bright [hot Jupiters](../../../exoplanet.md#hot-jupiter) to super-Earth-sized and terrestrial bodies. The aim is to determine whether they retain light envelopes or heavier secondary atmospheres and to understand [exoplanet habitability](../../../exoplanet.md#exoplanet-habitability). Potential [exoplanet biosignatures](../../../exoplanet.md#exoplanet-biosignature) require a chemical and stellar context because abiotic processes can mimic individual molecules; future infrared observatories such as the then-planned [James Webb Space Telescope](../../../exoplanet.md#james-webb-space-telescope) offered a route to better spectra, without guaranteeing a biological interpretation.
- Connecting measured composition to [planet formation](../../../planetary-science.md#planet-formation) and [planetary migration](../../../planetary-science.md#planetary-migration). [Atmospheric metallicity of a giant planet](../../../exoplanet.md#atmospheric-metallicity-of-a-giant-planet), [atmospheric carbon-to-oxygen ratio](../../../exoplanet.md#atmospheric-carbon-to-oxygen-ratio), orbital architecture and bulk [mass](../../../classical-mechanics.md#mass)-[radius](../../../topology.md#radius) measurements can constrain accretion of gas and solids. [Atmospheric condensate rainout](../../../exoplanet.md#atmospheric-condensate-rainout), [disequilibrium chemistry in an exoplanet atmosphere](../../../exoplanet.md#disequilibrium-chemistry-in-an-exoplanet-atmosphere) and [exoplanet interior-composition degeneracy](../../../exoplanet.md#exoplanet-interior-composition-degeneracy) make a one-to-one mapping from a measured ratio to a birth location unreliable; comparative samples and coupled models are needed.
- Resolving atmospheric structure in space and time. [Exoplanet thermal phase curves](../../../exoplanet.md#exoplanet-thermal-phase-curve), repeated spectra, high-resolution planetary spectroscopy and [exoplanet direct imaging](../../../exoplanet.md#exoplanet-direct-imaging) can test [day-night heat redistribution](../../../exoplanet.md#day-night-heat-redistribution), winds, patchy [exoplanet clouds](../../../exoplanet.md#exoplanet-cloud), [atmospheric escape](../../../exoplanet.md#atmospheric-escape) and chemical heterogeneity. The challenge is to distinguish actual variability or circulation from changes in stellar light and instrumental calibration.

**Small-planet atmospheres, formation through composition, and atmospheric dynamics/variability provide three concrete emerging directions.** The examples describe research aims as of the paper's date, rather than treating later discoveries or later operating missions as established in 2017.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
