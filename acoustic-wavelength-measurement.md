# Acoustic wavelength measurement

↑ **Parent:** [Wavelength](wavelength.md)

An [acoustic wavelength measurement](acoustic-wavelength-measurement.md) makes an invisible spatial pattern readable with a ruler. The authored guide [Interesting and inexpensive experiments for high school physics by Joe Wolfe](interesting-and-inexpensive-experiments-for-high-school-physics-by-joe-wolfe.md) places a loudspeaker near a pipe's open end, drives it with an oscillator, and slides a [microphone](microphone.md) attached to a metre rule through the pipe. An [oscilloscope](oscilloscope.md) or computer displays the [microphone](microphone.md) [signal](signal.md). Its oscillation [amplitude](wave-amplitude.md) rises and falls with position; adjacent minima locate [pressure](pressure.md) [nodes of a standing wave](node-physics.md) a distance $d=\lambda/2$ apart. A cap gives a [pressure](pressure.md) [antinode](antinode.md) at the closed end; an open end has a [pressure](pressure.md) node just outside it. These are [pressure](pressure.md) patterns, distinct from [displacement](displacement.md) patterns. The guide advises [wavelengths](wavelength.md) longer than the pipe diameter, sufficient pipe length to locate both a node and an [antinode](antinode.md), and [frequency spectrum](frequency-spectrum.md) analysis to distinguish the intended tone from other sounds.[pp. 10–11, Standing waves. Reflection and transmission. Speed of sound; apparatus, microphone scan, and pressure-node distinction](interesting-and-inexpensive-experiments-for-high-school-physics-by-joe-wolfe.md)

The inference follows from [superposition](superposition-principle.md) of two oppositely directed [acoustic plane waves](acoustic-plane-wave.md). In an ideal uniform, lossless pipe, taking equal [pressure](pressure.md) [amplitudes](wave-amplitude.md) $P$ and a rigid cap at $x=0$ gives

$$
p'(x,t)=P\cos(kx-\omega t)+P\cos(kx+\omega t)=2P\cos(kx)\cos(\omega t).
$$

The time-varying [pressure](pressure.md) perturbation $p'$ has local oscillation [amplitude](wave-amplitude.md) $2|P\cos(kx)|$. Its zeros are separated by $\pi/|k|=\lambda/2$. Unequal incident and reflected [amplitudes](wave-amplitude.md) leave nonzero minima, but their spacing remains $\lambda/2$ in this ideal model. A [microphone](microphone.md) detects that [pressure](pressure.md) variation through a changing electrical [signal](signal.md), rather than watching a [wave crest](wave-crest.md) move. Record the tone's [frequency](frequency.md) too, then infer [phase speed](phase-speed.md) $v_p=2fd$.

For proposed controls, keep the drive [frequency](frequency.md) and [amplitude](wave-amplitude.md) fixed during a scan, verify the [frequency](frequency.md) on the recorded [signal](signal.md), and repeat the scan in both directions. Fit several minimum positions $x_j=a+jd$ using [linear regression](linear-regression-split.md) to reduce dependence on one pair of positions. Check the ruler scale and use one consistent reference point on the [microphone](microphone.md). Compare with the source switched off to locate background [measurement noise](measurement-noise.md); use [frequency spectrum](frequency-spectrum.md) analysis to check for additional tones, and reduce drive if the trace ceases to resemble a [sinusoid](sinusoid.md). Record air [temperature](temperature.md) and avoid strong air motion. These are suggested controls, not additional procedures or observations attributed to the guide.

The pipe must support approximately [plane waves](plane-wave.md) over the measured region: transverse structure at shorter [wavelengths](wavelength.md), the [microphone](microphone.md)'s finite size, and disturbance by the ruler can compromise the interpretation. Weak reflection gives shallow minima, while [damping](damping.md) and other reflections can shift the extrema of the simple two-wave model. Measure interior spacings rather than assuming the first minimum is exactly at the pipe lip. A short scan may not include enough minima to estimate $d$ reliably, and drift during sequential scanning can imitate spatial variation.

For an explicitly hypothetical calculation, $f=1000\,\mathrm{Hz}$ and $d=0.1715\,\mathrm m$ give $\lambda=0.3430\,\mathrm m$, $K\simeq18.3183\,\mathrm{rad\,m^{-1}}$, and $v_p=343.0\,\mathrm{m\,s^{-1}}$. No such measurements are claimed here. If independent small [measurement errors](measurement-error.md) in $f$ and fitted $d$ have [standard deviations](standard-deviation.md) $\sigma_f$ and $\sigma_d$, first-order [error propagation](propagation-of-uncertainty.md) gives $\sigma_{v_p}/v_p\simeq\sqrt{(\sigma_f/f)^2+(\sigma_d/d)^2}$. A systematic scale error or changing air conditions requires separate assessment.

**Table of contents**

- [Oscilloscope](oscilloscope.md)
- [Propagation of uncertainty](propagation-of-uncertainty.md)

## ↑ Ancestors (8)

1. [Wavelength](wavelength.md)
2. [Wavenumber](wavenumber.md)
3. [Wave equation](wave-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Acoustic wavelength measurement](acoustic-wavelength-measurement.md)
- [Oscilloscope](oscilloscope.md)
