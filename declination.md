# Declination

↑ **Parent:** [Equatorial coordinate system](equatorial-coordinate-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Declination)

[Declination](declination.md) $\delta$ is the signed [angle](angle.md) from the reference [celestial equator](celestial-equator.md) to a direction, measured along its [hour circle](hour-circle.md): $-90^\circ\leq\delta\leq+90^\circ$. Positive [declination](declination.md) means celestial north, rather than necessarily north of the observer's [zenith](zenith.md). A direction with $\delta=0$ lies on the [celestial equator](celestial-equator.md); $\delta=+90^\circ$ is the north reference [celestial pole](celestial-pole.md). [Declination](declination.md) is an [angle](angle.md), not a height or a measure of [Euclidean distance](euclidean-distance.md). [US Naval Observatory: Astronomical Almanac glossary, declination and culmination](https://aa.usno.navy.mil/faq/asa_glossary).

The connection to an observation follows from a [dot product](dot-product.md). In the elementary spherical-[Earth](earth.md), unrefracted model, an observer at [geographical latitude](geographical-latitude.md) $\phi$ has [zenith](zenith.md) direction $\mathbf z=(\cos\phi\cos\Theta,\cos\phi\sin\Theta,\sin\phi)$ in the same reference axes. Since $\mathbf n\cdot\mathbf z=\sin a$ for [altitude](altitude.md) $a$, the [cosine addition formula](cosine-addition-formula.md) gives

$$
\sin a=\sin\phi\sin\delta+\cos\phi\cos\delta\cos H.
$$

At upper [meridian transit](meridian-transit.md), $H=0$, so $a_{\rm upper}=90^\circ-|\phi-\delta|$. For the synthetic site $\phi=52^\circ$ and synthetic direction $\delta=20^\circ$, this yields $a_{\rm upper}=58^\circ$. A direction with $\delta=70^\circ$ instead reaches $72^\circ$, north of the [zenith](zenith.md); positive [declination](declination.md) does not imply a crossing on the southern half of the [celestial meridian](celestial-meridian.md). A negative computed upper [altitude](altitude.md) means the direction never rises above the geometric [astronomical horizon](astronomical-horizon.md) at that site.

For an angular readout, define signed zenith distance $z_s$ on the upper [celestial meridian](celestial-meridian.md), positive toward the south and negative toward the north. Then $\delta=\phi-z_s$. A synthetic southward readout $z_s=32^\circ$ at $\phi=52^\circ$ recovers $\delta=20^\circ$. An unsigned distance $|z_s|$ alone would leave two possibilities, $\phi\pm|z_s|$, when both are in range. A calibrated [optical telescope](optical-telescope.md) must therefore record which side of the [zenith](zenith.md) it points toward. In this linear relation, a $1'$ error in the assumed [geographical latitude](geographical-latitude.md) produces a $1'$ error in inferred [declination](declination.md); averaging repeated readings cannot remove that shared offset. Near the [astronomical horizon](astronomical-horizon.md), uncorrected [atmospheric refraction](atmospheric-refraction.md) also invalidates the geometric readout.

The [unit vector](unit-vector.md) construction explains a subtle feature of sky maps. At fixed [declination](declination.md), changing [right ascension](right-ascension.md) traces a parallel whose radius on the unit [sphere](sphere.md) is $\cos\delta$. Its arc [length](length.md) is $\cos\delta\,|d\alpha|$, with [angles](angle.md) in [radians](radian.md); at $\delta=60^\circ$, a $15^\circ$ [right ascension](right-ascension.md) increment spans a $7.5^\circ$ arc along that parallel. This arc is not generally the shortest [great circle](great-circle.md) separation. At either [celestial pole](celestial-pole.md), all [right ascension](right-ascension.md) values represent the same direction: the [coordinate singularity](coordinate-singularity.md) belongs to the coordinate grid. The [unit vector](unit-vector.md) remains regular there.

## ↑ Ancestors (5)

1. [Equatorial coordinate system](equatorial-coordinate-system.md)
2. [Astrophysics](astrophysics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Astrometry](astrometry.md)
- [Celestial equator](celestial-equator.md)
- [Celestial pole](celestial-pole.md)
- [Declination](declination.md)
- [Earth-rotation aperture synthesis](earth-rotation-aperture-synthesis.md)
- [Epoch (astronomy)](epoch-astronomy.md)
- [Equatorial coordinate system](equatorial-coordinate-system.md)
- [Horizontal coordinate system](horizontal-coordinate-system.md)
- [Hour circle](hour-circle.md)
- [Orbital observations behind the area law](orbital-observations-behind-the-area-law.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/1/a/ii/solution.md)
- [Proper motion](proper-motion.md)
- [Right ascension](right-ascension.md)
- [Zenith distance](zenith-distance.md)
