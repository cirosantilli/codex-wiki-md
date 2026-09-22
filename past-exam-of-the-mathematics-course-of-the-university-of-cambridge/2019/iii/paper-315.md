# Paper 315

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_315.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_315.pdf)

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

Assume a uniform stellar disc of radius $R_\star$, an opaque planetary radius $R_p$, and a thin atmospheric annulus of thickness $z\ll R_p$. Neglect planetary light during transit and scattering back into the beam. The attenuation part of the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) gives $I_\lambda=I_{\lambda,0}e^{-\tau_\lambda}$, where $\tau_\lambda$ is the slant [optical depth](../../../astrophysics.md#optical-depth) along a stellar ray through the atmosphere. The fraction of light removed from that annulus is therefore $1-e^{-\tau_\lambda}$.

If the annulus is represented by one effective [optical depth](../../../astrophysics.md#optical-depth), its area divided by the stellar area is

$$
A=\frac{\pi[(R_p+z)^2-R_p^2]}{\pi R_\star^2}\simeq\frac{2R_pz}{R_\star^2}.
$$

The [annulus model for transmission spectroscopy](../../../exoplanet.md#annulus-model-for-transmission-spectroscopy) consequently gives the extra transit depth

$$
\boxed{\delta_\lambda=A(1-e^{-\tau_\lambda}).}
$$

Here $\delta_\lambda$ is normalized to the unobscured stellar flux and excludes the opaque-disc depth $(R_p/R_\star)^2$. For a spectral feature measured relative to a continuum with slant [optical depth](../../../astrophysics.md#optical-depth) $\tau_c$, the corresponding contrast is $A(e^{-\tau_c}-e^{-\tau_\lambda})$; the displayed formula takes the annular continuum to be transparent.

A real [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) has an impact-parameter-dependent [optical depth](../../../astrophysics.md#optical-depth). Its more accurate expression is

$$
\delta_\lambda=\frac2{R_\star^2}\int_{R_p}^{\infty}b\,[1-e^{-\tau_\lambda(b)}],db.
$$

Stellar limb darkening and horizontally varying clouds further modify the weighting. The single-annulus approximation is useful for estimating an [atmospheric spectral-feature amplitude](../../../exoplanet.md#atmospheric-spectral-feature-amplitude), rather than predicting every spectral line.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At 10 parsecs, $0.01$ arcseconds corresponds to $a=0.10$ astronomical units. Take a solar-radius star with $T_\star=5772\,\mathrm K$, zero [Bond albedo](../../../exoplanet.md#bond-albedo), full [day-night heat redistribution](../../../exoplanet.md#day-night-heat-redistribution), negligible internal heating, and a hydrogen-helium atmosphere with mean particle mass $2.3m_H$. The [planetary equilibrium temperature](../../../exoplanet.md#planetary-equilibrium-temperature) is

$$
T_p=T_\star\sqrt{\frac{R_\star}{2a}}\simeq880\,\mathrm K.
$$

For [Jupiter](../../../planetary-science.md#jupiter) mass and radius, $g\simeq24.8\,\mathrm{m\,s^{-2}}$. Its [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) is

$$
H=\frac{k_BT_p}{2.3m_Hg}\simeq1.27\times10^5\,\mathrm m.
$$

Assume a strong band spans $N_H=5$ [atmospheric scale heights](../../../exoplanet.md#atmospheric-scale-height) and saturates in the [annulus model for transmission spectroscopy](../../../exoplanet.md#annulus-model-for-transmission-spectroscopy). The [atmospheric spectral-feature amplitude](../../../exoplanet.md#atmospheric-spectral-feature-amplitude) is

$$
\delta_{\rm tr}\simeq\frac{2R_pN_HH}{R_\star^2}\simeq1.88\times10^{-4}=188\,\mathrm{ppm}.
$$

For a five-standard-deviation detection, the uncertainty of the measured differential contrast must satisfy

$$
\boxed{\sigma_{\rm tr}\lesssim38\,\mathrm{ppm}.}
$$

This estimate scales linearly with the assumed feature height; one [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height) would require about $7.5\,\mathrm{ppm}$. The question gives no opacity or abundance from which to fix $N_H$, so an atmospheric detection threshold is necessarily assumption-dependent.

For thermal emission at $10\,\mu\mathrm m$, assume the planet and star emit as [blackbodies](../../../astrophysics.md#blackbody). The [thermal eclipse depth](../../../exoplanet.md#thermal-eclipse-depth) from the [Planck law](../../../statistical-physics.md#planck-s-law) is

$$
\frac{F_p}{F_\star}=\left(\frac{R_p}{R_\star}\right)^2
\frac{e^{hc/(\lambda k_BT_\star)}-1}{e^{hc/(\lambda k_BT_p)}-1}
\simeq7.24\times10^{-4}=724\,\mathrm{ppm}.
$$

Thus the uncertainty required for a five-standard-deviation [exoplanet secondary eclipse](../../../exoplanet.md#exoplanet-secondary-eclipse) detection is

$$
\boxed{\sigma_{\rm em}\lesssim145\,\mathrm{ppm}.}
$$

These are uncertainties of the final transit or eclipse contrasts, including the uncertainty of their reference levels. The distance affects photon counts and observing time but cancels from the flux ratios. An opaque exactly isothermal atmosphere emits a featureless [blackbody](../../../astrophysics.md#blackbody) spectrum: an eclipse detects its thermal light, while identifying atmospheric composition requires spectral features and a nonisothermal structure or other diagnostics.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

In the [annulus model for transmission spectroscopy](../../../exoplanet.md#annulus-model-for-transmission-spectroscopy), an added aerosol [optical depth](../../../astrophysics.md#optical-depth) changes the signal to $A[1-e^{-(\tau_{\rm gas}+\tau_{\rm aerosol})}]$. Large particles can supply nearly wavelength-independent extinction. An opaque high [exoplanet cloud deck](../../../exoplanet.md#exoplanet-cloud-deck) then masks deeper gas, flattens the optical [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum), and weakens atomic or molecular features.

Small particles can instead produce a rising transit radius toward short wavelengths. In an isothermal atmosphere, the [slant optical depth of an isothermal atmosphere](../../../exoplanet.md#slant-optical-depth-of-an-isothermal-atmosphere) is

$$
\tau_\lambda(z)\simeq\sigma_\lambda n_0e^{-z/H}\sqrt{2\pi R_pH}.
$$

Taking the effective radius near $\tau_\lambda\sim1$ gives $z(\lambda)=H\log\sigma_\lambda+\mathrm{constant}$. For [Rayleigh scattering](../../../electromagnetism.md#rayleigh-scattering), $\sigma_\lambda\propto\lambda^{-4}$, so the [scattering slope of a transmission spectrum](../../../exoplanet.md#scattering-slope-of-a-transmission-spectrum) is

$$
\boxed{\frac{dR_p}{d\log\lambda}=-4H.}
$$

A steeper-than-expected optical slope or suppressed gas features can therefore indicate [atmospheric haze](../../../exoplanet.md#haze) or [exoplanet clouds](../../../exoplanet.md#exoplanet-cloud). These signatures are not unique: high mean molecular mass reduces $H$, gas itself can produce [Rayleigh scattering](../../../electromagnetism.md#rayleigh-scattering), and stellar surface heterogeneity can mimic slopes. Consistent optical and infrared features help distinguish these explanations.

## 2

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium), negligible scattering of thermal radiation, and a plane-parallel atmosphere. With inward [optical depth](../../../astrophysics.md#optical-depth) $\tau_\lambda$ and outward ray cosine $\mu$, the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) is

$$
\mu\frac{dI_\lambda}{d\tau_\lambda}=I_\lambda-B_\lambda[T(\tau_\lambda)].
$$

For a deep atmosphere, its [formal solution of the radiative transfer equation](../../../astrophysics.md#formal-solution-of-the-radiative-transfer-equation) is

$$
I_\lambda(0,\mu)=\int_0^\infty B_\lambda[T(t)]e^{-t/\mu}\frac{dt}{\mu}.
$$

The weighting samples $\tau_\lambda$ of order unity. The [Eddington-Barbier relation](../../../astrophysics.md#eddington-barbier-relation) makes this precise when the source function is nearly linear: $I_\lambda(0,\mu)\simeq B_\lambda[T(\tau_\lambda=\mu)]$.

A molecular band with greater [opacity](../../../stellar-structure.md#opacity) reaches unit [optical depth](../../../astrophysics.md#optical-depth) higher than the nearby continuum. If [temperature](../../../thermodynamics.md#temperature) decreases upward, that band samples cooler gas and appears in absorption. If an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) makes the upper gas hotter, the band appears in emission. If both depths have the same [temperature](../../../thermodynamics.md#temperature), an opaque isothermal atmosphere has

$$
\boxed{I_\lambda=B_\lambda(T),}
$$

and no opacity-dependent features. This last conclusion assumes all wavelengths are opaque or the lower boundary emits the same [Planck function](../../../astrophysics.md#planck-function); an optically thin isothermal layer over a different background need not be featureless.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $a\gg a_{AB}$, both stars illuminate the [circumbinary planet](../../../exoplanet.md#circumbinary-planet) at approximately distance $a$. Treat them as [blackbodies](../../../astrophysics.md#blackbody), neglect internal heating, and assume [Bond albedo](../../../exoplanet.md#bond-albedo) $A_B$ and uniform global reradiation. The absorbed and emitted powers are

$$
\pi R_p^2(1-A_B)\sigma_{\rm SB}\frac{R_A^2T_A^4+R_B^2T_B^4}{a^2}
=4\pi R_p^2\sigma_{\rm SB}T_p^4.
$$

Thus the [equilibrium temperature of a circumbinary planet](../../../exoplanet.md#equilibrium-temperature-of-a-circumbinary-planet) is

$$
\boxed{T_p=\left[\frac{1-A_B}{4a^2}(R_A^2T_A^4+R_B^2T_B^4)\right]^{1/4}.}
$$

For an example, take $R_A=R_\odot$, $R_B=0.3R_\odot$, $T_A=6000\,\mathrm K$, $T_B=3000\,\mathrm K$, $a=1\,\mathrm{au}$, $a_{AB}=0.05\,\mathrm{au}$, circular coplanar orbits, and $A_B=0$. Then

$$
\boxed{T_p\simeq290\,\mathrm K.}
$$

The cooler star contributes only $0.3^2(3000/6000)^4\simeq0.0056$ of the hotter star's luminosity in this example.

An opaque isothermal atmosphere emits $F_\lambda=\pi B_\lambda(T_p)$, with no absorption or emission bands. The [Wien displacement law](../../../astrophysics.md#wien-s-displacement-law) puts the maximum of this wavelength spectrum near $\lambda_{\rm max}\simeq10\,\mu\mathrm m$. At observer distance $d$, the planetary spectral flux is $\pi B_\lambda(T_p)(R_p/d)^2$.

<a id="2/b/image-isothermal-circumbinary-planet-emission-spectrum"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-315-isothermal-spectrum.png)

**[Figure 1](#2/b/image-isothermal-circumbinary-planet-emission-spectrum). Isothermal circumbinary-planet emission spectrum**. The emergent surface flux for the example above. The wavelength spectrum peaks near ten micrometres; the exactly isothermal opaque model has no molecular bands.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Assume all three planets retain approximately their original hydrogen-helium bulk composition. Stellar encounters change orbital energy and irradiation, not automatically the planet's elemental abundances. Their atmospheric structures can become approximately stationary long before their interiors finish cooling.

For the unperturbed [Jupiter](../../../planetary-science.md#jupiter)-like planet at $a\simeq5.2\,\mathrm{au}$, the zero-albedo globally averaged [planetary equilibrium temperature](../../../exoplanet.md#planetary-equilibrium-temperature) is about $122\,\mathrm K$. Stellar light heats the outer atmosphere, while internal cooling supports a deeper temperature gradient and convection. At cooler pressures, [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) favors methane and ammonia; condensate clouds can include ammonia at high levels and water deeper down. [Disequilibrium chemistry in an exoplanet atmosphere](../../../exoplanet.md#disequilibrium-chemistry-in-an-exoplanet-atmosphere) can preserve carbon monoxide or other species from deeper layers.

For the inward-migrated planet at $a\simeq0.052\,\mathrm{au}$, the irradiation-only [planetary equilibrium temperature](../../../exoplanet.md#planetary-equilibrium-temperature) is ten times higher, about $1220\,\mathrm K$, because $T_{\rm eq}\propto a^{-1/2}$. Its [irradiated planetary atmosphere](../../../exoplanet.md#irradiated-planetary-atmosphere) has a heated radiative exterior, potentially strong day-night differences, and a deep [radiative-convective boundary](../../../exoplanet.md#radiative-convective-boundary). At suitable pressures, [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) increasingly favors carbon monoxide over methane; water remains important, while alkali absorption and high-temperature condensates can matter. An [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) depends on absorbers, clouds, and irradiation and is not guaranteed simply by migration.

The ejected object is a [rogue planet](../../../planetary-science.md#rogue-planet). Its irradiation-based [planetary equilibrium temperature](../../../exoplanet.md#planetary-equilibrium-temperature) becomes very small, but its actual emitting [temperature](../../../thermodynamics.md#temperature) is set primarily by internal cooling and [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism). After only several million years it can remain warm and self-luminous, with deep convection and an outward-cooling radiative atmosphere. Its photospheric chemistry and clouds depend on that cooling temperature; they cannot be inferred from the absence of a host star alone. None of these cases fixes an exact pressure-temperature profile without a cooling model, opacities, and atmospheric composition.

## 3

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a spherical planet, combine the [hydrostatic pressure support equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) with $dm/dr=4\pi r^2\rho$:

$$
\frac{dP}{dm}=-\frac{Gm}{4\pi r^4}.
$$

Neglect surface [pressure](../../../thermodynamics.md#pressure). Since $r(m)\le R$, the [hydrostatic lower bound on planetary central pressure](../../../exoplanet.md#hydrostatic-lower-bound-on-planetary-central-pressure) is

$$
\boxed{P_c=\int_0^M\frac{Gm}{4\pi r(m)^4}\,dm\ge\frac{GM^2}{8\pi R^4}.}
$$

For a physically usual [mass density](../../../fluid-mechanics.md#density) decreasing outward, the mean interior density exceeds the global mean. Hence $r(m)\le R(m/M)^{1/3}$, giving the sharper minimum within this class,

$$
\boxed{P_c\ge\frac{3GM^2}{8\pi R^4}.}
$$

Uniform [mass density](../../../fluid-mechanics.md#density) attains the sharper bound; direct integration with $m(r)=Mr^3/R^3$ gives $P_c=3GM^2/(8\pi R^4)$. Real planets are centrally concentrated through compression and dense cores, so their central [pressure](../../../thermodynamics.md#pressure) is higher.

Using $M_\oplus=5.97\times10^{24}\,\mathrm{kg}$, $R_\oplus=6.37\times10^6\,\mathrm m$, $M_J=1.90\times10^{27}\,\mathrm{kg}$, and $R_J=7.15\times10^7\,\mathrm m$, the universal bounds are approximately $5.75\times10^{10}\,\mathrm{Pa}$ for [Earth](../../../planetary-science.md#earth) and $3.66\times10^{11}\,\mathrm{Pa}$ for [Jupiter](../../../planetary-science.md#jupiter). The uniform-density estimates are respectively $1.72\times10^{11}\,\mathrm{Pa}$ and $1.10\times10^{12}\,\mathrm{Pa}$, or $1.72$ and $11.0$ megabars. Either comparison gives **a Jupiter minimum about 6.4 times the Earth minimum**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

At $10\,\mathrm{au}$ from a four-solar-luminosity star, the incident flux is proportional to $4/10^2=1/25$, approximately the same as for [Jupiter](../../../planetary-science.md#jupiter) at $5\,\mathrm{au}$ around the Sun. Thus [Jupiter](../../../planetary-science.md#jupiter) supplies a possible old comparison at roughly the same mass and irradiation.

Assume the radius law holds from the young epoch to an old age of $4.5\,\mathrm{Gyr}$, that the irradiation history can be represented by the same fixed value, and that the present old radius is $R_J$. If $t$ is approximated by stellar age, then

$$
\frac{2R_J}{R_J}=\left(\frac{5\,\mathrm{Myr}}{4500\,\mathrm{Myr}}\right)^{-\alpha},
\qquad
\boxed{\alpha=\frac{\log2}{\log900}\simeq0.102.}
$$

If $t$ instead starts at completion of formation, the model's formation delay of up to $3\,\mathrm{Myr}$ leaves the young planet with thermal age between $2$ and $5\,\mathrm{Myr}$. Taking the old thermal age as approximately $4500\,\mathrm{Myr}$ then gives $\alpha\simeq0.090$–$0.102$.

Thus **an exponent of order 0.1** is a reasonable conditional estimate. A single radius at one age cannot determine both the exponent and normalization of a power law; the old [Jupiter](../../../planetary-science.md#jupiter) comparison and the assumptions about formation time and irradiation are essential.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[Exoplanet transit photometry](../../../exoplanet.md#exoplanet-transit-photometry) discovers a giant planet through a periodic flux decrement and measures $R_p/R_\star\simeq\sqrt{\delta}$. Stellar-radius estimates turn this into a planetary radius. The [radial-velocity method](../../../exoplanet.md#doppler-spectroscopy) discovers the stellar orbital reflex motion and constrains $M_p\sin i$. Follow-up [exoplanet transit photometry](../../../exoplanet.md#exoplanet-transit-photometry) is required to measure a geometric radius when such a planet also transits; a radial-velocity detection alone gives no direct size. Alternatively, [exoplanet direct imaging](../../../exoplanet.md#exoplanet-direct-imaging) finds young luminous giants, whose sizes are inferred less directly from luminosity, [temperature](../../../thermodynamics.md#temperature), distance, and a [planetary mass-radius relation](../../../exoplanet.md#planetary-mass-radius-relation) or atmosphere model.

The two broad explanations for [hot-Jupiter radius inflation](../../../exoplanet.md#hot-jupiter-radius-inflation) are retention of primordial heat and addition of new interior power.

[Delayed cooling of an inflated giant planet](../../../exoplanet.md#delayed-cooling-of-an-inflated-giant-planet) can arise from enhanced atmospheric [opacity](../../../stellar-structure.md#opacity), which slows radiative escape; an irradiation-maintained radiative blanket, which insulates the convective interior; or compositional stratification and inefficient [layered convection](../../../fluid-mechanics.md#layered-convection), which inhibit the outward transport of heat. These alter the rate of [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism).

[Heating of an inflated giant planet](../../../exoplanet.md#heating-of-an-inflated-giant-planet) can arise from [tidal heating](../../../planetary-science.md#tidal-heating) maintained by eccentricity or obliquity; [Joule heating](../../../electromagnetism.md#joule-heating) of currents driven by atmospheric winds through a [magnetic field](../../../electromagnetism.md#magnetic-field); or downward transport and dissipation of atmospheric mechanical energy generated by irradiation. To affect radius, the energy must be deposited at a depth and rate that changes the interior cooling balance. Simply absorbing starlight high in the atmosphere does not automatically supply deep heating. These are proposed mechanisms with different efficiencies, not six universally established contributions in every inflated planet.

## 4

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A close-in giant is often in [synchronous rotation](../../../planetary-science.md#synchronous-rotation) after [tidal locking](../../../planetary-science.md#tidal-locking), giving persistent dayside heating and nightside cooling. Its contrast is controlled by the competition between [radiative relaxation time in a planetary atmosphere](../../../exoplanet.md#radiative-relaxation-time-in-a-planetary-atmosphere), wind transport characterized by the [atmospheric advection time](../../../exoplanet.md#atmospheric-advection-time), wave adjustment, and drag. When heat transport is fast compared with radiation, [day-night heat redistribution](../../../exoplanet.md#day-night-heat-redistribution) lowers the contrast; when radiation is fast, each hemisphere stays closer to its local radiative balance.

For a rough atmospheric column estimate,

$$
\tau_{\rm rad}\sim\frac{c_pp}{4g\sigma_{\rm SB}T^3},\qquad
\tau_{\rm adv}\sim\frac{R_p}{U}.
$$

At comparable [pressure](../../../thermodynamics.md#pressure), higher [planetary equilibrium temperature](../../../exoplanet.md#planetary-equilibrium-temperature) sharply shortens radiative relaxation, tending to increase the day-night contrast. Wind speeds, rotation, and magnetic drag can modify this trend; dissociation and recombination can carry additional heat in very hot atmospheres.

At higher altitude, lower [pressure](../../../thermodynamics.md#pressure) generally means shorter radiative relaxation and a larger contrast. Infrared bands with larger [opacity](../../../stellar-structure.md#opacity) probe these higher layers, while lower-opacity windows sample deeper layers with longer cooling times and more effective redistribution. A wavelength-dependent [exoplanet thermal phase curve](../../../exoplanet.md#exoplanet-thermal-phase-curve) can therefore reveal how the contrast and hot-region displacement change with pressure.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $L_J$ be [Jupiter](../../../planetary-science.md#jupiter)'s current total emitted luminosity. Under the stipulated split, its intrinsic luminosity after removal of sunlight is approximately $L_J/2$. If the accessible energy reservoir down to $T_{\rm cold}$ is $E_J$, the constant-luminosity estimate gives $\tau\simeq E_J/(L_J/2)$.

Assume the more massive giant has approximately the same radius as [Jupiter](../../../planetary-science.md#jupiter), a comparable structure factor, and an accessible cooling reservoir scaling as $GM^2/R$, as in the [Kelvin-Helmholtz cooling time](../../../stellar-astrophysics.md#kelvin-helmholtz-cooling-time). Assume also that the final cold state contributes negligibly to that reservoir and that the giant radiates at the constant stipulated luminosity $L_J$. Then

$$
E_{10}\simeq100E_J,\qquad
\tau_{10}\simeq\frac{100E_J}{L_J}.
$$

Therefore

$$
\boxed{\tau_{10}\simeq50\tau.}
$$

This is a characteristic scaling under the stated assumptions, not a detailed evolutionary age. A different mass-radius relation, a different accessible internal-energy fraction, or time-dependent luminosity changes the result; the mass and luminosity alone do not uniquely determine a cooling time.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $F_{\rm abs}=\sigma_{\rm SB}T_{\rm eq}^4$ be the globally averaged absorbed stellar flux. The [single-layer greenhouse model](../../../exoplanet.md#single-layer-greenhouse-model) has an atmosphere transparent to incoming visible light and with infrared absorptivity and emissivity $\alpha$. Treat the surface as a [blackbody](../../../astrophysics.md#blackbody) and neglect internal heating. The layer emits $\alpha\sigma_{\rm SB}T_a^4$ both upward and downward.

Atmospheric radiative balance gives

$$
\alpha\sigma_{\rm SB}T_s^4=2\alpha\sigma_{\rm SB}T_a^4,
\qquad T_a^4=T_s^4/2\quad(\alpha>0).
$$

Surface radiative balance gives

$$
\sigma_{\rm SB}T_s^4=\sigma_{\rm SB}T_{\rm eq}^4+\alpha\sigma_{\rm SB}T_a^4.
$$

Eliminating $T_a$ yields

$$
\boxed{T_s=T_{\rm eq}\left(1-\frac\alpha2\right)^{-1/4}.}
$$

The transparent limit has $T_s=T_{\rm eq}$, and a fully infrared-opaque layer has $T_s=2^{1/4}T_{\rm eq}$. The model omits convection, wavelength-dependent opacity, and atmospheric absorption of starlight, so it captures the simplest greenhouse energy balance rather than a full surface-temperature prediction.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Assume a hydrogen-helium [perfect gas](../../../thermodynamics.md#ideal-gas) with mean particle mass $2.3m_H$, [Jupiter](../../../planetary-science.md#jupiter) gravity $g\simeq24.8\,\mathrm{m\,s^{-2}}$, and mixing over one [atmospheric scale height](../../../exoplanet.md#atmospheric-scale-height). At $T=1000\,\mathrm K$,

$$
H=\frac{k_BT}{2.3m_Hg}\simeq1.45\times10^5\,\mathrm m.
$$

The [eddy mixing time](../../../exoplanet.md#eddy-mixing-time) is $\tau_{\rm mix}\simeq H^2/K_{zz}$. A [chemical quench level](../../../exoplanet.md#chemical-quench-level) at one bar requires $\tau_{\rm mix}\lesssim\tau_{\rm chem}=10^5\,\mathrm s$, hence the [vertical eddy diffusion coefficient](../../../exoplanet.md#vertical-eddy-diffusion-coefficient) must be of order

$$
\boxed{K_{zz}\gtrsim2.1\times10^5\,\mathrm{m^2\,s^{-1}}=2.1\times10^9\,\mathrm{cm^2\,s^{-1}}.}
$$

The number depends quadratically on the assumed mixing length; using a fraction of $H$ reduces it accordingly.

Above the [chemical quench level](../../../exoplanet.md#chemical-quench-level), neglect photochemistry, condensation, and molecular diffusion. The [quenched atmospheric mixing ratio](../../../exoplanet.md#quenched-atmospheric-mixing-ratio) $f_A=n_A/n$ is approximately constant, while the [number density](../../../statistical-physics.md#number-density) is

$$
\boxed{n_A(z)=f_A\frac{p_q}{k_BT}e^{-(z-z_q)/H}.}
$$

Thus the abundance fraction is frozen, but the absolute [number density](../../../statistical-physics.md#number-density) falls with [pressure](../../../thermodynamics.md#pressure) and altitude. Examples are [carbon monoxide–methane quenching](../../../exoplanet.md#carbon-monoxide-methane-quenching), through $\mathrm{CO}+3\mathrm H_2\rightleftharpoons\mathrm{CH}_4+\mathrm H_2\mathrm O$, and [nitrogen–ammonia quenching](../../../exoplanet.md#nitrogen-ammonia-quenching), through $\mathrm N_2+3\mathrm H_2\rightleftharpoons2\mathrm{NH}_3$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

First refine the ephemeris, planetary mass, stellar radius, and stellar variability using [exoplanet transit photometry](../../../exoplanet.md#exoplanet-transit-photometry) and the [radial-velocity method](../../../exoplanet.md#doppler-spectroscopy). Then combine observations that probe different regions rather than relying on one spectrum. A present-day programme could use the following complementary measurements; in the 2019 setting of the paper, [James Webb Space Telescope](../../../exoplanet.md#james-webb-space-telescope) observations would have been a future capability.

- [Exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) at roughly $0.3$–$1\,\mu\mathrm m$ with the [Hubble Space Telescope](../../../exoplanet.md#hubble-space-telescope) or optical ground-based spectroscopy: constrain [exoplanet clouds](../../../exoplanet.md#exoplanet-cloud), [atmospheric haze](../../../exoplanet.md#haze), the [scattering slope of a transmission spectrum](../../../exoplanet.md#scattering-slope-of-a-transmission-spectrum), and sodium or potassium absorption.
- Near-infrared [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) with [NIRISS](../../../exoplanet.md#near-infrared-imager-and-slitless-spectrograph) at $0.6$–$2.8\,\mu\mathrm m$ and [NIRSpec](../../../exoplanet.md#nirspec) modes covering roughly $1$–$5\,\mu\mathrm m$: measure water, carbon monoxide, carbon dioxide, and methane bands, then constrain [atmospheric metallicity of a giant planet](../../../exoplanet.md#atmospheric-metallicity-of-a-giant-planet) and [atmospheric carbon-to-oxygen ratio](../../../exoplanet.md#atmospheric-carbon-to-oxygen-ratio) through a joint atmosphere model.
- [Exoplanet secondary eclipses](../../../exoplanet.md#exoplanet-secondary-eclipse) at near- and mid-infrared wavelengths with [NIRSpec](../../../exoplanet.md#nirspec) and [MIRI](../../../exoplanet.md#mid-infrared-instrument), especially about $5$–$12\,\mu\mathrm m$ for the latter's time-series low-resolution mode: infer [brightness temperatures](../../../exoplanet.md#brightness-temperature), the vertical pressure-temperature structure, and whether an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) turns bands into emission.
- A full-orbit [exoplanet thermal phase curve](../../../exoplanet.md#exoplanet-thermal-phase-curve) in one or more infrared bands with the [James Webb Space Telescope](../../../exoplanet.md#james-webb-space-telescope): constrain [day-night heat redistribution](../../../exoplanet.md#day-night-heat-redistribution), nightside emission, and the offset of the hottest region, with different bands probing different pressures.
- High-resolution near-infrared spectroscopy around molecular bands such as carbon monoxide near $2.3\,\mu\mathrm m$ using [CRIRES](../../../exoplanet.md#crires) on the [Very Large Telescope](../../../exoplanet.md#very-large-telescope): resolve the planetary [Doppler shift](../../../physics.md#doppler-effect) and seek wind velocities or rotation broadening after accounting for the orbital velocity.
- Ultraviolet transit spectroscopy with the [Hubble Space Telescope](../../../exoplanet.md#hubble-space-telescope), or ground-based near-infrared helium spectroscopy at $1.083\,\mu\mathrm m$: search for [atmospheric escape](../../../exoplanet.md#atmospheric-escape) and an extended upper atmosphere.

Together these address aerosols, molecular composition, elemental enrichment, vertical thermal structure, horizontal heat transport, winds, and escape. Repeat key events and monitor stellar activity, since stellar contamination and instrumental trends can imitate atmospheric signals. Use actual brightness, saturation limits, and predicted feature amplitudes to choose observing modes and exposure times.

The wavelength ranges and time-series capabilities are documented in the [NIRISS SOSS guide](https://jwst-docs.stsci.edu/jwst-near-infrared-imager-and-slitless-spectrograph/niriss-observing-modes/niriss-single-object-slitless-spectroscopy), [NIRSpec overview](https://science.nasa.gov/mission/webb/nirspec/), [MIRI spectroscopy guide](https://jwst-docs.stsci.edu/jwst-mid-infrared-instrument/miri-observing-modes/miri-low-resolution-spectroscopy), and [ESO's CRIRES description](https://www.eso.org/public/teles-instr/paranal-observatory/vlt/vlt-instr/crires%2B/).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
