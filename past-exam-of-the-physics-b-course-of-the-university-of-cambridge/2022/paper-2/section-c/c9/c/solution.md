<h1 id="section-c/c9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The equilibrium [photon gas](../../../../../../photon-gas.md) is [isotropic](../../../../../../isotropy.md), so the [energy density](../../../../../../energy-density.md) per unit [solid angle](../../../../../../solid-angle.md) in a narrow angular-frequency interval is $u(T,\omega)d\omega/(4\pi)$. For rays making [angle](../../../../../../angle.md) $\theta$ with an outward surface normal, a surface element $dA$ is crossed in time $dt$ by rays initially in a [volume](../../../../../../volume.md) $c\,dt\,dA\cos\theta$. Only the outward hemisphere contributes. Thus

$$
e(T,\omega)=\frac{cu(T,\omega)}{4\pi}\int_0^{2\pi}d\phi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta
=\boxed{\frac{cu(T,\omega)}4}.
$$

The hemispherical restriction supplies a factor $1/2$ and the directional projection supplies another $1/2$. A small aperture in a cavity therefore emits this spectral [power](../../../../../../power.md) per unit area. A [blackbody](../../../../../../blackbody.md) at the same [temperature](../../../../../../temperature-split.md) emits the same amount: otherwise radiation exchange between it and the aperture would violate [thermal equilibrium](../../../../../../thermal-equilibrium-split.md).

Integrating [Planck's law](../../../../../../planck-s-law.md) over all positive [angular frequencies](../../../../../../angular-frequency.md) gives the total emitted [heat flux density](../../../../../../heat-flux-density.md)

$$
M(T)=\int_0^\infty e(T,\omega)\,d\omega
=\frac{\hbar}{4\pi^2c^2}\int_0^\infty\frac{\omega^3\,d\omega}{e^{\hbar\omega/(k_BT)}-1}.
$$

Set $x=\hbar\omega/(k_BT)$. Then

$$
M(T)=\frac{k_B^4T^4}{4\pi^2\hbar^3c^2}\int_0^\infty\frac{x^3\,dx}{e^x-1}.
$$

The remaining [integral](../../../../../../integral-split.md) is independent of [temperature](../../../../../../temperature-split.md), proving $M\propto T^4$. Its value follows by expanding $(e^x-1)^{-1}=\sum_{m=1}^\infty e^{-mx}$ and integrating termwise:

$$
\int_0^\infty\frac{x^3\,dx}{e^x-1}=\sum_{m=1}^\infty\frac6{m^4}=\frac{\pi^4}{15}.
$$

Consequently the [Stefan–Boltzmann law](../../../../../../stefan-boltzmann-law.md) is

$$
\boxed{M(T)=\sigma T^4,\qquad \sigma=\frac{\pi^2k_B^4}{60\hbar^3c^2}=5.67037\times10^{-8}\,\mathrm{W\,m^{-2}\,K^{-4}}.}
$$

This is emitted [power](../../../../../../power.md) alone. A body in a radiation environment also absorbs incoming radiation, which must be included when calculating net [radiative cooling](../../../../../../radiative-cooling.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C9](../../c9.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
