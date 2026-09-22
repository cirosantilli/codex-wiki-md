# Frequency modulation

↑ **Parent:** [Electrical engineering](electrical-engineering-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frequency_modulation)

Frequency modulation carries a message by changing the [instantaneous frequency](instantaneous-frequency.md) of a [carrier wave](carrier-wave.md). In the ideal model the [wave amplitude](wave-amplitude.md) stays constant: information changes the rate at which the [wave phase](phase-waves.md) advances. Write a real electrical [signal](signal.md) and its chosen complex representation as

$$
s(t)=A\cos\phi(t),\qquad z(t)=Ae^{\mathrm i\phi(t)},\qquad A>0.
$$

The [wave envelope](envelope-waves.md) in this representation has [modulus](modulus.md) $|z(t)|=A$ throughout, although $s(t)$ continually passes through zero. A smaller instantaneous value of $s(t)$ therefore does not mean a smaller [wave amplitude](wave-amplitude.md). The continuously unwrapped [wave phase](phase-waves.md) $\phi$ is measured in [radians](radian.md); its [derivative](derivative.md) is an [angular frequency](angular-frequency.md), while division by $2\pi$ gives [frequency](frequency.md) in cycles per second, or [hertz](hertz.md).

For a message $m(t)$ expressed as an [electric potential difference](electric-potential-difference.md), an ideal [voltage-controlled oscillator](voltage-controlled-oscillator.md) has sensitivity $K_f$ in [hertz](hertz.md) per volt and obeys

$$
f_i(t)=f_c+K_fm(t),\qquad
\phi(t)=\phi(0)+2\pi f_ct+2\pi K_f\int_0^t m(\tau)\,d\tau.
$$

The [integral](integral-split.md) is essential: putting the message directly into the [wave phase](phase-waves.md) gives [phase modulation](phase-modulation.md), whose [instantaneous frequency](instantaneous-frequency.md) instead depends on the message's [derivative](derivative.md). [Amplitude modulation](amplitude-modulation.md) changes the multiplying [wave amplitude](wave-amplitude.md). These are different ways to encode the same kind of message [signal](signal.md).

An original slow illustration uses $f_c=20\,\mathrm{Hz}$, message [frequency](frequency.md) $f_m=1\,\mathrm{Hz}$, [frequency deviation](frequency-deviation.md) $\Delta f=5\,\mathrm{Hz}$, and [FM modulation index](fm-modulation-index.md) $\beta=5$. With zero initial [wave phase](phase-waves.md),

$$
\phi(t)=2\pi\cdot20t+5\sin(2\pi t),\qquad
s(t)=A\cos\bigl(2\pi\cdot20t+5\sin(2\pi t)\bigr),\qquad
f_i(t)=20+5\cos(2\pi t).
$$

Here $t$ is in seconds. The [instantaneous frequency](instantaneous-frequency.md) stays positive, between $15$ and $25\,\mathrm{Hz}$; the [wave phase](phase-waves.md) always advances. The oscillations bunch up where $f_i$ is large and spread out where it is small, while the [wave envelope](envelope-waves.md) remains at $A$.

<a id="image-constant-amplitude-and-changing-cycle-spacing-in-a-frequency-modulated-carrier"></a>
![](frequency-modulation-waveform-and-instantaneous-frequency.png)

**[Figure 8](#image-constant-amplitude-and-changing-cycle-spacing-in-a-frequency-modulated-carrier). Constant amplitude and changing cycle spacing in a frequency-modulated carrier**. Original illustration with $f_c=20\,\mathrm{Hz}$, $f_m=1\,\mathrm{Hz}$, $\Delta f=5\,\mathrm{Hz}$ and $\beta=5$. The upper bounds are $s/A=\pm1$, not measured data; the lower curve is the exact derivative of the specified wave phase.

This separation is useful in a receiver: changing a positive multiplying [wave amplitude](wave-amplitude.md) does not change the zero crossings of $\cos\phi$, so their timing still carries the message. [Noise](noise-signal-processing.md) that moves those crossings, a vanishing [wave amplitude](wave-amplitude.md), and [frequency response](frequency-response.md) distortion can still damage it. The surprising beauty of [FM](frequency-modulation.md) is that a constant [wave envelope](envelope-waves.md) can conceal a rich [frequency spectrum](frequency-spectrum.md): the components interfere to change timing instead of the envelope's height.

**Table of contents**

- [Instantaneous frequency](instantaneous-frequency.md)
- [Frequency deviation](frequency-deviation.md)
- [FM modulation index](fm-modulation-index.md)
- [Single-tone FM sidebands](single-tone-fm-sidebands.md)
- [Narrowband frequency modulation](narrowband-frequency-modulation.md)
- [Frequency modulation laboratory](frequency-modulation-laboratory.md)

## ↑ Ancestors (2)

1. [Electrical engineering](electrical-engineering-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Radio communication](radio-communication.md)
- [Single-molecule absorption in a molecular crystal](single-molecule-absorption-in-a-molecular-crystal.md)
- [Voltage-controlled oscillator](voltage-controlled-oscillator.md)
