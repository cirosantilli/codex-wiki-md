<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A stable sinusoidal [radial-velocity semi-amplitude](../../../../radial-velocity-semi-amplitude.md) can be stellar reflex motion caused by a companion on a nearly [circular orbit](../../../../circular-orbit.md). The amplitude is compatible with a giant [planet](../../../../planet.md); a low-[mass](../../../../mass.md) [star](../../../../star.md) or [brown dwarf](../../../../brown-dwarf.md) viewed nearly face-on can mimic the same projected motion, but requires an increasingly unlikely orientation. [Starspots](../../../../starspot.md) and magnetically suppressed [convection](../../../../convection-split.md) can produce a rotational [stellar activity](../../../../stellar-activity.md) signal on a ten-day timescale; contemporaneous photometry, activity indicators and [stellar spectral-line bisector](../../../../stellar-spectral-line-bisector.md) and other profile changes distinguish these from a clean common Doppler shift. Solar-like [stellar oscillations](../../../../stellar-oscillation.md) ordinarily have much shorter periods, so a coherent ten-day oscillation of an otherwise ordinary solar-type dwarf is less plausible. Instrumental drift, sampling aliases and blended spectra also need checking. A sinusoid alone does not establish a planetary origin, and the data do not assign numerical probabilities to these alternatives.

For the [minimum companion mass from radial velocity](../../../../minimum-companion-mass-from-radial-velocity.md), take a circular two-body orbit and initially $M_\star=M_\odot$. The exact relation and its low-[mass](../../../../mass.md) limit are

$$
K=\left(\frac{2\pi G}{P}\right)^{1/3}\frac{M_p\sin i}{(M_\star+M_p)^{2/3}},\qquad M_p\sin i\simeq K\left(\frac P{2\pi G}\right)^{1/3}M_\star^{2/3}.
$$

With $\sin i=1$,

$$
\boxed{M_{p,\min}\simeq0.636\,M_J\simeq202\,M_\oplus,\qquad a\simeq0.0908\,\mathrm{au}.}
$$

Here $a=[GM_\star P^2/(4\pi^2)]^{1/3}$ is the relative orbital [semi-major axis](../../../../semi-major-axis.md). Nonzero [orbital eccentricity](../../../../orbital-eccentricity.md) multiplies the inferred $M_p\sin i$ by $\sqrt{1-e^2}$ at fixed measured $K,P$, but the sinusoidal model motivates $e=0$ here.

For the [radial-velocity sensitivity limit at fixed planet mass](../../../../radial-velocity-sensitivity-limit-at-fixed-planet-mass.md), use $K=M_p\sin i\sqrt{G/(M_\star a)}$ and interpret the stated detection scale as a semi-amplitude threshold $K_{\min}$. The largest distance occurs for $\sin i=1$:

$$
\boxed{a_{\max}=\frac{G M_p^2}{M_\star K_{\min}^2}\simeq0.0180\,\mathrm{au}\quad(M_\star=M_\odot).}
$$

For an inclination $i$, this boundary is smaller by $\sin^2i$. The result assumes adequate time coverage and neglects the stipulated [stellar noise](../../../../stellar-noise.md). If the detection scale instead denotes a full peak-to-peak excursion, set $K_{\min}$ to half that scale; $a_{\max}$ then increases fourfold.

