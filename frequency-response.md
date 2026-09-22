# Frequency response

↑ **Parent:** [Linear time-invariant system](linear-time-invariant-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frequency_response)

The frequency response gives the change in [complex amplitude](complex-amplitude.md) of a sustained oscillation under a [linear time-invariant system](linear-time-invariant-system.md). If the [impulse response](impulse-response.md) is finite or has [absolute summability](absolute-convergence.md), substituting $x[n]=e^{\mathrm i\omega n}$ into its [discrete convolution](discrete-convolution.md) yields

$$
y[n]=\sum_jh[j]e^{\mathrm i\omega(n-j)}
=H(\omega)e^{\mathrm i\omega n},\qquad
H(\omega)=\sum_jh[j]e^{-\mathrm i\omega j}.
$$

Thus $|H(\omega)|$ is the amplitude gain and its [complex argument](argument-complex-analysis.md) is the phase change. Real sinusoids follow by taking real or imaginary parts. Here $\omega$ is radians per sample; $\omega=2\pi f$ for $f$ cycles per sample. A physical sampling rate converts that normalized frequency into cycles per second.

For a trailing [moving average](moving-average.md),

$$
H(\omega)=\frac1M\sum_{j=0}^{M-1}e^{-\mathrm i\omega j}
=e^{-\mathrm i\omega(M-1)/2}\frac{\sin(M\omega/2)}{M\sin(\omega/2)},
$$

with removable singularities evaluated from the finite sum. In particular $H(0)=1$. For $M=5$ and $\omega=2\pi/5$, the five [roots of unity](root-of-unity.md) sum to zero, so the oscillation is canceled. At small positive frequencies in the first pass region, the real sine ratio is positive and the phase factor gives a delay of $(M-1)/2$ samples.

<a id="image-moving-average-gain-curves-and-five-phase-contributions-that-cancel-at-one-frequency"></a>
![](moving-average-frequency-response.png)

**[Figure 23](#image-moving-average-gain-curves-and-five-phase-contributions-that-cancel-at-one-frequency). Moving-average gain curves and five phase contributions that cancel at one frequency**.

Increasing $M$ moves the first zero to $\omega=2\pi/M$, narrowing the main region of large gain. It does not create an ideal low-frequency cutoff: later side lobes transmit some higher-frequency components, and suppressing a component is only helpful when that component is unwanted. The frequency plot is the same operation as the delayed-sample average; the five-vector diagram explains one exact zero geometrically.

**Table of contents**

- [Antiresonance](antiresonance.md)

## ↑ Ancestors (4)

1. [Linear time-invariant system](linear-time-invariant-system.md)
2. [Signal processing](signal-processing.md)
3. [Electrical engineering](electrical-engineering-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Amplifier](amplifier.md)
- [Barkhausen pulse area](barkhausen-pulse-area.md)
- [Bode plot](bode-plot.md)
- [Continuous-time frequency response](continuous-time-frequency-response.md)
- [Cutoff frequency](cutoff-frequency.md)
- [Discrete-jump model of Barkhausen noise](discrete-jump-model-of-barkhausen-noise.md)
- [Effective noise bandwidth](effective-noise-bandwidth.md)
- [Einstein-de Haas experiment](einstein-de-haas-experiment.md)
- [Electrical engineering](electrical-engineering-split.md)
- [Electrical reactance](electrical-reactance.md)
- [Filtered shot noise](filtered-shot-noise.md)
- [Frequency modulation](frequency-modulation.md)
- [Impulse response](impulse-response.md)
- [Linear filter](linear-filter.md)
- [Linear time-invariant system](linear-time-invariant-system.md)
- [Moving average](moving-average.md)
- [Optical trap position readout](optical-trap-position-readout.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)
- [Patch clamp](patch-clamp.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [Relative attenuation by a linear filter](relative-attenuation-by-a-linear-filter.md)
- [Seismometer](seismometer.md)
- [Shot noise photocurrent measurement](shot-noise-photocurrent-measurement.md)
- [Signal processing](signal-processing.md)
- [Thermal noise spectral convention](thermal-noise-spectral-convention.md)
- [Thermodynamic and Rayleigh-Jeans antenna temperatures](thermodynamic-and-rayleigh-jeans-antenna-temperatures.md)
