# Rutherford differential cross-section

↑ **Parent:** [Rutherford scattering](rutherford-scattering.md)

For an incident beam uniform across its relevant [impact parameters](impact-parameter.md), an incident [annulus](annulus-mathematics.md) has [area](surface-area.md) $d\sigma=2\pi b|db|$. Rotational symmetry maps it to outgoing [solid angle](solid-angle.md) $d\Omega=2\pi\sin\theta\,d\theta$. The [central-potential classical differential cross-section](central-potential-classical-differential-cross-section.md) and the [Rutherford impact-parameter relation](rutherford-impact-parameter-relation.md) therefore give

$$
\left|\frac{db}{d\theta}\right|=\frac a2\csc^2\frac\theta2,\qquad
\frac{d\sigma}{d\Omega}
=\frac{b}{\sin\theta}\left|\frac{db}{d\theta}\right|
=\frac{a^2}{4}\csc^4\frac\theta2
=\boxed{\frac{\kappa^2}{16E^2}\csc^4\frac\theta2}.
$$

This is a [differential scattering cross-section](differential-scattering-cross-section.md), with units of [area](surface-area.md) per [steradian](steradian.md), conventionally $\mathrm{m^2\,sr^{-1}}$, not a detector count and not an [area](surface-area.md) per degree. It applies for $0<\theta<\pi$, with a finite limiting value at $\pi$. Doubling incident [kinetic energy](kinetic-energy.md) divides it by four at fixed [angle](angle.md); doubling either [electric charge](electric-charge-split.md) number multiplies it by four.

A useful independent check integrates over all azimuths between two positive [angles](angle.md). For $0<\theta_1<\theta_2\leq\pi$,

$$
\sigma_{[\theta_1,\theta_2]}
=\int_{\theta_1}^{\theta_2}\frac{d\sigma}{d\Omega}\,2\pi\sin\theta\,d\theta
=\pi a^2\left(\cot^2\frac{\theta_1}{2}-\cot^2\frac{\theta_2}{2}\right).
$$

This equals the incident [annulus](annulus-mathematics.md) [area](surface-area.md) $\pi(b_1^2-b_2^2)$ directly. A detector covering only a small patch at one [angle](angle.md) does not collect this full azimuthal band.

**Table of contents**

- [Target normalization in Rutherford scattering rates](target-normalization-in-rutherford-scattering-rates.md)

## ↑ Ancestors (4)

1. [Rutherford scattering](rutherford-scattering.md)
2. [Atomic physics](atomic-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Born amplitude for a Yukawa potential](born-amplitude-for-a-yukawa-potential.md)
- [Geiger-Marsden angular-scattering experiment of 1913](geiger-marsden-angular-scattering-experiment-of-1913.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1/section-a/a4/solution.md)
- [Rutherford model](rutherford-model.md)
- [Target normalization in Rutherford scattering rates](target-normalization-in-rutherford-scattering-rates.md)
