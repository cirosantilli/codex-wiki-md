# Etendue bench measurement

↑ **Parent:** [Etendue](etendue.md)

A proposed [optical bench](optical-bench.md) test uses a steady illuminated diffuse patch, a relay made from two [optical lens](lens-optics.md) elements, interchangeable centred circular stops, and a calibrated [optical power meter](optical-power-meter.md) large enough to collect the whole output bundle. Start with small cone [angles](angle.md) so an ordinary relay approximates the [area-angle tradeoff](area-angle-tradeoff.md). Measure the patch's image [diameter](diameter.md) and the accepted angular extent at both conjugate planes; the [transverse magnification](transverse-magnification.md) gives the spatial scale, but does not by itself measure [etendue](etendue.md).

Map the local [radiance](radiance.md) with a baffled [photodiode](photodiode.md) on translation and rotation stages, using two small aligned holes to select a narrow known [solid angle](solid-angle.md). Keep the sampled position fixed while scanning direction, calibrate the sampling footprint and angular response, and repeat at several positions. Numerically integrate $n^2\cos\theta\,dA\,d\Omega$ over the occupied samples, and integrate $(L/n^2)dG$ to predict the collected [radiant flux](radiant-flux.md). This checks the filled-cone assumption instead of inferring it from two outer dimensions.

Compare the relay without a stop and with a stop of $0.6$ times the illuminated [diameter](diameter.md) in the same plane. The uniform-bundle prediction is a [radiant flux](radiant-flux.md) ratio of $0.36$, with unchanged local [radiance](radiance.md) in the surviving samples. Cover the input for a dark reading, monitor source drift, repeat the open-stop reading, check detector linearity with calibrated [optical attenuators](optical-attenuator.md), and enlarge the collecting detector or scan it to check for missed [light rays](light-ray.md). Lens losses, angular response, illumination gradients, alignment errors and [diffraction](diffraction.md) can spoil the ideal prediction; their effects must be measured separately. This is a procedure to try, with predicted readouts, not purported experimental data.

## ↑ Ancestors (6)

1. [Etendue](etendue.md)
2. [Geometrical optics](geometrical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
