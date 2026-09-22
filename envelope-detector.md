# Envelope detector

↑ **Parent:** [Amplitude modulation](amplitude-modulation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Envelope_detector)

An envelope detector extracts the slowly varying nonnegative [wave envelope](envelope-waves.md) of a rapid [carrier wave](carrier-wave.md). In a simple electrical version a [diode](diode.md) charges a [capacitor](capacitor.md) near positive carrier peaks and an attached [resistor](resistor.md) discharges it between peaks. When $0\leq m<1$, ideal envelope extraction gives $E(t)=A[1+m\cos(\Omega t)]$; removing the constant $A$ leaves $Am\cos(\Omega t)$. This permits recovery without a synchronized carrier reference. Carrier injection thus trades transmitted [power](power.md) for simplicity.[Signals and Systems, Lecture 13: Continuous-Time Modulation, printed p. 13-2 and transparencies 13.17–13.19 on pp. 13-11–13-12: asynchronous recovery and injected carrier](continuous-time-modulation-by-alan-v-oppenheim.md)

A working peak detector needs margins as well as $m<1$: $E_{\min}=A(1-m)$ should comfortably exceed the [diode](diode.md)'s forward-voltage scale and [noise](noise-signal-processing.md), and the [time constant](time-constant.md) $\tau=RC$ must suppress carrier ripple while following a falling [wave envelope](envelope-waves.md). The coarse scale window is

$$
\frac{2\pi}{\omega_c}\ll\tau\ll\frac1\Omega.
$$

A [time constant](time-constant.md) that is too short leaves carrier ripple; one that is too long makes the discharging [capacitor](capacitor.md) fall more slowly than the envelope. In the ideal zero-drop, continuous-tracking approximation, following a falling $E$ requires $E/\tau\geq-E'$. For $0<m<1$,

$$
\max_{0<\theta<\pi}\frac{m\Omega\sin\theta}{1+m\cos\theta}
=\frac{m\Omega}{\sqrt{1-m^2}},\qquad
\tau\leq\frac{\sqrt{1-m^2}}{m\Omega}.
$$

Differentiating the ratio locates its maximum at $\cos\theta=-m$. This original slope check explains why operation near $m=1$ is demanding even before [overmodulation](overmodulation.md): the upper bound tends to zero while the need to smooth carrier cycles persists. It is an approximate circuit criterion, not a guarantee in the presence of [diode](diode.md) drops, loading or [noise](noise-signal-processing.md). At $m=0$ there is no varying message to track; at $m=1$ ideal envelope extraction remains algebraically possible, but the simple detector has no positive trough margin.

For $m>1$, even an ideal noiseless envelope detector returns $A|q(t)|$. Removing its mean or its original offset cannot restore the discarded sign. A more elaborate receiver can use the retained [wave phase](phase-waves.md) through [coherent demodulation](coherent-demodulation.md).

## ↑ Ancestors (3)

1. [Amplitude modulation](amplitude-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Amplitude modulation](amplitude-modulation.md)
- [Amplitude modulation laboratory](amplitude-modulation-laboratory.md)
- [Amplitude modulation sidebands](amplitude-modulation-sidebands.md)
- [Wireless telegraphy](wireless-telegraphy.md)
