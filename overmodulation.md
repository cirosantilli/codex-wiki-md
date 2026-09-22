# Overmodulation

↑ **Parent:** [Amplitude modulation](amplitude-modulation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Overmodulation)

For this single-tone [AM](amplitude-modulation.md) model, overmodulation means $m>1$. The signed factor $q(t)$ becomes negative whenever $\cos(\Omega t)<-1/m$. On such intervals,

$$
Aq(t)\cos(\omega_ct)=A|q(t)|\cos(\omega_ct+\pi).
$$

The sign reversal is a $\pi$ [radian](radian.md) shift of the carrier's [wave phase](phase-waves.md). At each zero of $q$, the [wave envelope](envelope-waves.md) vanishes and that phase is undefined. The waveform itself is continuous: the formula has not clipped it or created extra spectral lines.

At $m=1.4=7/5$, sign changes occur at message phases $\Omega t=\arccos(-5/7)$ and $2\pi-\arccos(-5/7)$ within each cycle. At the trough $\Omega t=\pi$, the desired signed factor is $-0.4$, whereas its nonnegative [wave envelope](envelope-waves.md) is $0.4A$. Ideal envelope recovery followed by subtraction of $A$ would give $-0.6A$ there, rather than the desired message voltage $-1.4A$. This is loss of polarity in the detector, not loss of the message from the full modulated signal. Actual transmitter clipping is a separate [signal distortion](signal-distortion.md) that can generate additional spectral components.

## ↑ Ancestors (3)

1. [Amplitude modulation](amplitude-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [AM modulation index](am-modulation-index.md)
- [Coherent demodulation](coherent-demodulation.md)
- [Envelope detector](envelope-detector.md)
