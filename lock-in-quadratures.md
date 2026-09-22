# Lock-in quadratures

↑ **Parent:** [Lock-in amplifier](lock-in-amplifier.md)

Let the input [electric potential difference](electric-potential-difference.md) be $s(t)=A\cos(\omega t+\phi)$, with peak [amplitude](wave-amplitude.md) $A\geq0$, [angular frequency](angular-frequency.md) $\omega>0$, and [phase difference](phase-difference.md) $\phi$ relative to $\cos\omega t$. For an observation [interval](interval-mathematics.md) $[0,T]$ containing an [integer](integer-split.md) number $N\geq1$ of cycles, each lasting one [period of a function](period-of-a-function.md), $T=2\pi N/\omega$, define the [lock-in quadratures](lock-in-quadratures.md) in a peak convention:

$$
X=\frac2T\int_0^T s(t)\cos\omega t\,dt,\qquad
Y=-\frac2T\int_0^T s(t)\sin\omega t\,dt.
$$

These [integrals](integral-split.md) average the products with dimensionless references $2\cos\omega t$ and $-2\sin\omega t$; $X$ and $Y$ have the input's units. The minus sign makes positive $\phi$ give positive $Y$. The [trigonometric functions](trigonometric-function.md) give

$$
\begin{aligned}
2s(t)\cos\omega t&=A\cos\phi+A\cos(2\omega t+\phi),\\
-2s(t)\sin\omega t&=A\sin\phi-A\sin(2\omega t+\phi).
\end{aligned}
$$

The oscillating terms have zero [integral](integral-split.md) over the stated [interval](interval-mathematics.md), proving $X=A\cos\phi$ and $Y=A\sin\phi$. Their [orthogonality](orthogonal-vectors.md) turns an oscillating [signal](signal.md) into two constant coordinates.

Represent those coordinates as a [vector](vector.md), or as the [complex number](complex-number.md) $Z=X+\mathrm iY$. Its [modulus](modulus.md) and [complex argument](argument-complex-analysis.md) recover the peak [amplitude](wave-amplitude.md) and [phase difference](phase-difference.md):

$$
R=\sqrt{X^2+Y^2}=A,\qquad
\phi=\operatorname{atan2}(Y,X)\pmod{2\pi},\qquad R>0.
$$

Here $\operatorname{atan2}(Y,X)$ selects the [angle](angle.md) with the correct signs of both coordinates, rather than applying the [arctangent](inverse-tangent.md) to $Y/X$ and losing the quadrant. When $X=Y=0$, the [amplitude](wave-amplitude.md) is zero and the [phase difference](phase-difference.md) is undefined. When $\phi=\pi/2$, $X=0$ despite a nonzero [signal](signal.md); measuring $Y$ prevents this blind spot. Rotating both references by a fixed [angle](angle.md) rotates the coordinate [vector](vector.md) but preserves $R$.

The factors of two above deliberately recover peak [amplitude](wave-amplitude.md). The SR830 instead reports the selected sinusoidal component in [root mean square](root-mean-square.md) units: in a calibrated, zero-offset display, $R_{\mathrm{rms}}=R/\sqrt2$. For $R=0.4\,\mathrm V$ this is $0.282843\,\mathrm V$, while the peak-to-peak span of that component is $0.8\,\mathrm V$. Display normalization, reference sign, gain and [angle](angle.md) units must be checked for the particular instrument.[Model SR830 DSP Lock-In Amplifier manual, printed p. 3-3, “RMS or Peak?” and “Degrees or Radians?”; pp. 3-13–3-14, output scaling and display offsets](model-sr830-dsp-lock-in-amplifier-manual-by-stanford-research-systems.md)

## ↑ Ancestors (7)

1. [Lock-in amplifier](lock-in-amplifier.md)
2. [Electronic amplifier](electronic-amplifier.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite-window lock-in response](finite-window-lock-in-response.md)
- [Lock-in harmonic rejection](lock-in-harmonic-rejection.md)
- [Lock-in quadratures](lock-in-quadratures.md)
