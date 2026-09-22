# Astrometry

↑ **Parent:** [Astronomy](astronomy-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Astrometry)

Astrometry measures the [positions](position.md) and motions of celestial objects. Repeated [position](position.md) measurements can distinguish [stellar parallax](stellar-parallax.md), caused by the observer's motion, from [proper motion](proper-motion.md) of the source across the sky.

An [astrometry](astrometry.md) measurement needs a date and a [reference frame](reference-frame.md), as well as an [angle](angle.md). In an [equatorial coordinate system](equatorial-coordinate-system.md), [right ascension](right-ascension.md) and [declination](declination.md) label two viewing directions. A catalogue's reference date states when its quoted [position](position.md) applies; comparing entries at different dates without accounting for [proper motion](proper-motion.md) can make the same [star](star.md) appear misplaced. The observational problem is to infer a consistent history from successive incoming [light](light.md) directions, while accounting for the observer's changing [position](position.md) and [measurement error](measurement-error.md).

To see the separation clearly, consider just one angular coordinate $\theta$, with $t$ the numerical elapsed [time](time-in-physics.md) in years. Assume a simplified [circular orbit](circular-orbit.md) of the [Earth](earth.md), a fixed source [Euclidean distance](euclidean-distance.md), constant [proper motion](proper-motion.md) in this coordinate and no other [accelerations](acceleration.md). Choose the direction and the starting date so that the annual [stellar parallax](stellar-parallax.md) projection is the [cosine](cosine.md) term

$$
\theta(t)=\theta_0+\mu t+p\cos(2\pi t).
$$

Here $\theta_0$ is the coordinate without the annual [stellar parallax](stellar-parallax.md) offset at the reference date; the observed $\theta(0)$ is $\theta_0+p$. The [proper motion](proper-motion.md) coefficient $\mu$ is quoted in [arcseconds](arcsecond.md) per year, and $p$ is the annual [stellar parallax](stellar-parallax.md) in [arcseconds](arcsecond.md). This is an illustrative choice of a full-[amplitude](wave-amplitude.md) projection. General sky directions have different projected [amplitudes](wave-amplitude.md) and [phases](phase-waves.md) in their two coordinates; their apparent paths need not be [circles](circle.md). Real [astrometry](astrometry.md) uses the observer's calculated [position](position.md) rather than imposing this single [cosine](cosine.md). [ESA Gaia DR3: Astrometric source model](https://gea.esac.esa.int/archive/documentation/GDR3/Data_processing/chap_cu3ast/sec_cu3ast_cali/ssec_cu3ast_cali_source.html).

Set $\theta_0=0$, $\mu=100\,\mathrm{mas\,yr^{-1}}$ and $p=50\,\mathrm{mas}$, where $1\,\mathrm{mas}$ is one thousandth of an [arcsecond](arcsecond.md). The model gives $\theta(0)=50$, $\theta(0.5)=0$ and $\theta(1)=150\,\mathrm{mas}$. Same-season observations one year apart differ by $100\,\mathrm{mas}$ because the annual [stellar parallax](stellar-parallax.md) contribution repeats. Subtracting that fitted straight trend leaves an annual signal between $-50$ and $+50\,\mathrm{mas}$. The existing [stellar parallax](stellar-parallax.md) distance relation then gives $20$ [parsecs](parsec.md).

<a id="image-separating-a-100-mas-per-year-proper-motion-trend-from-a-50-mas-annual-parallax-projection"></a>
![](proper-motion-parallax-separation.png)

**[Figure 5](#image-separating-a-100-mas-per-year-proper-motion-trend-from-a-50-mas-annual-parallax-projection). Separating a 100-mas-per-year proper-motion trend from a 50-mas annual parallax projection**.

Observing only at the same annual [phase](phase-waves.md) would recover the [proper motion](proper-motion.md) trend but leave $p$ indistinguishable from a constant offset. Sampling several seasons as well as several years separates the repeating signal from the accumulating [displacement](displacement.md). The two signatures answer different questions using the same measurements.

**Table of contents**

- [Orbital parallax](orbital-parallax.md)
- [Proper motion](proper-motion.md)

## ↑ Ancestors (2)

1. [Astronomy](astronomy-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Astrometry](astrometry.md)
- [Astronomy](astronomy-split.md)
- [Mass-distance degeneracy of an angular stellar orbit](mass-distance-degeneracy-of-an-angular-stellar-orbit.md)
- [Methods of detecting exoplanets](methods-of-detecting-exoplanets.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2015/paper-1/3/e/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2014/paper-1/2/c/solution.md)
- [Proper motion](proper-motion.md)
- [Stellar orbits at the Galactic centre](stellar-orbits-at-the-galactic-centre.md)
- [Stellar parallax](stellar-parallax.md)
- [Stellar reflex motion](stellar-reflex-motion.md)
- [Very Long Baseline Array](very-long-baseline-array.md)
