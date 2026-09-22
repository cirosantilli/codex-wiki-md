# Continuous-time frequency response

↑ **Parent:** [Transfer function](transfer-function.md)

The [continuous-time frequency response](continuous-time-frequency-response.md) is the [frequency response](frequency-response.md) of a continuous-time [linear time-invariant system](linear-time-invariant-system.md). From zero initial state, a [BIBO stable](bounded-input-bounded-output-stability.md) system driven by a sustained [sinusoid](sinusoid.md) $u(t)=A\cos(\omega t)$ approaches the steady response

$$
y_{\mathrm{ss}}(t)=A|G(i\omega)|\cos\bigl(\omega t+\arg G(i\omega)\bigr).
$$

Any decaying initial or switching transient is separate. The [modulus](modulus.md) $|G(i\omega)|$ is the amplitude gain; the [complex argument](argument-complex-analysis.md) is the shift in [oscillation phase](phase-waves.md). Thus evaluating a [transfer function](transfer-function.md) at $s=i\omega$ measures both how much of an oscillation passes through and how far it lags.

For the [first-order low-pass filter](first-order-low-pass-filter.md), with $K>0$, direct [complex number](complex-number.md) arithmetic gives

$$
G(i\omega)=\frac{K}{1+i\omega\tau},\qquad
|G(i\omega)|=\frac{K}{\sqrt{1+(\omega\tau)^2}},\qquad
\arg G(i\omega)=-\arctan(\omega\tau).
$$

The phase uses the [inverse tangent](inverse-tangent.md) branch between $-\pi/2$ and $\pi/2$. Low [angular frequencies](angular-frequency.md) have gain close to $K$ and little lag. High [angular frequencies](angular-frequency.md) have gain approximately $K/(\omega\tau)$ and lag approaching $\pi/2$. This is why the model is a [first-order low-pass filter](first-order-low-pass-filter.md): it suppresses fast variation compared with slow variation. Rowell relates [frequency response](frequency-response.md) gain and phase to [poles](pole.md) and then introduces [Bode plots](bode-plot.md) in [MIT 2.004, lecture 32, sections 1 and 2](https://www.ocw.mit.edu/courses/2-004-dynamics-and-control-ii-spring-2008/2a0a97261561177bf1a91b07202bb09a_lecture_32.pdf).

At the corner [angular frequency](angular-frequency.md),

$$
\omega_c=\frac1\tau,\qquad |G(i\omega_c)|=\frac K{\sqrt2},\qquad
\arg G(i\omega_c)=-\frac\pi4.
$$

For $K=2$ and $\tau=3\,\mathrm{s}$, $\omega_c=1/3\,\mathrm{rad}\,\mathrm{s}^{-1}$, the gain is $\sqrt2\approx1.4142$, and the lag is $45$ degrees. The [angular frequency](angular-frequency.md) $\omega$ is measured in [radians](radian.md) per second; ordinary [frequency](frequency.md) $f$ is measured in hertz (cycles per second), with $\omega=2\pi f$. Consequently the same corner is $f_c=1/(2\pi\tau)\approx0.0531\,\mathrm{Hz}$, not $1/3\,\mathrm{Hz}$.

<a id="image-bode-plot-of-the-first-order-low-pass-filter-with-k-2-and-tau-3-mathrm-s"></a>
![](first-order-transfer-frequency-response.png)

**[Figure 12](#image-bode-plot-of-the-first-order-low-pass-filter-with-k-2-and-tau-3-mathrm-s). Bode plot of the first-order low-pass filter with $K=2$ and $\tau=3\,\mathrm{s}$**. Gain and [oscillation phase](phase-waves.md) are plotted against [angular frequency](angular-frequency.md) on a logarithmic horizontal axis. The vertical line marks $\omega_c=1/3\,\mathrm{rad}\,\mathrm{s}^{-1}$, where the gain is $\sqrt2$ and the phase is $-45$ degrees. The gain panel shows $20\log_{10}|G(i\omega)|$; its corner is $3.01$ decibels below the low-frequency gain.

**Table of contents**

- [Bode plot](bode-plot.md)

## ↑ Ancestors (5)

1. [Transfer function](transfer-function.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Continuous-time frequency response](continuous-time-frequency-response.md)
- [RC low-pass frequency response](rc-low-pass-frequency-response.md)
- [RC low-pass output loading](rc-low-pass-output-loading.md)
- [Transfer function](transfer-function.md)
