<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use one [spectral resolution element](../../../../spectral-resolution-element.md), $\Delta\nu=0.5\,\mathrm{cm}^{-1}$, and assume comparable angular resolution horizontally and vertically, so the pixel [solid angle](../../../../solid-angle.md) is $\Omega\simeq\theta^2=6.67\times10^{-6}\,\mathrm{sr}$. The question specifies only the vertical angle; without an assumption about horizontal field of view the diameter is not unique. Interpret throughput $\eta=0.5$ as dimensionless transmission. With primary collecting area $A_p=\pi d^2/4$, the power in that element is

$$
P_s=\eta B_\nu\Delta\nu\,A_p\Omega
=1.30\times10^{-7}A_p\,\mathrm W,
$$

when $A_p$ is in square metres. There is no extra factor of $\pi$ multiplying the supplied [spectral radiance](../../../../spectral-radiance.md).

For an integration time $t=1$ s, the order-of-magnitude [effective noise bandwidth](../../../../effective-noise-bandwidth.md) is $\Delta f\simeq1/t=1$ Hz. The root-mean-square [noise-equivalent power](../../../../noise-equivalent-power.md) is then $P_n={\rm NEP}\sqrt{\Delta f}=5\times10^{-11}$ W.[p. 1, NEP Definition; p. 2, equations (2)–(3): minimum power and averaging time](../../../../nep-noise-equivalent-power-by-thorlabs.md) A [signal-to-noise ratio](../../../../signal-to-noise-ratio.md) of 10 requires $P_s=5\times10^{-10}$ W, and therefore

$$
\boxed{A_p\simeq3.84\times10^{-3}\,\mathrm{m^2},\qquad d\simeq7.0\,\mathrm{cm}.}
$$

An ideal rectangular average of a one-sided white [noise](../../../../noise-signal-processing.md) spectral density has $\Delta f=1/(2t)$, giving $d\simeq5.9$ cm instead. A circular field with diameter $\theta$ changes the diameter by another order-unity factor. These convention choices all require an aperture substantially larger than the $9.5$ mm [diffraction](../../../../diffraction.md) estimate, so signal collection is the stronger constraint. The estimate treats the quoted NEP as applicable to the reconstructed channel; a detailed [Fourier transform spectroscopy](../../../../fourier-transform-spectroscopy.md) design would also specify scan weighting, background and how interferogram noise propagates into that channel.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
