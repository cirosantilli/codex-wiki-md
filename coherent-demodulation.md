# Coherent demodulation

↑ **Parent:** [Amplitude modulation](amplitude-modulation.md)

Coherent demodulation recovers a message by multiplying the received [signal](signal.md) by a reference [carrier wave](carrier-wave.md) of the same [frequency](frequency.md) and known relative [wave phase](phase-waves.md), then passing the result through a [low-pass filter](low-pass-filter.md). For the ideal [AM](amplitude-modulation.md) model and reference $2\cos(\omega_ct+\varphi)$,

$$
2s(t)\cos(\omega_ct+\varphi)
=Aq(t)\cos\varphi+Aq(t)\cos(2\omega_ct+\varphi).
$$

A unity-gain ideal [low-pass filter](low-pass-filter.md) passing $0$ and $\Omega$ but rejecting $2\omega_c$ and $2\omega_c\pm\Omega$ leaves $Aq(t)\cos\varphi$. Such a separating cutoff exists because $\Omega<2\omega_c-\Omega$. At $\varphi=0$, subtraction of $A$ recovers $Am\cos(\Omega t)$ exactly for any finite $m\geq0$, including [overmodulation](overmodulation.md), provided the transmitter and channel preserve this linear waveform. This is the signed factor, not its [absolute value](absolute-value.md).

A constant phase error scales the recovered message by $\cos\varphi$: a $\pi/3$ [radian](radian.md) error halves it, and a $\pi/2$ error removes it. A known error with nonzero [cosine](cosine.md) can be compensated in gain; a frequency mismatch makes the relative [wave phase](phase-waves.md) drift and no longer gives constant attenuation. The lecture illustrates synchronous multiplication, filtering and phase error.[Signals and Systems, Lecture 13: Continuous-Time Modulation, transparencies 13.10–13.11 on pp. 13-7–13-8 and 13.16 on p. 13-10: multiplier, low-pass separation and phase-error cosine factor](continuous-time-modulation-by-alan-v-oppenheim.md)

## ↑ Ancestors (3)

1. [Amplitude modulation](amplitude-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Amplitude modulation](amplitude-modulation.md)
- [Envelope detector](envelope-detector.md)
