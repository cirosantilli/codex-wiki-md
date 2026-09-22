# Lunar phase

↑ **Parent:** [Moon](moon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lunar_phase)

A [lunar phase](lunar-phase.md) is the appearance of the sunlit portion of the [Moon](moon.md) as seen from [Earth](earth.md). Outside a [lunar eclipse](lunar-eclipse.md), the distant [Sun](sun.md) illuminates approximately one hemisphere of the [Moon](moon.md), but an observer sees a changing overlap of that hemisphere with the hemisphere facing [Earth](earth.md). The [lunar phase](lunar-phase.md) therefore changes even though [synchronous rotation](synchronous-rotation.md) keeps approximately the same [near side of the Moon](near-side-of-the-moon.md) facing [Earth](earth.md). [NASA: Moon phases and illumination geometry](https://science.nasa.gov/moon/moon-phases/).

The cycle runs through new Moon, waxing crescent, first quarter, waxing gibbous, full Moon, waning gibbous, last quarter and waning crescent. “Waxing” means that the [lunar illuminated fraction](lunar-illuminated-fraction.md) is increasing; “waning” means it is decreasing. A crescent has less than half its apparent disk sunlit, and a gibbous [lunar phase](lunar-phase.md) has more than half. First and last quarter each show half a disk: “quarter” refers to progress around the cycle, rather than a quarter of the disk being lit. [US Naval Observatory: disk fractions and waxing versus waning](https://aa.usno.navy.mil/data/MoonFraction).

An instructive [circular orbit](circular-orbit.md) model puts [Earth](earth.md) at the origin, the [Sun](sun.md) far away along $+x$, and the [Moon](moon.md) at $R(\cos\theta,\sin\theta)$. The sunward position $x>0$, $\theta=0$, gives new Moon; the opposite position $x<0$, $\theta=\pi$, gives full Moon. Counterclockwise motion gives first quarter at $\theta=\pi/2$ and last quarter at $\theta=3\pi/2$. The [Sun](sun.md)'s direction is fixed during this snapshot of the cycle. Every small globe in the orbital view is illuminated on its $+x$ half; the adjacent apparent disks are separate views from [Earth](earth.md), rather than globes viewed from above.

<a id="image-eight-lunar-phases-in-a-circular-orbit-and-the-corresponding-apparent-disks-from-earth"></a>
![](lunar-phases-orbit-and-disks.png)

**[Figure 1](#image-eight-lunar-phases-in-a-circular-orbit-and-the-corresponding-apparent-disks-from-earth). Eight lunar phases in a circular orbit and the corresponding apparent disks from Earth**.

The disk views choose north up, with the upward direction perpendicular to the [orbital plane](orbital-plane.md). In this convention waxing [lunar phases](lunar-phase.md) are bright on the right and waning [lunar phases](lunar-phase.md) on the left. Local horizon orientation and viewing from different locations on [Earth](earth.md) can rotate the apparent disk; its lit edge always points toward the projected direction of the [Sun](sun.md). The [lunar illuminated fraction](lunar-illuminated-fraction.md) is unaffected by this rotation.

The useful [angle](angle.md) is the [phase angle](phase-angle-astronomy.md) $\alpha=\angle SME$, with $S$ the [Sun](sun.md), $M$ the [Moon](moon.md) and $E$ the observer at [Earth](earth.md)'s center: its vertex is at the [Moon](moon.md). Full Moon has $\alpha=0$, quarter has $\alpha=\pi/2$, and new Moon has $\alpha=\pi$ in the ideal model. By contrast, the [elongation](elongation-astronomy.md) $\epsilon=\angle SEM$ has its vertex at [Earth](earth.md). For a distant [Sun](sun.md), its rays are parallel, so

$$
\alpha=\pi-\epsilon,\qquad k=\frac{1+\cos\alpha}{2}=\frac{1-\cos\epsilon}{2}.
$$

Here $k$ is the [lunar illuminated fraction](lunar-illuminated-fraction.md): a fraction of projected disk [area](surface-area.md), not a fraction of the [Moon](moon.md)'s total [surface area](surface-area.md) or its received [radiant flux](radiant-flux.md) relative to full Moon. The [phase angle](phase-angle-astronomy.md) and unsigned [elongation](elongation-astronomy.md) each lie between $0$ and $\pi$, so either alone gives the illuminated amount without distinguishing waxing from waning. The orbital direction resolves that ambiguity.

<a id="image-projected-illuminated-fraction-versus-the-sun-moon-observer-phase-angle-at-the-moon"></a>
![](lunar-phase-illuminated-fraction.png)

**[Figure 2](#image-projected-illuminated-fraction-versus-the-sun-moon-observer-phase-angle-at-the-moon). Projected illuminated fraction versus the Sun–Moon–observer phase angle at the Moon**.

The [lunar illuminated fraction](lunar-illuminated-fraction.md) has an elegant geometric derivation. Model the [Moon](moon.md) as a [sphere](sphere.md) of unit radius and view it along the $z$ direction. Take the [Sun](sun.md)'s unit direction to be $(\sin\alpha,0,\cos\alpha)$. A visible surface point above apparent disk coordinates $(x,y)$ has $z=\sqrt{1-x^2-y^2}$. Direct illumination requires the outward normal's [dot product](dot-product.md) with the sunward direction to be positive. The [day-night terminator](day-night-terminator.md) therefore obeys $x\sin\alpha+z\cos\alpha=0$. At a fixed $y$, set $q=\sqrt{1-y^2}$; the visible [day-night terminator](day-night-terminator.md) is $x_t=-q\cos\alpha$, and the illuminated strip extends from $x_t$ to the right edge $q$. Integrating its width gives

$$
A_{\mathrm{lit}}=\int_{-1}^{1}(1+\cos\alpha)\sqrt{1-y^2}\,dy
=\frac{\pi}{2}(1+\cos\alpha),\qquad
k=\frac{A_{\mathrm{lit}}}{\pi}.
$$

The [integral](integral.md) is the [area](surface-area.md) of half a unit [circle](circle.md). Thus a three-dimensional visibility problem reduces to a [circle](circle.md)'s [area](surface-area.md) and a [cosine](cosine.md). The derivation assumes parallel sunlight, a distant observer and a [sphere](sphere.md), and ignores a [lunar eclipse](lunar-eclipse.md). Real observed brightness additionally depends on surface [scattering of light](scattering-of-light.md) and observing geometry, so $k=1/2$ does not promise half the full-Moon [radiant flux](radiant-flux.md).

For a worked example, [elongation](elongation-astronomy.md) $\epsilon=60^\circ$ gives [phase angle](phase-angle-astronomy.md) $\alpha=120^\circ$ and $k=(1+\cos120^\circ)/2=1/4$: a crescent with $25\%$ of its apparent disk sunlit. At [elongation](elongation-astronomy.md) $120^\circ$, the [phase angle](phase-angle-astronomy.md) is $60^\circ$ and $k=3/4$: a gibbous [lunar phase](lunar-phase.md). At $90^\circ$, $k=1/2$. In each case the same $k$ occurs once while waxing and once while waning in the ideal cycle.

Ordinary [lunar phases](lunar-phase.md) are not caused by [Earth](earth.md)'s shadow. A [lunar eclipse](lunar-eclipse.md) occurs only when the [Moon](moon.md) actually enters that shadow near full Moon. The [orbital inclination](orbital-inclination.md) of the [Moon](moon.md) is about $5^\circ$ relative to [Earth](earth.md)'s [orbital plane](orbital-plane.md) around the [Sun](sun.md); most full Moons pass above or below the shadow. This is why full Moon does not imply a [lunar eclipse](lunar-eclipse.md) every month. [NASA: lunar eclipses and the Moon's roughly five-degree orbital tilt](https://science.nasa.gov/moon/eclipses/).

The phase cycle is a [synodic month](synodic-month.md), about $29.5$ days, whereas the [Moon](moon.md)'s [orbital period](orbital-period.md) relative to distant stars is a [sidereal month](sidereal-month.md), about $27.3$ days. During one [sidereal month](sidereal-month.md), [Earth](earth.md) advances around the [Sun](sun.md), so the [Moon](moon.md) must move farther to repeat the sunward alignment. For coplanar [circular orbits](circular-orbit.md) traversed in the same direction, subtract their [mean motions](mean-motion.md): $n_{\mathrm{syn}}=n_{\mathrm{sid}}-n_{\mathrm{year}}$, with $n=2\pi/P$. Hence

$$
\frac{1}{P_{\mathrm{syn}}}=\frac{1}{P_{\mathrm{sid}}}-\frac{1}{P_{\mathrm{year}}},\qquad
P_{\mathrm{syn}}=\frac{P_{\mathrm{sid}}P_{\mathrm{year}}}{P_{\mathrm{year}}-P_{\mathrm{sid}}}.
$$

Using $P_{\mathrm{sid}}=27.321661\,\mathrm{days}$ and $P_{\mathrm{year}}=365.256\,\mathrm{days}$ gives $P_{\mathrm{syn}}=29.530591\,\mathrm{days}$, consistent with the mean [synodic month](synodic-month.md) of $29.53059$ days. After one [sidereal month](sidereal-month.md), the sunward direction has advanced about $26.93^\circ$; catching up takes about $2.21$ more days. These are mean-period estimates: [orbital eccentricity](orbital-eccentricity.md) and changing geometry make individual [synodic months](synodic-month.md) vary. [Fred Espenak, NASA: sidereal and synodic months and varying lunations](https://eclipse.gsfc.nasa.gov/SEhelp/moonorbit.html). [David R. Williams, NASA: Earth's sidereal orbital period](https://nssdc.gsfc.nasa.gov/planetary/factsheet/earthfact.html).

The [lunar phase](lunar-phase.md) is also a practical clock for observing. Full Moon is opposite the [Sun](sun.md) and rises roughly at sunset; first quarter is about a [right angle](right-angle.md) from the [Sun](sun.md) and is convenient in the evening, while last quarter is convenient before dawn. These are rough guides, not exact rise-time predictions for every place and season. [NASA: approximate visibility times by lunar phase](https://science.nasa.gov/moon/moon-phases/). Historically, repeated [lunar phases](lunar-phase.md) provided the month in lunar calendars, while half-lit disks gave [Aristarchus of Samos](aristarchus-of-samos.md) a way to infer astronomical distances. [Fred Espenak, NASA: lunations and lunar calendars](https://eclipse.gsfc.nasa.gov/SEhelp/moonorbit.html).

**Table of contents**

- [Phase angle (astronomy)](phase-angle-astronomy.md)
- [Elongation (astronomy)](elongation-astronomy.md)
- [Lunar illuminated fraction](lunar-illuminated-fraction.md)
- [Sidereal month](sidereal-month.md)
- [Synodic month](synodic-month.md)
- [Aristarchus of Samos](aristarchus-of-samos.md)

## ↑ Ancestors (7)

1. [Moon](moon.md)
2. [Natural satellite](natural-satellite.md)
3. [Planetary science](planetary-science-split.md)
4. [Astrophysics](astrophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Aristarchus of Samos](aristarchus-of-samos.md)
- [Elongation (astronomy)](elongation-astronomy.md)
- [Far side of the Moon](far-side-of-the-moon.md)
- [Illumination of a synchronously rotating moon](illumination-of-a-synchronously-rotating-moon.md)
- [Lunar eclipse](lunar-eclipse.md)
- [Lunar phase](lunar-phase.md)
- [Phase angle (astronomy)](phase-angle-astronomy.md)
- [Synodic month](synodic-month.md)
