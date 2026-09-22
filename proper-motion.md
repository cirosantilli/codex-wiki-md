# Proper motion

↑ **Parent:** [Astrometry](astrometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_motion)

Proper motion describes the change in a celestial object's direction on the sky due to its motion relative to the observer. Its [angular velocity](angular-velocity.md) differs from the annual [stellar parallax](stellar-parallax.md) signal caused by the observer's orbit.

Thus [proper motion](proper-motion.md) is an [angular velocity](angular-velocity.md), rather than a [speed](speed.md) in kilometres per second. It describes the relative transverse motion of source and observer in a specified [reference frame](reference-frame.md). A [star](star.md) moving towards us can have little [proper motion](proper-motion.md), while a nearer [star](star.md) can show larger [proper motion](proper-motion.md) than a faster but more distant one. In the example above, the observed coordinate actually decreases over the first half-year, although $\mu$ is positive: the annual [stellar parallax](stellar-parallax.md) excursion temporarily outweighs the steady drift. A short observed [displacement](displacement.md) alone therefore need not estimate [proper motion](proper-motion.md) well.

Real catalogues give two [proper motion](proper-motion.md) components. For [right ascension](right-ascension.md) $\alpha$ and [declination](declination.md) $\delta$, the [angular velocities](angular-velocity.md) in perpendicular directions on the local sky are

$$
\mu_{\alpha *}=\cos\delta\,\frac{d\alpha}{dt},\qquad
\mu_\delta=\frac{d\delta}{dt},\qquad
\mu_{\rm tot}=\sqrt{\mu_{\alpha *}^2+\mu_\delta^2}.
$$

The [cosine](cosine.md) factor accounts for the shorter east-west arc associated with a given [right ascension](right-ascension.md) increment away from the [celestial equator](celestial-equator.md). ESA's Gaia DR3 fields `pmra` and `pmdec` already contain these two components; `pm` is their total [proper motion](proper-motion.md). Do not multiply `pmra` by another [cosine](cosine.md). Components of $60$ and $80\,\mathrm{mas\,yr^{-1}}$, for example, give total [proper motion](proper-motion.md) $100\,\mathrm{mas\,yr^{-1}}$. [ESA Gaia DR3: Proper-motion columns and conventions](https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html).

For nearby [stars](star.md) in the ordinary nonrelativistic approximation, [Euclidean distance](euclidean-distance.md) $d$ converts total [proper motion](proper-motion.md) into transverse [speed](speed.md) $v_\perp$:

$$
\frac{v_\perp}{1\,\mathrm{km\,s^{-1}}}
=4.74047\,\frac{\mu_{\rm tot}}{1\,\mathrm{arcsec\,yr^{-1}}}\,\frac{d}{1\,\mathrm{pc}}.
$$

The [small-angle approximation](small-angle-approximation.md) gives transverse [speed](speed.md) as [Euclidean distance](euclidean-distance.md) times [angular velocity](angular-velocity.md) in [radians](radian.md) per unit [time](time-in-physics.md). With [arcseconds](arcsecond.md) and [parsecs](parsec.md), the [parsec](parsec.md) convention turns their product into [astronomical units](astronomical-unit.md) per year. One [astronomical unit](astronomical-unit.md) per Julian year of $365.25$ days is approximately $4.74047\,\mathrm{km\,s^{-1}}$. The coefficient is a unit conversion, rather than a property of a particular [star](star.md).

Taking the model's $100\,\mathrm{mas\,yr^{-1}}=0.100\,\mathrm{arcsec\,yr^{-1}}$ as the total [proper motion](proper-motion.md), with the other component zero, gives $v_\perp=4.74047\times0.100\times20\simeq9.48\,\mathrm{km\,s^{-1}}$. At the same total [proper motion](proper-motion.md), [Euclidean distances](euclidean-distance.md) of $10$, $20$ and $100$ [parsecs](parsec.md) instead give transverse [speeds](speed.md) of $4.74$, $9.48$ and $47.40\,\mathrm{km\,s^{-1}}$, respectively. Their [stellar parallax](stellar-parallax.md) values are $100$, $50$ and $10\,\mathrm{mas}$. The same annual angular [displacement](displacement.md) can therefore describe quite different journeys through space.

<a id="image-the-same-100-mas-per-year-proper-motion-gives-larger-transverse-speed-at-greater-distance"></a>
![](angular-rate-versus-speed.png)

**[Figure 2](#image-the-same-100-mas-per-year-proper-motion-gives-larger-transverse-speed-at-greater-distance). The same 100-mas-per-year proper motion gives larger transverse speed at greater distance**.

The transverse [speed](speed.md) still omits the line-of-sight [velocity](velocity.md), which can be measured through the [Doppler effect](doppler-effect.md) in [spectral lines](spectral-line.md). Combining these measurements permits a three-dimensional [velocity](velocity.md) estimate in a consistent [reference frame](reference-frame.md). [ESA: Combining proper motion, distance and radial velocity](https://www.esa.int/Science_Exploration/Space_Science/Gaia/How_does_Gaia_study_the_Milky_Way).

Historically, [Edmond Halley](edmond-halley.md)'s 1718 paper compared contemporary and ancient stellar directions and argued that some supposedly fixed [stars](star.md) had moved. Its title, "Considerations on the change of the latitudes of some of the principal fixt stars", captures the conceptual surprise: long-separated measurements could reveal motion invisible in an ordinary night's watching. Modern [astrometry](astrometry.md) retains that insight, using repeated precise measurements to turn the apparently static sky into a record of changing [positions](position.md). [Halley: Original Royal Society paper, pages 736-738](https://archive.org/details/paper-doi-10_1098_rstl_1717_0025). [ESA: Halley's 1718 comparison](https://www.esa.int/Science_Exploration/Space_Science/Gaia/How_does_Gaia_study_the_Milky_Way).

## ↑ Ancestors (3)

1. [Astrometry](astrometry.md)
2. [Astronomy](astronomy-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Astrometry](astrometry.md)
- [Astronomy](astronomy-split.md)
- [Epoch (astronomy)](epoch-astronomy.md)
- [Equatorial coordinate system](equatorial-coordinate-system.md)
- [Proper motion](proper-motion.md)
- [Stellar parallax](stellar-parallax.md)
