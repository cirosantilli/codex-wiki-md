# Finite-window lock-in response

↑ **Parent:** [Lock-in amplifier](lock-in-amplifier.md)

An observation [interval](interval-mathematics.md) of finite duration is not an infinitely sharp [frequency](frequency.md) selector. Combine the [lock-in quadratures](lock-in-quadratures.md) into

$$
Z_T=\frac2T\int_0^T s(t)e^{-\mathrm i\omega t}\,dt.
$$

For unwanted [electric potential difference](electric-potential-difference.md) $s(t)=B\cos((\omega+\delta)t+\psi)$, where $\delta$ is an [angular frequency](angular-frequency.md) offset and $\omega+\delta>0$, expansion into [complex exponentials](complex-exponential-function.md) gives the exact response

$$
\begin{aligned}
Z_T&=Be^{\mathrm i\psi}F_T(\delta)
+Be^{-\mathrm i\psi}F_T(-(2\omega+\delta)),\\
F_T(\nu)&=\frac1T\int_0^T e^{\mathrm i\nu t}\,dt
=e^{\mathrm i\nu T/2}\operatorname{sinc}(\nu T/2),\\
\operatorname{sinc}(x)&=\begin{cases}\sin x/x,&x\ne0,\\1,&x=0.\end{cases}
\end{aligned}
$$

The [sinc function](sinc-function.md) formula follows by integrating the [exponential function](exponential-function.md) and factoring $e^{\mathrm i\nu T}-1=2\mathrm i e^{\mathrm i\nu T/2}\sin(\nu T/2)$; its value at zero follows from a [limit](limit-of-a-function.md). The first term changes slowly after multiplication; the second oscillates at the sum [frequency](frequency.md). It vanishes at exact matching when $T$ is an [integer](integer-split.md) number of reference cycles, each lasting one [period of a function](period-of-a-function.md), but cannot generally be discarded in a short-window calculation.

For $|\delta|\ll\omega$ and many reference cycles, the first term usually dominates: its [modulus](modulus.md) is $B|\operatorname{sinc}(\delta T/2)|$ and its [complex argument](argument-complex-analysis.md) includes $\delta T/2$. Thus $|\delta|T\ll1$ gives almost no rejection. A longer observation separates closer [frequencies](frequency.md), with the first zeros of this term at $|\delta|=2\pi/T$. Those zeros are not a brick-wall cutoff: the [sinc function](sinc-function.md) has nonzero lobes beyond them. At $\delta=0$ a synchronized contribution remains however large $T$ becomes.

<a id="image-lock-in-quadratures-preserve-phase-difference-a-finite-interval-limits-rejection"></a>
![](lock-in-quadratures-and-window-response.png)

**[Figure 6](#image-lock-in-quadratures-preserve-phase-difference-a-finite-interval-limits-rejection). Lock-in quadratures preserve phase difference; a finite interval limits rejection**. Original calculated geometry and responses, not measurements. Left: $X=0.2\,\mathrm V$, $Y=0.2\sqrt3\,\mathrm V$, $R=0.4\,\mathrm V$, $\phi=60^\circ$; the dotted [vector](vector.md) shows an added synchronized $0.1\,\mathrm V$ contribution. Right: exact $|Z_T|/B$ for $\psi=0$ and $T$ equal to four reference cycles, against dimensionless detuning $(f-f_0)T$. The dashed curve keeps only the difference-frequency term. Their difference shows why the sum-frequency term matters for a short observation.

For a numerical check, use $f_0=1\,\mathrm{Hz}$, $T=4\,\mathrm s$, $\psi=0$ and an unwanted [frequency](frequency.md) $f=1.125\,\mathrm{Hz}$. Then $(f-f_0)T=1/2$ and the exact expression gives

$$
\frac{|Z_T|}{B}=\frac2\pi-\frac2{17\pi}=\frac{32}{17\pi}\approx0.599172,
$$

whereas the difference-frequency term alone gives $2/\pi\approx0.636620$. An interference [amplitude](wave-amplitude.md) $B=0.9\,\mathrm V$ therefore contributes $0.539254\,\mathrm V$ to $|Z_T|$ in this constructed example. A nearby [frequency](frequency.md) can survive strongly even though the three-times-frequency component in [lock-in harmonic rejection](lock-in-harmonic-rejection.md) cancels exactly.

A practical [lock-in amplifier](lock-in-amplifier.md)'s [low-pass filter](low-pass-filter.md) weights past products differently from this rectangular observation [interval](interval-mathematics.md). Its [time constant](time-constant.md) and roll-off determine near-reference rejection and [settling time](settling-time.md); narrowing detection slows the response.[Model SR830 DSP Lock-In Amplifier manual, printed p. 3-2, “Narrow band detection”; pp. 3-11–3-12, time constants and filter roll-off](model-sr830-dsp-lock-in-amplifier-manual-by-stanford-research-systems.md)

## ↑ Ancestors (7)

1. [Lock-in amplifier](lock-in-amplifier.md)
2. [Electronic amplifier](electronic-amplifier.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Chopped-light lock-in experiment](chopped-light-lock-in-experiment.md)