The [stellar-mass scaling of radial-velocity planet estimates](../../../../stellar-mass-scaling-of-radial-velocity-planet-estimates.md) changes these inferences because [Kepler's third law](../../../../kepler-s-third-law.md) and the stellar reflex response depend on the stellar [mass](../../../../mass.md). At fixed $K,P$, $M_p\sin i\propto M_\star^{2/3}$ and $a\propto M_\star^{1/3}$, whereas the fixed-[mass](../../../../mass.md) detectability boundary scales as $M_\star^{-1}$. Therefore

$$
\boxed{M_{p,\min}\simeq0.401\,M_J\simeq127\,M_\oplus,\quad a\simeq0.0721\,\mathrm{au},\quad a_{\max}(3M_\oplus)\simeq0.0360\,\mathrm{au}.}
$$

The observed period and amplitude are unchanged. The [stellar radius](../../../../stellar-radius.md) does not enter these leading dynamical estimates, but is crucial for the [exoplanet transit](../../../../exoplanet-transit.md) inference.

For the transiting companion, assume an opaque spherical [planet](../../../../planet.md), negligible [transit dilution](../../../../transit-dilution.md) and negligible [limb darkening](../../../../limb-darkening.md). Its [radius](../../../../radius.md) ratio is $k=R_p/R_\star=\sqrt\delta=0.03873$, hence

$$
\boxed{R_p=0.01936\,R_\odot\simeq1.35\times10^7\,\mathrm m\simeq2.11\,R_\oplus.}
$$

Using the revised stellar [mass](../../../../mass.md) and a [circular orbit](../../../../circular-orbit.md) gives $a=0.01850\,\mathrm{au}$ and $A=a/R_\star=7.957$. Interpret the duration as the total first-to-fourth-contact duration $T_{14}$. The [impact parameter from total transit duration](../../../../impact-parameter-from-total-transit-duration.md) follows from the [total duration of a circular planetary transit](../../../../total-duration-of-a-circular-planetary-transit.md):

$$
s=\sin\left(\frac{\pi T_{14}}P\right),\qquad b^2=\frac{(1+k)^2-A^2s^2}{1-s^2},\qquad\boxed{b\simeq0.893,\quad i=\arccos(b/A)\simeq83.56^\circ.}
$$

This is noncentral but not grazing: $b<1-k$. The small-[planet](../../../../planet.md) straight-chord approximation gives $b\simeq0.845$; retaining finite $R_p$ and orbital curvature gives the stated value. A duration measured between other contacts needs the corresponding contact formula. Unknown [orbital eccentricity](../../../../orbital-eccentricity.md) and argument of periapsis change the transverse speed and prevent a unique unconstrained $b$; the numerical estimate is conditional on the stated circular model.[Section3.1, equations1–4: depth, contact geometry and circular-orbit scale](../../../../on-the-unique-solution-of-planet-and-star-parameters-from-an-extrasolar-planet-transit-light-curve-by-sara-seager-and-gabriela-mallen-ornelas.md)

<a id="1/image-the-measured-transit-duration-selects-a-short-off-centre-chord-when-finite-planet-size-is-retained"></a>
![](../../../../past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2015/paper-1-transit-geometry.png)

**[Figure 1](#1/image-the-measured-transit-duration-selects-a-short-off-centre-chord-when-finite-planet-size-is-retained). The measured transit duration selects a short off-centre chord when finite planet size is retained**. [Source](paper-1-transit-geometry.py).

Because the transit constrains $\sin i\simeq0.994$, the RV nondetection now bounds the actual planetary [mass](../../../../mass.md), rather than only its projected [mass](../../../../mass.md). The [bulk-density upper limit from a transit and an RV nondetection](../../../../bulk-density-upper-limit-from-a-transit-and-an-rv-nondetection.md) is

$$
\boxed{M_p\lesssim2.16\,M_\oplus,\qquad\bar\rho_p\lesssim1.26\,\mathrm{g\,cm^{-3}}.}
$$

These bounds assume the instrumental threshold can be applied to a fitted signal at the transit period; no statistical confidence level is specified. Such a large [radius](../../../../radius.md) at this low [mass](../../../../mass.md) is inconsistent with an ordinary compact rock-and-iron body. A low-[density](../../../../density.md) volatile-rich [planet](../../../../planet.md), possibly with an extended H/He envelope, is indicated under the planetary interpretation. The observations do not uniquely determine interior composition, atmospheric abundance or formation history; blended eclipses and activity still require validation. There is no luminosity or effective [temperature](../../../../temperature-split.md) supplied for the host, so a numerical planetary equilibrium [temperature](../../../../temperature-split.md) cannot be inferred from these data alone.

The numerical conversions above use externally documented $(GM)_\odot=1.3271244\times10^{20}\,\mathrm{m^3\,s^{-2}}$, $R_\odot=6.957\times10^8\,\mathrm m$, $M_\oplus=5.9722\times10^{24}\,\mathrm{kg}$, $R_\oplus=6.371\times10^6\,\mathrm m$, $M_J=1.89813\times10^{27}\,\mathrm{kg}$, $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$ and $1\,\mathrm{au}=149597870700\,\mathrm m$. They are conversion constants, not additional measured system parameters.[2015 ResolutionB3: solar [radius](../../../../radius.md) and solar [mass](../../../../mass.md) parameter](../../../../nominal-solar-and-planetary-conversion-constants-by-the-international-astronomical-union.md)[Masses, mean radii and CODATA2018 gravitational constant](../../../../planetary-physical-parameters-by-nasa-jpl.md)

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the exoplanets and Planetary Systems course of the University of Cambridge](../../../split.md)
5. [Exoplanets and Planetary Systems course of the University of Cambridge](../../../../exoplanets-and-planetary-systems-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
