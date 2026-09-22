# Lock-in harmonic rejection

↑ **Parent:** [Lock-in amplifier](lock-in-amplifier.md)

Consider this original constructed input [electric potential difference](electric-potential-difference.md), with $t$ in seconds and $f_0=1\,\mathrm{Hz}$:

$$
s(t)=(0.4\,\mathrm V)\cos(2\pi f_0t+\pi/3)
+(0.9\,\mathrm V)\cos(6\pi f_0t+\pi/5).
$$

The unwanted component has three times the reference [frequency](frequency.md) and more than twice the wanted peak [amplitude](wave-amplitude.md). Nevertheless, the [lock-in quadratures](lock-in-quadratures.md) over $T=4/f_0=4\,\mathrm s$ are exactly

$$
X=0.4\cos(\pi/3)\,\mathrm V=0.2\,\mathrm V,\qquad
Y=0.4\sin(\pi/3)\,\mathrm V=0.2\sqrt3\,\mathrm V\approx0.34641016\,\mathrm V,
$$

so $R=0.4\,\mathrm V$ and $\operatorname{atan2}(Y,X)=\pi/3=60^\circ$. This is a peak [amplitude](wave-amplitude.md) calculation, not an SR830 display prediction.

To see why the larger component vanishes, multiply $B\cos(3\omega t+\psi)$ by each reference:

$$
\begin{aligned}
2B\cos(3\omega t+\psi)\cos\omega t
&=B\cos(2\omega t+\psi)+B\cos(4\omega t+\psi),\\
-2B\cos(3\omega t+\psi)\sin\omega t
&=B\sin(2\omega t+\psi)-B\sin(4\omega t+\psi).
\end{aligned}
$$

Each [sinusoid](sinusoid.md) has zero [average value of a function](average-value-of-a-function.md) over a whole reference cycle. More generally, a component $B\cos(n\omega t+\psi)$ with [integer](integer-split.md) $n\geq2$ gives products at $(n-1)\omega$ and $(n+1)\omega$, whose [integrals](integral-split.md) vanish over any [integer](integer-split.md) number of reference cycles. This is the [orthogonality](orthogonal-vectors.md) behind selecting a [Fourier coefficient](fourier-coefficient.md) with sinusoidal references. A nonsinusoidal reference can contain additional [frequencies](frequency.md) and need not have the same rejection property.

<a id="image-lock-in-harmonic-rejection-multiplication-reveals-a-constant-component"></a>
![](lock-in-multiplication-and-averaging.png)

**[Figure 5](#image-lock-in-harmonic-rejection-multiplication-reveals-a-constant-component). Lock-in harmonic rejection: multiplication reveals a constant component**. Original calculated waveforms for the declared $0.4\,\mathrm V$ wanted component and $0.9\,\mathrm V$ interference; no measured data. Top: input and wanted [signal](signal.md). Middle: products with the two dimensionless references. Bottom: running [lock-in quadratures](lock-in-quadratures.md); markers at complete reference cycles equal $X=0.2\,\mathrm V$, $Y=0.2\sqrt3\,\mathrm V$. Partial-cycle estimates need not equal those values.

An unwanted component at the reference [frequency](frequency.md) survives. If $u(t)=B\cos(\omega t+\psi)$ is added to the input, its coordinate [vector](vector.md) adds to the wanted one:

$$
Z=Ae^{\mathrm i\phi}+Be^{\mathrm i\psi}.
$$

For example, adding $B=0.1\,\mathrm V$ with $\psi=0$ to the wanted component gives $X=0.3\,\mathrm V$, $Y=0.2\sqrt3\,\mathrm V$, $R=\sqrt{0.21}\,\mathrm V\approx0.458258\,\mathrm V$, and [phase difference](phase-difference.md) $\operatorname{atan2}(0.2\sqrt3,0.3)\approx49.1066^\circ$. Longer averaging cannot separate these two synchronized contributions.

## ↑ Ancestors (7)

1. [Lock-in amplifier](lock-in-amplifier.md)
2. [Electronic amplifier](electronic-amplifier.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Finite-window lock-in response](finite-window-lock-in-response.md)
- [Lock-in harmonic rejection](lock-in-harmonic-rejection.md)
