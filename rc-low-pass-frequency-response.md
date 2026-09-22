# RC low-pass frequency response

↑ **Parent:** [RC low-pass filter](rc-low-pass-filter.md)

Use the [complex amplitude](complex-amplitude.md) convention $v(t)=\operatorname{Re}(\widehat V e^{\mathrm i\omega t})$, where $\omega=2\pi f$ is the [angular frequency](angular-frequency.md) and $f$ is the [frequency](frequency.md) in cycles per second. Substitution into the [RC low-pass filter](rc-low-pass-filter.md) equation replaces the time [derivative](derivative.md) with multiplication by $\mathrm i\omega$, giving its [continuous-time frequency response](continuous-time-frequency-response.md)

$$
H(\omega)=\frac{\widehat V_{\rm out}}{\widehat V_{\rm in}}
=\frac1{1+\mathrm i\omega\tau},\qquad
|H|=\frac1{\sqrt{1+(\omega\tau)^2}},\qquad
\phi=\arg H=-\arctan(\omega\tau).
$$

Here $\phi$ is the output-minus-input [phase difference](phase-difference.md); a negative value means the output lags. Equivalently, the [voltage divider](voltage-divider.md) formed from the [electrical impedances](electrical-impedance.md) $R$ and $1/(\mathrm i\omega C)$ gives the same ratio. For an input $A\cos(\omega t)$, the sustained output is $A|H|\cos(\omega t+\phi)$ after the initial [exponential decay](exponential-decay.md) has died away.

Define the [cutoff frequency](cutoff-frequency.md) by a voltage [amplitude](wave-amplitude.md) ratio $1/\sqrt2$ relative to the low-[frequency](frequency.md) value:

$$
\omega_c=\frac1\tau,\qquad f_c=\frac1{2\pi\tau},\qquad
|H(\omega_c)|=\frac1{\sqrt2},\qquad \phi(\omega_c)=-\frac\pi4.
$$

On a [Bode plot](bode-plot.md), the voltage gain in [decibels](decibel.md) is

$$
G_{\rm dB}=20\log_{10}|H|=-10\log_{10}\left(1+(f/f_c)^2\right).
$$

At the [cutoff frequency](cutoff-frequency.md) it is $-3.0103\,\mathrm{dB}$, and far above that [frequency](frequency.md) it approaches a decrease of $20\,\mathrm{dB}$ per factor of ten in $f$. There is a smooth transition rather than an abrupt wall. The squared voltage ratio is one half at the corner; converting that statement to a [power](power.md) ratio requires the same real [electrical resistance](electrical-resistance.md) for the compared voltages. It does not mean that an unloaded [capacitor](capacitor.md) dissipates half the source [power](power.md).

For $R=2.2\,\mathrm{k}\Omega$ and $C=47\,\mathrm{nF}$, the [cutoff frequency](cutoff-frequency.md) is $f_c\approx1.5392\,\mathrm{kHz}$. A $1\,\mathrm V$ peak input at $0.1f_c$, $f_c$, and $10f_c$ produces peak output [amplitudes](wave-amplitude.md) of approximately $0.9950\,\mathrm V$, $0.7071\,\mathrm V$, and $0.09950\,\mathrm V$, with [phase differences](phase-difference.md) $-5.711^\circ$, $-45^\circ$, and $-84.289^\circ$. Thus a wanted oscillation at $0.1f_c$ is almost preserved while an unwanted one at $10f_c$ is reduced by about a factor of ten in voltage. The [superposition principle](superposition-principle.md) lets these two responses be added when both oscillations occur in the same [signal](signal.md).

## ↑ Ancestors (6)

1. [RC low-pass filter](rc-low-pass-filter.md)
2. [Low-pass filter](low-pass-filter.md)
3. [Linear filter](linear-filter.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Low-pass filter](low-pass-filter.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-d/d17/c/solution.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [RC low-pass step response](rc-low-pass-step-response.md)
- [Resistor-capacitor equilibrium noise](resistor-capacitor-equilibrium-noise.md)
