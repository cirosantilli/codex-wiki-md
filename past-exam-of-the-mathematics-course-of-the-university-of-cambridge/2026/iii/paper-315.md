# Paper 315

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20315.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20315.pdf)

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
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
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

The [internal effective temperature of a planet](../../../exoplanet.md#internal-effective-temperature-of-a-planet) $T_{\rm int}$ parametrizes intrinsic cooling, while the [irradiation temperature](../../../exoplanet.md#irradiation-temperature) $T_{\rm irr}$ parametrizes incident stellar flux before the redistribution factor $f$. The quantity

$$
\gamma=\frac{\kappa_{\rm vis}}{\kappa_{\rm IR}}
$$

is the visible-to-thermal mean-opacity ratio, and $\tau$ is downward thermal [optical depth](../../../astrophysics.md#optical-depth). Under the Eddington two-stream boundary condition,

$$
a=\frac34,
\qquad b=\frac23,
\qquad\boxed{ab=\frac12},
$$

while the common semi-grey choice is $c=\sqrt3$.

For a young giant at $40\,\mathrm{au}$, stellar heating is weak and a still-large $T_{\rm int}$ dominates. Its pressure-temperature profile rises steadily inward, approximately as $T^4\propto b+\tau$, and joins a deep convective adiabat.

For a hot Jupiter close to a Sun-like star, $T_{\rm irr}\gg T_{\rm int}$. It has a broad, nearly isothermal irradiated radiative layer, followed by a deep rise where intrinsic flux and increasing opacity matter. If $\gamma>1$, absorption of starlight above the thermal photosphere can create an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology).

For a temperate sub-Neptune around an M dwarf, irradiation and internal cooling can be more comparable. Its profile generally has a moderate radiative layer above a convective interior; near-infrared stellar radiation, molecular opacity, clouds, and hazes determine whether the upper profile is weakly inverted or decreases outward.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At depths satisfying $\gamma c\tau\gg1$, the exponential term is negligible. The atmosphere remains approximately isothermal while its intrinsic contribution is also small:

$$
T_{\rm int}^4(b+\tau)
\ll fT_{\rm irr}^4
\left(b+\frac1{\gamma c}\right).
$$

Thus the plateau occupies approximately

$$
\boxed{
\frac1{\gamma c}\ll\tau\ll
f\left(\frac{T_{\rm irr}}{T_{\rm int}}\right)^4
\left(b+\frac1{\gamma c}\right)-b}
$$

and has temperature

$$
\boxed{T_{\rm iso}\simeq T_{\rm irr}
\left[af\left(b+\frac1{\gamma c}\right)\right]^{1/4}}.
$$

For example, take $T_{\rm irr}=2000\,\mathrm K$, $T_{\rm int}=200\,\mathrm K$, $\gamma=1$, $f=1/2$, and the Eddington constants. Then $T_{\rm iso}\simeq1650\,\mathrm K$ and the formal plateau extends from $\tau$ of order unity to several thousand. At still greater depth,

$$
T^4\simeq aT_{\rm int}^4\tau+	ext{constant},
$$

so the radiative solution rises as $T\propto\tau^{1/4}$ until convection replaces it.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Differentiating the [semi-grey irradiated atmosphere](../../../exoplanet.md#semi-grey-irradiated-atmosphere) profile gives

$$
4T^3\frac{dT}{d\tau}
=a\left[T_{\rm int}^4
+fT_{\rm irr}^4(1-\gamma^2)e^{-\gamma c\tau}\right].
$$

Hydrostatic balance gives $d\tau/dP=\kappa_{\rm IR}/g$ when the thermal mean opacity is locally constant. Hence

$$
\boxed{
\frac{dT}{dP}
=\frac{a\kappa_{\rm IR}}{4gT^3}
\left[T_{\rm int}^4
+fT_{\rm irr}^4(1-\gamma^2)e^{-\gamma c\tau}\right]}.
$$

For variable opacity, replace $\kappa_{\rm IR}$ by its local value and integrate $d\tau=\kappa_{\rm IR}(P,T)dP/g$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A useful first estimate places the [radiative-convective boundary](../../../exoplanet.md#radiative-convective-boundary) where the intrinsic term becomes comparable to the deep irradiation plateau:

$$
T_{\rm int}^4\tau_{\rm RCB}
\sim fT_{\rm irr}^4
\left(b+\frac1{\gamma c}\right).
$$

Thus

$$
\boxed{\tau_{\rm RCB}\sim
f\left(\frac{T_{\rm irr}}{T_{\rm int}}\right)^4
\left(b+\frac1{\gamma c}\right)},
\qquad
\boxed{P_{\rm RCB}\sim\frac g{\kappa_{\rm IR}}\tau_{\rm RCB}}.
$$

With the assumptions of part (b), $g=10\,\mathrm{m\,s^{-2}}$ and $\kappa_{\rm IR}=10^{-3}\,\mathrm{m^2\,kg^{-1}}$, one finds $\tau_{\rm RCB}\sim6.2\times10^3$ and $P_{\rm RCB}\sim6.2\times10^7\,\mathrm{Pa}\simeq620\,\mathrm{bar}$.

More precisely one equates the local radiative logarithmic gradient to the adiabatic gradient. A constant-opacity grey profile approaches $\nabla_{\rm rad}=1/4$, so a diatomic adiabat with $\nabla_{\rm ad}=2/7$ requires the realistic increase of opacity with depth to become convective. The numerical pressure is therefore an order-of-magnitude estimate, sensitive mainly to $T_{\rm int}$ and deep opacity.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A thermal inversion means temperature rises outward, so $dT/d\tau<0$. From part (c), near the observable atmosphere this requires

$$
T_{\rm int}^4
+fT_{\rm irr}^4(1-\gamma^2)e^{-\gamma c\tau}<0.
$$

At the top, the condition is

$$
\boxed{\gamma>1,
\qquad
fT_{\rm irr}^4(\gamma^2-1)>T_{\rm int}^4}.
$$

It states that shortwave absorption high in the atmosphere must overwhelm intrinsic heating.

Jupiter has substantial intrinsic flux and generally lacks enough persistent high-altitude visible opacity for a strong global inversion, although localized stratospheric heating occurs. An ultra-hot Jupiter around a $6500\,\mathrm K$ star receives intense optical and ultraviolet radiation; metals, TiO/VO where present, and continuum absorption can make $\gamma>1$, so inversions are common. A temperate sub-Neptune around a $2500\,\mathrm K$ star receives much of its stellar power in the near infrared, where the same molecules also emit thermally. This reduces the separation between shortwave and longwave opacity; clouds or photochemical hazes can still create upper heating, but an inversion is less automatic.

## 2

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

At full phase immediately before an [exoplanet secondary eclipse](../../../exoplanet.md#exoplanet-secondary-eclipse), reflected and thermal light give

$$
\boxed{
\frac{F_p}{F_*}(\lambda)
=A_g(\lambda)\left(\frac{R_p}{a_{\rm orb}}\right)^2
+\left(\frac{R_p}{R_*}\right)^2
\frac{B_\lambda(T_p)}{B_\lambda(T_*)}}.
$$

The phase function equals one at secondary eclipse. For the stated model, the first term is constant below $1\,\mu\mathrm m$ and negligible above it. The $600\,\mathrm K$ thermal component is tiny in the visible, rises through the infrared, and peaks near $4.8\,\mu\mathrm m$ in $B_\lambda$, while the contrast continues to improve toward the mid-infrared because the stellar spectrum falls more rapidly.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Assume full heat redistribution, so

$$
T_{\rm eq}=T_*\sqrt{\frac{R_*}{2a_{\rm orb}}}
(1-A_B)^{1/4}.
$$

For $T_*=5778\,\mathrm K$, $T_{\rm eq}=600\,\mathrm K$, and [Bond albedo](../../../exoplanet.md#bond-albedo) $A_B=0.5$,

$$
\frac{a_{\rm orb}}{R_*}
=\frac12\left(\frac{T_*}{T_{\rm eq}}\right)^2
\sqrt{1-A_B}\simeq32.8.
$$

Taking $R_p=R_{\rm Nep}=0.0354R_*$ gives

$$
\left(\frac{R_p}{a_{\rm orb}}\right)^2
\simeq1.17\times10^{-6}.
$$

The reported $50\,\mathrm{ppm}$ visible eclipse would therefore imply

$$
\boxed{A_g\simeq\frac{50\times10^{-6}}{1.17\times10^{-6}}simeq43},
$$

which is impossible. At least one assumption, the measurement, or the stated system parameters must fail; even $A_g=1$ gives only about $1.2\,\mathrm{ppm}$.

At $20\,\mu\mathrm m$, reflected light is negligible. The [thermal eclipse depth](../../../exoplanet.md#thermal-eclipse-depth) is

$$
\left(\frac{R_p}{R_*}\right)^2
\frac{e^{hc/(\lambda k_BT_*)}-1}
{e^{hc/(\lambda k_BT_p)}-1}.
$$

With $T_p=600\,\mathrm K$ this is

$$
\boxed{F_p/F_*\simeq7.2\times10^{-5}\simeq72\,\mathrm{ppm}}.
$$

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

A perfectly reflecting [Lambertian surface](../../../exoplanet.md#lambertian-surface) receiving normal flux $F$ has radiance

$$
I=\frac F\pi,
$$

because integrating $I\cos\theta$ over the outward hemisphere returns $F$. A face-on disc of radius $R$ subtends solid angle $\pi R^2/d^2$. The observed flux is consequently

$$
\boxed{F_{\rm obs}=I\frac{\pi R^2}{d^2}
=F\left(\frac Rd\right)^2}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $\tau_1$ and $\tau_2$ be the top-down optical depths at $P_1$ and $P_2$, and let $\mu$ be the outward direction cosine. The [formal solution of the radiative transfer equation](../../../astrophysics.md#formal-solution-of-the-radiative-transfer-equation) gives

$$
\boxed{
I_\nu(0,\mu)
=B_\nu(T_1)(1-e^{-\tau_1/\mu})
+B_\nu(T_2)(e^{-\tau_1/\mu}-e^{-\tau_2/\mu})
+I_{\nu,0}e^{-\tau_2/\mu}}.
$$

For a semi-infinite lower layer in [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium), $I_{\nu,0}=B_\nu(T_3)$.

Define

$$
E_3(x)=\int_0^1\mu e^{-x/\mu}\,d\mu.
$$

The emergent planetary surface flux is

$$
F_{p,\nu}=2\pi\left[
B_1\left(\frac12-E_3(\tau_1)\right)
+B_2(E_3(\tau_1)-E_3(\tau_2))
+B_3E_3(\tau_2)\right].
$$

Hence the band-centre planet-star ratio is

$$
\boxed{
\frac{F_p}{F_*}
=\left(\frac{R_p}{R_*}\right)^2
\frac{2[B_1(1/2-E_3(\tau_1))
+B_2(E_3(\tau_1)-E_3(\tau_2))+B_3E_3(\tau_2)]}
{B_\nu(T_*)}}.
$$

If $T_1=T_2=T_3=T_p$, the weights telescope to $1/2$, so $F_{p,\nu}=\pi B_\nu(T_p)$ and the expression reduces to the blackbody [thermal eclipse depth](../../../exoplanet.md#thermal-eclipse-depth), about $72\,\mathrm{ppm}$ for $T_p=600\,\mathrm K$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

At $20\,\mu\mathrm m$,

$$
E_3(0.1)=0.4163,
\qquad
E_3(1)=0.1097.
$$

The normalized flux weights of the $400$, $600$, and $800\,\mathrm K$ layers are therefore

$$
2(1/2-E_3(0.1))=0.1674,
$$



$$
2(E_3(0.1)-E_3(1))=0.6132,
\qquad
2E_3(1)=0.2194.
$$

Using the [Planck law](../../../statistical-physics.md#planck-s-law) at the band centre and $R_p/R_*=0.0354$ gives

$$
\boxed{F_p/F_*\simeq7.45\times10^{-5}simeq74.5\,\mathrm{ppm}}.
$$

This is only slightly larger than the $71.7\,\mathrm{ppm}$ isothermal $600\,\mathrm K$ value because the cool upper-layer suppression and hot deep-layer enhancement nearly cancel in this broad weighting.

## 3

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

In the [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum), the constant $a$ is the wavelength-independent reference transit depth, set mainly by the opaque planetary radius and any grey cloud deck. The Gaussian term can represent a resolved atomic or molecular absorption band centered at $\lambda_0$, with amplitude $b$ and width controlled by $\alpha$. The power-law term represents a continuum such as Rayleigh scattering or haze extinction; for Rayleigh scattering the opacity index is approximately $\gamma=-4$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Where the spectral components vanish, $a=(R_p/R_*)^2$, so

$$
\boxed{R_p=R_*\sqrt a}.
$$

For extinction cross-section $\sigma\propto\lambda^\gamma$, the [scattering slope of a transmission spectrum](../../../exoplanet.md#scattering-slope-of-a-transmission-spectrum) obeys

$$
\frac{dR_p}{d\log\lambda}=\gamma H,
\qquad
H=\frac{k_BT}{\bar m g}.
$$

Since $y=(R_p/R_*)^2$,

$$
H=\frac{R_*^2}{2R_p\gamma}
\frac{dy}{d\log\lambda}.
$$

After subtracting the Gaussian feature, the model gives $dy/d\log\lambda=\gamma c(\lambda/\lambda_1)^\gamma$. At $\lambda=\lambda_1$,

$$
\boxed{T
=\frac{\bar m g}{k_B}
\frac{cR_*^2}{2R_p}}
$$

or, with $g=GM_p/R_p^2$, $T=\bar m GM_pcR_*^2/(2k_BR_p^3)$. This estimates the mean isothermal terminator temperature under hydrostatic conditions.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

For a hot Jupiter transiting a Sun-sized star,

$$
a\simeq\left(\frac{R_J}{R_\odot}\right)^2\simeq0.010,
$$

a one-percent baseline transit. Taking $T\simeq1500\,\mathrm K$, $g\simeq20\,\mathrm{m\,s^{-2}}$, and an $\mathrm H_2$-dominated mean molecular mass $\bar m\simeq2.3m_H$ gives an [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) near $270\,\mathrm{km}$. A strong band spanning five scale heights then has

$$
b\sim\frac{2R_J(5H)}{R_\odot^2}
\sim4\times10^{-4},
$$

or several hundred parts per million; very strong clear-atmosphere features can approach $10^{-3}$. The spectrum is therefore a roughly one-percent baseline with a localized Gaussian-sized band near $\lambda_0$ and a continuum rising toward short wavelengths when $\gamma<0$. Clouds reduce both $b$ and the observable power-law slope.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

A deep ultraviolet transit and asymmetric light curve are signatures of an extended, escaping atmosphere rather than the optical planetary disc. Neutral hydrogen and ionized or neutral metals can form a comet-like tail, while interaction with the stellar wind can create an asymmetric bow shock.

For $R_*=0.5R_\odot$ and transit depth $D=0.5$, the absorbing radius is

$$
R_{\rm abs}=R_*\sqrt D
\simeq0.354R_\odot\simeq2.46\times10^8\,\mathrm m,
$$

about ten Neptune radii. This scale directly demonstrates that the ultraviolet absorber is gravitationally extended.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The [Jeans escape parameter](../../../exoplanet.md#jeans-escape-parameter) compares gravitational binding with thermal energy:

$$
\lambda(r)=\frac{GM_pm}{k_BTr}
=\frac{v_{\rm esc}^2}{2k_BT/m}.
$$

Hydrostatic thermal escape becomes strong when the Maxwellian tail is no longer exponentially small, roughly $\lambda\lesssim2$--$3$, and blow-off occurs for order-unity $\lambda$. Atomic hydrogen at an exobase radius $R_e$ therefore requires

$$
\boxed{T_e\gtrsim\frac{GM_pm_H}{k_BR_e}}
$$

for $\lambda\lesssim1$.

For a Neptune-mass planet this is about $3.4\times10^4\,\mathrm K$ at the optical radius $R_{\rm Nep}$. If the relevant base is the observed ultraviolet absorbing radius, approximately $10R_{\rm Nep}$, the corresponding value is about $3.4\times10^3\,\mathrm K$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

For $\lambda\gtrsim10$--$20$, escape is well described by the dilute high-velocity tail of a nearly hydrostatic exosphere. For $\lambda\lesssim2$--$3$, collisions couple the escaping gas into [hydrodynamic atmospheric escape](../../../exoplanet.md#hydrodynamic-escape); the intermediate regime requires a kinetic or transonic calculation.

The hydrostatic-tail estimate follows by integrating a Maxwell distribution over outward velocities exceeding escape speed. The [Jeans escape flux](../../../exoplanet.md#jeans-escape-flux) is

$$
\Phi_J=\frac{n_ev_{\rm th}}{2\sqrt\pi}(1+\lambda)e^{-\lambda},
\qquad
v_{\rm th}=\sqrt{\frac{2k_BT}{m}}.
$$

Therefore

$$
\boxed{\dot M_J
=4\pi R_e^2m\Phi_J
=4\pi R_e^2m\frac{n_ev_{\rm th}}{2\sqrt\pi}
(1+\lambda)e^{-\lambda}}.
$$

When $\lambda\leq1$, this is of order the free thermal supply $4\pi R_e^2\rho_ec_s$; quantitatively the flow is hydrodynamic and its conserved mass-loss rate is $\dot M=4\pi r^2\rho u$ through the transonic wind.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

Three nonthermal atmospheric-escape mechanisms are stellar-wind ion pickup, sputtering of neutrals by energetic incident particles, and photochemical escape in exothermic reactions. Charge exchange, polar-wind acceleration, and impact erosion provide further examples.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Three useful target classes are:

- temperate rocky Earth-size planets around late M dwarfs, such as TRAPPIST-1 e;
- temperate high-gravity super-Earths around small stars, such as LHS 1140 b;
- temperate hydrogen-rich sub-Neptunes, sometimes discussed as ocean-world or Hycean candidates, such as K2-18 b.

These examples are observing targets rather than assertions that any is inhabited. An Earth twin crossing a Sun twin has atmospheric transmission features near one part per million, a one-year orbital period, and only one transit per year. Stellar photon noise, instrumental stability, clouds, and the much brighter stellar spectrum make molecular detection exceptionally difficult for JWST.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

In transmission, the leading scaling is the [atmospheric spectral-feature amplitude](../../../exoplanet.md#atmospheric-spectral-feature-amplitude)

$$
\Delta D\sim\frac{2R_pN_HH}{R_*^2}.
$$

Observability therefore improves for a small bright host star, a large planet, low surface gravity, high atmospheric temperature, low mean molecular mass, large molecular abundance, and cloud-free limbs. Stellar activity and heterogeneity, refraction, aerosols, limited transit count, detector noise, and spectral overlap reduce it.

In emission, the contrast scales approximately as

$$
\left(\frac{R_p}{R_*}\right)^2
\frac{B_\lambda(T_p)}{B_\lambda(T_*)}.
$$

It depends on dayside temperature, vertical temperature gradient, molecular opacity, heat redistribution, orbital geometry, stellar brightness, and instrumental background.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

Assume a feature spans $N_H=5$ [atmospheric scale heights](../../../exoplanet.md#atmospheric-scale-height).

For an Earth twin around the Sun, $R_p=R_\oplus$, $R_*=R_\odot$, $H\simeq8\,\mathrm{km}$, giving

$$
\Delta D\sim1\,\mathrm{ppm}.
$$

For a $1.7R_\oplus$ super-Earth with a heavy atmosphere around a $0.2R_\odot$ M dwarf, take $H\simeq6\,\mathrm{km}$, giving

$$
\Delta D\sim30\,\mathrm{ppm}.
$$

For a $2.6R_\oplus$ hydrogen-rich sub-Neptune around a $0.4R_\odot$ star, take $T\simeq300\,\mathrm K$, $g\simeq12\,\mathrm{m\,s^{-2}}$, $\bar m=2.3m_H$, and hence $H\simeq90\,\mathrm{km}$. Then

$$
\Delta D\sim200\,\mathrm{ppm}.
$$

The hydrogen-rich sub-Neptune is the most observable with JWST because its low molecular mass and large radius produce the largest transmission annulus. Clouds can reverse this ranking in a particular system.

## 4

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The day-night contrast is controlled mainly by the ratio of radiative cooling time to horizontal advection and wave-adjustment times. A useful scaling is

$$
t_{\rm rad}\sim\frac{Pc_p}{g\,4\sigma T^3}.
$$

Stronger irradiation raises $T$ and sharply shortens $t_{\rm rad}$, allowing the dayside to reradiate before circulation reaches the nightside; the contrast therefore generally increases with irradiation. In ultra-hot atmospheres, hydrogen dissociation and recombination can transport latent heat and partly reduce it, while magnetic drag can weaken winds and increase it.

At low pressure, small atmospheric mass and short $t_{\rm rad}$ produce a large contrast. At greater pressure, the radiative time grows, waves and winds redistribute heat more effectively, and the contrast decreases. The observed contrast is wavelength dependent because each wavelength probes a different pressure.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Without scattering and in [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium), the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) has the emergent solution

$$
I_\nu(0,\mu)=\int_0^\infty
B_\nu[T(\tau_\nu)]e^{-\tau_\nu/\mu}
\frac{d\tau_\nu}{\mu}.
$$

The [Eddington-Barbier relation](../../../astrophysics.md#eddington-barbier-relation) gives the useful approximation

$$
I_\nu(0,\mu)\simeq B_\nu[T(\tau_\nu=\mu)].
$$

A molecular band has larger opacity than its neighboring continuum and therefore reaches optical depth unity at lower pressure.

If temperature decreases outward, the band samples cooler gas and appears in absorption. If the atmosphere is isothermal, both levels have the same source function and the feature disappears. If an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) makes the upper layer hotter, the band appears in emission. For a weak separation of formation pressures,

$$
\Delta I_\nu\simeq
\frac{\partial B_\nu}{\partial T}
\frac{dT}{d\log P}\Delta\log P,
$$

which explicitly shows that feature sign and amplitude measure the vertical temperature gradient.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Three important atmospheric chemical processes are:

- thermochemical equilibrium in hot, dense layers, for example conversion between CO and methane according to local temperature and pressure;
- vertical or horizontal transport followed by chemical quenching, which can preserve CO or methane at abundances inherited from deeper levels;
- ultraviolet photochemistry in the upper atmosphere, which can produce HCN, complex hydrocarbons, and haze from methane-bearing gas.

Condensation and rainout provide another major process, removing species such as silicates or water from the gas phase where their saturation curves are crossed.

A solid or liquid surface supplies reservoirs and sinks through weathering, dissolution, volcanism, deposition, and possible biological cycling; it also caps the atmospheric mass. A surface-free sub-Neptune instead has a deep envelope merging continuously into high-pressure volatile or hydrogen-rich layers, with composition governed more by bulk elemental inventory, mixing, and deep thermochemistry.

At Earth-like equilibrium temperature, a sub-Neptune can retain methane, ammonia, and water in a hydrogen-rich atmosphere, subject to photochemistry and condensation. A hot Jupiter is hotter, usually hydrogen dominated, and more strongly driven toward CO, water, and nitrogen at depth; at extreme irradiation molecules dissociate and atomic, ionic, and negative-hydrogen opacity become important.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The mass fractions of the $10M_\oplus$ planet are

$$
\boxed{x_{\rm iron}=0.4,
\qquad x_{\rm silicate}=0.4,
\qquad x_{\rm H_2}=0.2}.
$$

On an [exoplanet bulk-composition ternary diagram](../../../exoplanet.md#exoplanet-bulk-composition-ternary-diagram) with iron, silicate, and hydrogen vertices, it lies in the interior on the line of equal iron and silicate fractions, one fifth of the way from the iron-silicate edge toward the hydrogen vertex.

Neglecting its atmosphere and minor volatile reservoirs, Earth lies on the iron-silicate edge at approximately

$$
\boxed{(x_{\rm iron},x_{\rm silicate},x_{\rm H_2})simeq(0.32,0.68,0)}.
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Consider a ray bundle from projected source area $dA_s\cos\theta_s$ into solid angle $d\Omega_s$. In empty space its power is conserved, while geometric propagation preserves the étendue

$$
dA_s\cos\theta_s\,d\Omega_s
=dA_o\cos\theta_o\,d\Omega_o.
$$

Since [specific intensity](../../../astrophysics.md#specific-intensity) is power divided by this étendue and by frequency interval,

$$
\boxed{I_\nu/\nu^3=\text{constant along a ray}}.
$$

In a static medium with no redshift, frequency is unchanged and $I_\nu$ itself is independent of distance. The apparent solid angle shrinks as distance squared while the physical beam area grows by the same factor.

For a full plane-parallel angular field linear in direction cosine,

$$
I(\mu)=I_0+I_1\mu,
$$

the [radiation-field moments](../../../astrophysics.md#radiation-field-moment) are

$$
\boxed{J=I_0,
\qquad H=\frac{I_1}{3},
\qquad K=\frac{I_0}{3}=\frac J3},
$$

and $F=4\pi H=4\pi I_1/3$. At a surface with no incoming intensity and the same law only for $0<\mu<1$,

$$
J=\frac{I_0}{2}+\frac{I_1}{4},
\quad
F=\pi I_0+\frac{2\pi I_1}{3},
\quad
K=\frac{I_0}{6}+\frac{I_1}{8}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
