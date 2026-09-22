# Amplitude modulation

↑ **Parent:** [Electrical engineering](electrical-engineering-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Amplitude_modulation)

Amplitude modulation encodes a message by varying the multiplying [wave amplitude](wave-amplitude.md) of a [carrier wave](carrier-wave.md). Conventional [AM](amplitude-modulation.md) adds a positive constant before multiplication, allowing a simple [envelope detector](envelope-detector.md) to recover the message within its limits. Multiplication translates the message's [frequency spectrum](frequency-spectrum.md) into a band around the carrier, adapting a slow message to a faster channel. This is an application of the [modulation property of the Fourier transform](modulation-property-of-the-fourier-transform.md).[Signals and Systems, Lecture 13: Continuous-Time Modulation, printed pp. 13-1–13-2: channel matching, spectrum translation, carrier injection and demodulation](continuous-time-modulation-by-alan-v-oppenheim.md)

For an original single-message-[frequency](frequency.md) voltage model, choose

$$
s(t)=A[1+m\cos(\Omega t)]\cos(\omega_ct),\qquad
A>0,\quad 0<\Omega<\omega_c,\quad m\geq0.
$$

Here $t$ is time, $A$ is the peak voltage [amplitude](wave-amplitude.md) of the unmodulated [carrier wave](carrier-wave.md), $\omega_c$ is its [angular frequency](angular-frequency.md), $\Omega$ is the message [angular frequency](angular-frequency.md), and $m$ is the dimensionless [AM modulation index](am-modulation-index.md). The message shape is $\cos(\Omega t)$; $m$ measures how deeply it changes the multiplying factor. Define the signed factor $q(t)=1+m\cos(\Omega t)$. The nonnegative [wave envelope](envelope-waves.md) of the representation $z(t)=Aq(t)e^{\mathrm i\omega_ct}$ is

$$
E(t)=|z(t)|=A|q(t)|.
$$

The instantaneous voltage $s(t)$ crosses zero every carrier cycle, even when $E(t)$ is large. Its value at one time, its [wave envelope](envelope-waves.md), and its carrier-component [amplitude](wave-amplitude.md) are three different quantities. The narrow-envelope intuition additionally needs $\Omega\ll\omega_c$; the algebraic model only assumes $\Omega<\omega_c$.

<a id="image-am-waveform-signed-modulation-factor-and-envelope-before-and-after-overmodulation"></a>
![](amplitude-modulation-envelope-and-phase-reversal.png)

**[Figure 6](#image-am-waveform-signed-modulation-factor-and-envelope-before-and-after-overmodulation). AM waveform, signed modulation factor and envelope before and after overmodulation**. Original voltage model with $\omega_c/\Omega=20$ and $m=0.5$ or $1.4$. Orange curves bound the waveform by $\pm|q|$; the purple dashed curve is the signed $q$. Shading marks negative $q$, where the carrier phase reverses. These are calculated curves, not oscilloscope traces or detector measurements.

The beauty is that two views reveal different parts of the same operation. In time, the message appears to ride on the oscillations. In the [frequency spectrum](frequency-spectrum.md), [amplitude modulation sidebands](amplitude-modulation-sidebands.md) show it as a pair of translated components. An [envelope detector](envelope-detector.md) reads their combined shape without needing the carrier's [wave phase](phase-waves.md); [coherent demodulation](coherent-demodulation.md) instead uses a synchronized reference and preserves the signed factor.

**Table of contents**

- [Single-sideband modulation](single-sideband-modulation.md)
- [AM modulation index](am-modulation-index.md)
- [Amplitude modulation sidebands](amplitude-modulation-sidebands.md)
  - [Fourier filtering of overlapping amplitude-modulation sidebands](fourier-filtering-of-overlapping-amplitude-modulation-sidebands.md)
- [Overmodulation](overmodulation.md)
- [Envelope detector](envelope-detector.md)
- [Coherent demodulation](coherent-demodulation.md)
- [Amplitude modulation laboratory](amplitude-modulation-laboratory.md)
- [Suppressed-carrier amplitude modulation](suppressed-carrier-amplitude-modulation.md)

## ↑ Ancestors (2)

1. [Electrical engineering](electrical-engineering-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Frequency modulation](frequency-modulation.md)
- [Holographic wavefront reconstruction](holographic-wavefront-reconstruction.md)
- [Radio communication](radio-communication.md)
- [Single-sideband modulation](single-sideband-modulation.md)
