# Photodiode responsivity measurement

↑ **Parent:** [Photodiode](photodiode.md)

Thorlabs' [silicon](silicon.md) FDS100 experiment sends a collimated, fibre-coupled [laser](laser-split.md) beam through a [beam splitter](beam-splitter.md) to the [photodiode](photodiode.md) and a reference [optical power meter](optical-power-meter.md). Varying reverse bias and [electrical load](electrical-load.md) tests linearity. The measured readout approaches saturation when its [electric potential difference](electric-potential-difference.md) consumes the bias.[Photodiodes, Lab Facts, Photodiode Saturation Limit and Noise Floor, opening experiment description and Figs. 1–3: reference power sensor, bias/load comparisons and saturation](photodiodes-by-thorlabs.md) A separate low-signal setup uses a $637\,\mathrm{nm}$ [laser](laser-split.md), [polarizers](polarizer.md), an [optical chopper](optical-chopper.md), [optical attenuators](optical-attenuator.md) and a [lock-in amplifier](lock-in-amplifier.md) inside a light-tight enclosure. These are actual apparatus choices, not the parameters of the constructed example above.[Photodiode Saturation and Noise Floor, p. 7 of 12, Experimental Design — Noise Floor: 637 nm source, polarizers, chopper, attenuation filters, lock-in readout and light-tight enclosure](photodiode-saturation-and-noise-floor-by-thorlabs.md)

For an independent [dark current](dark-current-physics.md) check, Thorlabs enclosed a [photodiode](photodiode.md) in nested metal boxes to exclude [light](light.md) and suppress interference, used a Keithley 6487 [ammeter](ammeter.md) supplying reverse bias, and monitored [temperature](temperature-split.md). Only one specimen per type was tested; the nearby temperature sensor did not directly contact the [semiconductor](semiconductor-split.md). Such a dark control measures the baseline but cannot certify [spectral responsivity](spectral-responsivity.md).[Photodiodes, Lab Facts, Dark Current as a Function of Temperature, Experimental Setup and Experimental Limitations: nested enclosure, ammeter and specimen/temperature limitations](photodiodes-by-thorlabs.md)

To infer [spectral responsivity](spectral-responsivity.md) at a selected [wavelength](wavelength.md), measure the [radiant flux](radiant-flux.md) actually reaching the test [photodiode](photodiode.md), rather than just the reference arm. A reference-arm [measurement calibration](measurement-calibration.md) must include the [beam splitter](beam-splitter.md) ratio and path losses. With signed readouts in one fixed orientation, subtract a beam-blocked baseline and use

$$
R(\lambda)=\frac{|I_{\rm light}-I_{\rm blocked}|}{P_{\rm test}},\qquad
R(\lambda)=\frac{|V_{\rm light}-V_{\rm blocked}|}{R_fP_{\rm test}}
$$

for direct [electric current](electric-current.md) readout or a calibrated linear [transimpedance amplifier](transimpedance-amplifier.md), respectively. Repeating at several incident [powers](power.md) tests whether this ratio is constant. Blocking only the source estimates ambient [light](light.md) plus electronic baseline; covering the detector excludes ambient [light](light.md) too. Their difference distinguishes optical background from [dark current](dark-current-physics.md) and readout offset. For a broad [optical spectrum](optical-spectrum.md), the ratio is a spectrum-weighted response, not generally $R$ at one [wavelength](wavelength.md).

For independent [Poisson distribution](poisson-distribution.md) collection, the [root mean square](root-mean-square.md) shot [noise](noise-signal-processing.md) in a one-sided rectangular [frequency](frequency.md) band of [signal bandwidth](signal-bandwidth.md) $B>0$ is

$$
i_{\rm shot}=\sqrt{2q(I_{\rm ph}+I_d)B},
$$

Here $I_d$ is reverse [dark current](dark-current-physics.md); [thermal electrical noise](thermal-electrical-noise.md) and amplifier [noise](noise-signal-processing.md) also contribute.[Si photodiodes, p. 6, §2-4, equations (2-4)–(2-7): independent thermal, dark-current and photocurrent noise terms](si-photodiodes-by-hamamatsu-photonics-k-k.md)

Subtracting a mean [dark current](dark-current-physics.md) removes its offset, not its fluctuations: subtracting a constant leaves the [variance](variance-split.md) unchanged. Consequently $I_{\rm ph}\gg I_d$ makes [dark current](dark-current-physics.md) shot [noise](noise-signal-processing.md) small relative to signal shot [noise](noise-signal-processing.md); it does not by itself establish high [signal-to-noise ratio](signal-to-noise-ratio.md). With an independently measured baseline, the [variance](variance-split.md) of that estimate must also be propagated. Increasing the measurement [signal bandwidth](signal-bandwidth.md) raises the admitted [noise](noise-signal-processing.md). Calibration of [wavelength](wavelength.md), reference [radiant flux](radiant-flux.md), readout gain and collection geometry, together with drift and linearity, determines what [measurement uncertainty](measurement-uncertainty.md) can be claimed.

## ↑ Ancestors (7)

1. [Photodiode](photodiode.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
