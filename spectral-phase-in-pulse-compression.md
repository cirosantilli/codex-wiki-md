# Spectral phase in pulse compression

↑ **Parent:** [Chirped pulse amplification](chirped-pulse-amplification.md)

Use a complex envelope $A(t)$ normalized so that $|A(t)|^2=P(t)$; its units are $\mathrm{W}^{1/2}$. The optical carrier convention is $e^{-i\omega_0t}$: the physical [electric field](electric-field-split.md) is proportional to the real part of $A(t)e^{-i\omega_0t}$ for a fixed transverse mode. With [angular frequency](angular-frequency.md) offset $\Omega=\omega-\omega_0$, fix the [Fourier transform](fourier-transform-split.md) convention

$$
\widetilde A(\Omega)=\int_{-\infty}^{\infty}A(t)e^{i\Omega t}\,dt,\qquad
A(t)=\frac{1}{2\pi}\int_{-\infty}^{\infty}\widetilde A(\Omega)e^{-i\Omega t}\,d\Omega.
$$

Write $\widetilde A=B e^{i\phi}$ with real $B\geq0$. A dispersive element adds [spectral phase](spectral-phase.md)

$$
\phi(\Omega)=\phi_0+\phi_1\Omega+\frac{\phi_2}{2}\Omega^2+\frac{\phi_3}{6}\Omega^3+\cdots.
$$

Constant [phase](phase-waves.md) rotates the envelope; the linear term delays it by $\phi_1$. The [group delay](group-delay.md) is $d\phi/d\Omega$. The quadratic coefficient $\phi_2$ is [group delay dispersion](group-delay-dispersion.md), abbreviated GDD, with units of time squared. Positive GDD makes higher [frequencies](frequency.md) arrive later with this convention. It is accumulated dispersion of a component; material [group velocity dispersion](group-velocity-dispersion.md) is its corresponding coefficient per unit length.

To undo a quadratic stretcher [spectral phase](spectral-phase.md), the compressor must supply opposite GDD. Include the amplifier and all intervening optics in the sum:

$$
\phi_{2,\rm total}=\phi_{2,\rm stretch}+\phi_{2,\rm amplifier}+\phi_{2,\rm compress}.
$$

Setting this sum to zero does not cancel [third-order dispersion](third-order-dispersion.md), $\phi_3$, or still higher orders. Residual [spectral phase](spectral-phase.md) can produce asymmetry and satellite pulses even when the quadratic term vanishes. A [diffraction grating](diffraction-grating.md) system can make path length depend on [frequency](frequency.md); matching the complete [spectral phase](spectral-phase.md) over the occupied spectrum is more demanding than merely choosing opposite quadratic coefficients.

There is a useful proof of what phase correction can accomplish. By [Parseval's identity](parseval-identity.md),

$$
U=\int |A|^2\,dt=\frac{1}{2\pi}\int B^2\,d\Omega.
$$

For a smooth decaying spectrum, the [Fourier transform](fourier-transform-split.md) of $tA$ is $-i\,d\widetilde A/d\Omega$. Consequently the power-weighted mean arrival time and [variance](variance-split.md) obey

$$
\bar t=\frac{\int B^2\phi'\,d\Omega}{\int B^2\,d\Omega},\qquad
\sigma_t^2=\frac{\int (B')^2\,d\Omega}{\int B^2\,d\Omega}
+\frac{\int B^2(\phi'-\bar t)^2\,d\Omega}{\int B^2\,d\Omega}.
$$

At fixed spectral amplitude, constant [group delay](group-delay.md) minimizes this [root mean square](root-mean-square.md) duration. Such a pulse is a [transform-limited pulse](transform-limited-pulse.md), up to a time shift and constant [phase](phase-waves.md). The nonnegative second term measures temporal broadening from unequal arrival times; the first term remains even after perfect phase correction.

## ↑ Ancestors (6)

1. [Chirped pulse amplification](chirped-pulse-amplification.md)
2. [Laser](laser-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
