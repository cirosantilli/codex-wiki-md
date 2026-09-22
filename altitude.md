# Altitude

↑ **Parent:** [Horizontal coordinate system](horizontal-coordinate-system.md)

[Altitude](altitude.md) $\gamma$, also called [elevation angle](altitude.md), is the signed [angle](angle.md) from the [astronomical horizon](astronomical-horizon.md) to a viewing direction, measured in the vertical [plane](plane.md) containing that direction and the [zenith](zenith.md). Its range is $-90^\circ\leq\gamma\leq90^\circ$: positive [altitude](altitude.md) is above the horizontal [plane](plane.md), zero [altitude](altitude.md) lies on the [astronomical horizon](astronomical-horizon.md), and $90^\circ$ points to the [zenith](zenith.md). [Altitude](altitude.md) measures direction, rather than a [Euclidean distance](euclidean-distance.md) or a height in metres. In the local [horizontal coordinate system](horizontal-coordinate-system.md), $\sin\gamma=\mathbf n\cdot\mathbf e_U$; the [dot product](dot-product.md) makes the sign unambiguous even for directions below the [astronomical horizon](astronomical-horizon.md).

A concrete motivating observation is the Exploratorium Teacher Institute's Height Sight activity. Its [inclinometer](inclinometer.md) uses a sighting tube fixed to a card and an angular scale, with a string and small weight hanging from the scale's pivot. A partner reads where the freely hanging string meets the scale. Sighting a level target should give a readout near zero; sighting a taller target gives an angular height. The activity asks the observer to move closer and farther: the closer position gives the larger [angle](angle.md). The interpretation is that the readout measures the tube's tilt relative to the [gravity](gravity.md) reference, while converting that [angle](angle.md) to a physical height also requires distance and eye height. The activity also extends the [inclinometer](inclinometer.md) to sky observations. [Exploratorium Teacher Institute: Height Sight, construction, level check and distance-dependent angular observations](https://www.exploratorium.edu/snacks/height-sight).

The following calibration and sky sequence is a proposed extension, with no claimed observing dataset. First establish two reference marks at the same height with a water level, rather than assuming that a sloping floor or distant ridge is horizontal. Keep the [inclinometer](inclinometer.md) in a vertical [plane](plane.md), sight between the marks, wait for the weight to settle, and read the zero several times. Next sight a mark whose independently measured rise $q$ above the tube and horizontal separation $d$ are known; a [right triangle](right-triangle.md) predicts $\gamma_{\rm ref}=\arctan(q/d)$. A synthetic $q=3\,\mathrm m$, $d=5\,\mathrm m$ gives $\gamma_{\rm ref}=30.964^\circ$. Checking both zero and this nonzero [angle](angle.md) can reveal a wrongly attached tube or a scale read from the wrong end. Use level separation, not distance along inclined ground.

If the scale's indicated [altitude](altitude.md) is $m=\gamma_{\rm app}+b$, estimate its additive zero $b$ from the level sight, then obtain apparent [altitude](altitude.md) $\gamma_{\rm app}=m-b$. For synthetic readings $b=1.0^\circ$ and $m=32.0^\circ$, the corrected [altitude](altitude.md) is $31.0^\circ$, close to the $30.964^\circ$ calibration prediction. Declaring illustrative readout bounds of $0.5^\circ$ for each reading gives a conservative combined bound of $1.0^\circ$ on $m-b$; these bounds are assumptions, not measured performance. Repeatability tests the variation between readings, whereas a persistent zero offset remains a systematic [measurement error](measurement-error.md). Include uncertainty in the reference rise and separation before judging agreement.

At a fixed site, sight a recognizable [star](star.md), record the observation [time](time-in-physics.md), corrected [altitude](altitude.md) and north-through-east [azimuth](azimuth.md), and repeat over a short interval. Record the terrain boundary at the same [azimuth](azimuth.md) separately from the gravity-defined zero. The fixed-direction model in [horizontal coordinate system](horizontal-coordinate-system.md) predicts changing angular readouts as the [Earth](earth.md) rotates; this is a prospective test, rather than a fabricated measurement curve. Keep the tube aligned, the string free of contact and shielded from wind, the eye at the same reference position, and repeat the level check afterward. Timestamp each sight so genuine sky motion is not mistaken for poor repeatability. An [optical telescope](optical-telescope.md) with an angular readout can replace the sighting tube, but its mounting still needs an independently established level and angular zero.

The corrected instrument reads apparent [altitude](altitude.md), including [atmospheric refraction](atmospheric-refraction.md). Under ordinary conditions [atmospheric refraction](atmospheric-refraction.md) raises a low direction, so if $R$ is the upward angular correction, $\gamma_{\rm app}=\gamma_{\rm geom}+R$. Subtracting the instrument zero does not subtract $R$. Record site height, [temperature](temperature.md) and [pressure](pressure.md) if applying a [refraction](refraction.md) model: these are explicit observer inputs in the US Naval Observatory's NOVAS software. A coarse [inclinometer](inclinometer.md) may be unable to resolve the correction, and a local weather reading alone does not determine every atmospheric layer. [US Naval Observatory: NOVAS C3.0 user's guide, observer inputs and equ2hor refraction options](https://aa.usno.navy.mil/downloads/Circular_180C_C.pdf).

**Table of contents**

- [Inclinometer](inclinometer.md)

## ↑ Ancestors (5)

1. [Horizontal coordinate system](horizontal-coordinate-system.md)
2. [Astrophysics](astrophysics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Altazimuth mount](altazimuth-mount.md)
- [Altitude](altitude.md)
- [Astronomical horizon](astronomical-horizon.md)
- [Declination](declination.md)
- [Equatorial coordinate system](equatorial-coordinate-system.md)
- [Geographical latitude](geographical-latitude.md)
- [Horizontal coordinate system](horizontal-coordinate-system.md)
- [Inclinometer](inclinometer.md)
- [Meridian transit](meridian-transit.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/b/i/solution.md)
- [Zenith](zenith.md)
- [Zenith distance](zenith-distance.md)
