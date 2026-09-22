# Astronomy

↑ **Parent:** [Codex Wiki](README.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Astronomy)

Astronomy studies celestial objects and phenomena, including [stars](stellar-astrophysics.md#star), [planets](planetary-science.md#planet) and [galaxies](galaxy.md). [Astrometry](#astrometry) measures their [positions](classical-mechanics.md#position) and motion; [astrophysics](astrophysics.md) uses [physics](physics.md) to explain their properties and behaviour.

Much of [astronomy](astronomy.md) begins with incoming [light](optics.md#light). An image tells us which direction the [light](optics.md#light) arrived from, rather than directly providing the source's three-dimensional [position](classical-mechanics.md#position). Two [stars](stellar-astrophysics.md#star) close together on the sky may be very far apart in space. The [celestial sphere](astrophysics.md#celestial-sphere) organizes these viewing directions; locating an object on it is a different task from measuring how far away that object is. Repeated observations turn this limitation into an opportunity: the changing direction of [light](optics.md#light) contains evidence about both [Euclidean distance](topological-analysis.md#euclidean-distance) and motion.

The particularly satisfying combination is [stellar parallax](astrophysics.md#stellar-parallax) with [proper motion](#proper-motion). The first supplies a geometric [Euclidean distance](topological-analysis.md#euclidean-distance), while the second measures how rapidly the viewing direction changes after accounting for the observer's annual motion. Together they give a transverse [speed](classical-mechanics.md#speed), connecting tiny [angles](geometry-and-topology.md#angle) on an image to kilometres travelled each second. This bridge from a flat sky map to moving [stars](stellar-astrophysics.md#star) is one reason [astrometry](#astrometry) matters to the study of the [Milky Way](galaxy.md#milky-way).

**Table of contents**

- [Astronomer](#astronomer)
  - [Edmond Halley](#edmond-halley)
  - [Johannes Kepler](#johannes-kepler)
- [Astrometry](#astrometry)
  - [Proper motion](#proper-motion)

## Astronomer

↑ **Parent:** [Astronomy](astronomy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Astronomer)

### Edmond Halley

↑ **Parent:** [Astronomer](#astronomer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edmond_Halley)

### Johannes Kepler

↑ **Parent:** [Astronomer](#astronomer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Johannes_Kepler)

## Astrometry

↑ **Parent:** [Astronomy](astronomy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Astrometry)

Astrometry measures the [positions](classical-mechanics.md#position) and motions of celestial objects. Repeated [position](classical-mechanics.md#position) measurements can distinguish [stellar parallax](astrophysics.md#stellar-parallax), caused by the observer's motion, from [proper motion](#proper-motion) of the source across the sky.

An [astrometry](#astrometry) measurement needs a date and a [reference frame](physics.md#reference-frame), as well as an [angle](geometry-and-topology.md#angle). In an [equatorial coordinate system](astrophysics.md#equatorial-coordinate-system), [right ascension](astrophysics.md#right-ascension) and [declination](astrophysics.md#declination) label two viewing directions. A catalogue's reference date states when its quoted [position](classical-mechanics.md#position) applies; comparing entries at different dates without accounting for [proper motion](#proper-motion) can make the same [star](stellar-astrophysics.md#star) appear misplaced. The observational problem is to infer a consistent history from successive incoming [light](optics.md#light) directions, while accounting for the observer's changing [position](classical-mechanics.md#position) and [measurement error](probability-and-statistics.md#measurement-error).

To see the separation clearly, consider just one angular coordinate $\theta$, with $t$ the numerical elapsed [time](classical-mechanics.md#time-in-physics) in years. Assume a simplified [circular orbit](classical-mechanics.md#circular-orbit) of the [Earth](planetary-science.md#earth), a fixed source [Euclidean distance](topological-analysis.md#euclidean-distance), constant [proper motion](#proper-motion) in this coordinate and no other [accelerations](classical-mechanics.md#acceleration). Choose the direction and the starting date so that the annual [stellar parallax](astrophysics.md#stellar-parallax) projection is the [cosine](geometry-and-topology.md#cosine) term

$$
\theta(t)=\theta_0+\mu t+p\cos(2\pi t).
$$

Here $\theta_0$ is the coordinate without the annual [stellar parallax](astrophysics.md#stellar-parallax) offset at the reference date; the observed $\theta(0)$ is $\theta_0+p$. The [proper motion](#proper-motion) coefficient $\mu$ is quoted in [arcseconds](geometry-and-topology.md#arcsecond) per year, and $p$ is the annual [stellar parallax](astrophysics.md#stellar-parallax) in [arcseconds](geometry-and-topology.md#arcsecond). This is an illustrative choice of a full-[amplitude](physics.md#wave-amplitude) projection. General sky directions have different projected [amplitudes](physics.md#wave-amplitude) and [phases](physics.md#phase-waves) in their two coordinates; their apparent paths need not be [circles](topology.md#circle). Real [astrometry](#astrometry) uses the observer's calculated [position](classical-mechanics.md#position) rather than imposing this single [cosine](geometry-and-topology.md#cosine). [ESA Gaia DR3: Astrometric source model](https://gea.esac.esa.int/archive/documentation/GDR3/Data_processing/chap_cu3ast/sec_cu3ast_cali/ssec_cu3ast_cali_source.html).

Set $\theta_0=0$, $\mu=100\,\mathrm{mas\,yr^{-1}}$ and $p=50\,\mathrm{mas}$, where $1\,\mathrm{mas}$ is one thousandth of an [arcsecond](geometry-and-topology.md#arcsecond). The model gives $\theta(0)=50$, $\theta(0.5)=0$ and $\theta(1)=150\,\mathrm{mas}$. Same-season observations one year apart differ by $100\,\mathrm{mas}$ because the annual [stellar parallax](astrophysics.md#stellar-parallax) contribution repeats. Subtracting that fitted straight trend leaves an annual signal between $-50$ and $+50\,\mathrm{mas}$. The existing [stellar parallax](astrophysics.md#stellar-parallax) distance relation then gives $20$ [parsecs](astrophysics.md#parsec).

<a id="image-separating-a-100-mas-per-year-proper-motion-trend-from-a-50-mas-annual-parallax-projection"></a>
![](proper-motion-parallax-separation.png)

**[Figure 1](#image-separating-a-100-mas-per-year-proper-motion-trend-from-a-50-mas-annual-parallax-projection). Separating a 100-mas-per-year proper-motion trend from a 50-mas annual parallax projection**.

Observing only at the same annual [phase](physics.md#phase-waves) would recover the [proper motion](#proper-motion) trend but leave $p$ indistinguishable from a constant offset. Sampling several seasons as well as several years separates the repeating signal from the accumulating [displacement](classical-mechanics.md#displacement). The two signatures answer different questions using the same measurements.

### Proper motion

↑ **Parent:** [Astrometry](#astrometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_motion)

Proper motion describes the change in a celestial object's direction on the sky due to its motion relative to the observer. Its [angular velocity](classical-mechanics.md#angular-velocity) differs from the annual [stellar parallax](astrophysics.md#stellar-parallax) signal caused by the observer's orbit.

Thus [proper motion](#proper-motion) is an [angular velocity](classical-mechanics.md#angular-velocity), rather than a [speed](classical-mechanics.md#speed) in kilometres per second. It describes the relative transverse motion of source and observer in a specified [reference frame](physics.md#reference-frame). A [star](stellar-astrophysics.md#star) moving towards us can have little [proper motion](#proper-motion), while a nearer [star](stellar-astrophysics.md#star) can show larger [proper motion](#proper-motion) than a faster but more distant one. In the example above, the observed coordinate actually decreases over the first half-year, although $\mu$ is positive: the annual [stellar parallax](astrophysics.md#stellar-parallax) excursion temporarily outweighs the steady drift. A short observed [displacement](classical-mechanics.md#displacement) alone therefore need not estimate [proper motion](#proper-motion) well.

Real catalogues give two [proper motion](#proper-motion) components. For [right ascension](astrophysics.md#right-ascension) $\alpha$ and [declination](astrophysics.md#declination) $\delta$, the [angular velocities](classical-mechanics.md#angular-velocity) in perpendicular directions on the local sky are

$$
\mu_{\alpha *}=\cos\delta\,\frac{d\alpha}{dt},\qquad
\mu_\delta=\frac{d\delta}{dt},\qquad
\mu_{\rm tot}=\sqrt{\mu_{\alpha *}^2+\mu_\delta^2}.
$$

The [cosine](geometry-and-topology.md#cosine) factor accounts for the shorter east-west arc associated with a given [right ascension](astrophysics.md#right-ascension) increment away from the [celestial equator](astrophysics.md#celestial-equator). ESA's Gaia DR3 fields `pmra` and `pmdec` already contain these two components; `pm` is their total [proper motion](#proper-motion). Do not multiply `pmra` by another [cosine](geometry-and-topology.md#cosine). Components of $60$ and $80\,\mathrm{mas\,yr^{-1}}$, for example, give total [proper motion](#proper-motion) $100\,\mathrm{mas\,yr^{-1}}$. [ESA Gaia DR3: Proper-motion columns and conventions](https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html).

For nearby [stars](stellar-astrophysics.md#star) in the ordinary nonrelativistic approximation, [Euclidean distance](topological-analysis.md#euclidean-distance) $d$ converts total [proper motion](#proper-motion) into transverse [speed](classical-mechanics.md#speed) $v_\perp$:

$$
\frac{v_\perp}{1\,\mathrm{km\,s^{-1}}}
=4.74047\,\frac{\mu_{\rm tot}}{1\,\mathrm{arcsec\,yr^{-1}}}\,\frac{d}{1\,\mathrm{pc}}.
$$

The [small-angle approximation](geometry-and-topology.md#small-angle-approximation) gives transverse [speed](classical-mechanics.md#speed) as [Euclidean distance](topological-analysis.md#euclidean-distance) times [angular velocity](classical-mechanics.md#angular-velocity) in [radians](geometry-and-topology.md#radian) per unit [time](classical-mechanics.md#time-in-physics). With [arcseconds](geometry-and-topology.md#arcsecond) and [parsecs](astrophysics.md#parsec), the [parsec](astrophysics.md#parsec) convention turns their product into [astronomical units](planetary-science.md#astronomical-unit) per year. One [astronomical unit](planetary-science.md#astronomical-unit) per Julian year of $365.25$ days is approximately $4.74047\,\mathrm{km\,s^{-1}}$. The coefficient is a unit conversion, rather than a property of a particular [star](stellar-astrophysics.md#star).

Taking the model's $100\,\mathrm{mas\,yr^{-1}}=0.100\,\mathrm{arcsec\,yr^{-1}}$ as the total [proper motion](#proper-motion), with the other component zero, gives $v_\perp=4.74047\times0.100\times20\simeq9.48\,\mathrm{km\,s^{-1}}$. At the same total [proper motion](#proper-motion), [Euclidean distances](topological-analysis.md#euclidean-distance) of $10$, $20$ and $100$ [parsecs](astrophysics.md#parsec) instead give transverse [speeds](classical-mechanics.md#speed) of $4.74$, $9.48$ and $47.40\,\mathrm{km\,s^{-1}}$, respectively. Their [stellar parallax](astrophysics.md#stellar-parallax) values are $100$, $50$ and $10\,\mathrm{mas}$. The same annual angular [displacement](classical-mechanics.md#displacement) can therefore describe quite different journeys through space.

<a id="image-the-same-100-mas-per-year-proper-motion-gives-larger-transverse-speed-at-greater-distance"></a>
![](angular-rate-versus-speed.png)

**[Figure 2](#image-the-same-100-mas-per-year-proper-motion-gives-larger-transverse-speed-at-greater-distance). The same 100-mas-per-year proper motion gives larger transverse speed at greater distance**.

The transverse [speed](classical-mechanics.md#speed) still omits the line-of-sight [velocity](classical-mechanics.md#velocity), which can be measured through the [Doppler effect](physics.md#doppler-effect) in [spectral lines](stellar-astrophysics.md#spectral-line). Combining these measurements permits a three-dimensional [velocity](classical-mechanics.md#velocity) estimate in a consistent [reference frame](physics.md#reference-frame). [ESA: Combining proper motion, distance and radial velocity](https://www.esa.int/Science_Exploration/Space_Science/Gaia/How_does_Gaia_study_the_Milky_Way).

Historically, [Edmond Halley](#edmond-halley)'s 1718 paper compared contemporary and ancient stellar directions and argued that some supposedly fixed [stars](stellar-astrophysics.md#star) had moved. Its title, "Considerations on the change of the latitudes of some of the principal fixt stars", captures the conceptual surprise: long-separated measurements could reveal motion invisible in an ordinary night's watching. Modern [astrometry](#astrometry) retains that insight, using repeated precise measurements to turn the apparently static sky into a record of changing [positions](classical-mechanics.md#position). [Halley: Original Royal Society paper, pages 736-738](https://archive.org/details/paper-doi-10_1098_rstl_1717_0025). [ESA: Halley's 1718 comparison](https://www.esa.int/Science_Exploration/Space_Science/Gaia/How_does_Gaia_study_the_Milky_Way).

## ↑ Ancestors (1)

1. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Astronomy](astronomy.md)
- [Orbital observations behind the area law](classical-mechanics.md#orbital-observations-behind-the-area-law)
- [Spherical trigonometry](geometry-and-topology.md#spherical-trigonometry)
