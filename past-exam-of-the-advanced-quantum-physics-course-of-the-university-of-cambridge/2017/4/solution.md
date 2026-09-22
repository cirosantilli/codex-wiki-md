<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For elastic scattering by the [Yukawa potential](../../../yukawa-potential.md), take $\kappa>0$ and use the [first Born approximation](../../../born-approximation.md) in the plane-wave normalization

$$
f_B(\mathbf q)=-\frac{m}{2\pi\hbar^2}\int e^{-i\mathbf q\cdot\mathbf r}V(r)\,d^3r.
$$

Choose the polar axis along the [momentum transfer](../../../momentum-transfer.md) $\hbar\mathbf q$. The angular integral is

$$
\int e^{-iqr\cos\vartheta}\,d\Omega
=2\pi\int_{-1}^{1}e^{-iqru}\,du
=4\pi\frac{\sin(qr)}{qr}.
$$

The radial volume element cancels the remaining powers of $r$, leaving

$$
f_B(q)=-\frac{2mA}{\hbar^2q}\int_0^\infty e^{-\kappa r}\sin(qr)\,dr
=-\frac{2mA}{\hbar^2(q^2+\kappa^2)}.
$$

For real $A$, the [differential scattering cross-section](../../../differential-scattering-cross-section.md) is therefore

$$
\boxed{\frac{d\sigma}{d\Omega}=|f_B(q)|^2
=\left[\frac{2mA}{\hbar^2(q^2+\kappa^2)}\right]^2}.
$$

This also has a finite forward limit when $\kappa>0$. The [Born amplitude for a Yukawa potential](../../../born-amplitude-for-a-yukawa-potential.md) provides a screened route to the [Coulomb potential](../../../coulomb-potential-energy.md) by taking $\kappa\to0^+$ at fixed $q>0$.

For an [alpha particle](../../../alpha-particle.md) of charge $2e$ scattering from a heavy nucleus of charge $Ze$, set $A=2Ze^2/(4\pi\epsilon_0)$. Neglect recoil, so that the reduced mass is approximately the projectile mass, $E=\hbar^2k^2/(2m)$, and elastic geometry gives

$$
q^2=|\mathbf k_{\rm out}-\mathbf k_{\rm in}|^2
=4k^2\sin^2\frac\theta2.
$$

The Coulomb-limit [scattering amplitude](../../../scattering-amplitude.md) becomes

$$
f_B(\theta)=-\frac{A}{4E\sin^2(\theta/2)}
=-\frac{Ze^2}{8\pi\epsilon_0E\sin^2(\theta/2)},
$$

which gives the [Rutherford differential cross-section](../../../rutherford-differential-cross-section.md)

$$
\boxed{\frac{d\sigma}{d\Omega}
=\left[\frac{Ze^2}{8\pi\epsilon_0E\sin^2(\theta/2)}\right]^2}.
$$

The unscreened [Coulomb potential](../../../coulomb-potential-energy.md) has long range, so taking this limit does not justify the [Born approximation](../../../born-approximation.md) for its full scattering state, particularly for a strongly charged target. The exact [Rutherford scattering](../../../rutherford-scattering.md) amplitude differs by a phase and has the same modulus. Thus the resulting [differential scattering cross-section](../../../differential-scattering-cross-section.md) remains applicable to the ideal nonrelativistic Coulomb problem beyond the weak-potential regime.

To relate the detector counts to the [atomic number](../../../atomic-number.md), first compute the number of target atoms per illuminated area. With molar mass $M=0.197\ \mathrm{kg\,mol^{-1}}$, the [number density](../../../number-density.md) integrated through the foil is

$$
\mathcal N=\frac{\rho tN_A}{M}
=\frac{(19.3\times10^3)(2.1\times10^{-7})(6.02214\times10^{23})}{0.197}
=1.239\times10^{22}\ \mathrm{m^{-2}}.
$$

The detector's transverse area is already its area normal to the scattered ray. Its small [solid angle](../../../solid-angle.md) is

$$
\Delta\Omega\simeq\frac{10^{-6}}{(10^{-2})^2}=10^{-2}\ \mathrm{sr}.
$$

There is no extra $\cos45^\circ$ factor: the foil is traversed normally and the detector area is transverse to its line of sight.

For a thin foil with negligible [multiple scattering](../../../multiple-scattering.md) and [energy](../../../energy-split.md) loss, the detected fraction is $f=\mathcal N(d\sigma/d\Omega)\Delta\Omega$. Thus the measurements imply

$$
\frac{d\sigma}{d\Omega}
=\frac{3.7\times10^{-7}}{(1.239\times10^{22})(10^{-2})}
=2.986\times10^{-27}\ \mathrm{m^2\,sr^{-1}}.
$$

Using $E=7.68\times10^6e\ \mathrm J=1.23047\times10^{-12}\ \mathrm J$ in the [Rutherford differential cross-section](../../../rutherford-differential-cross-section.md) gives

$$
Z=\frac{8\pi\epsilon_0 E\sin^2(22.5^\circ)}{e^2}
\sqrt{\frac{f}{\mathcal N\Delta\Omega}},\qquad
\boxed{Z\simeq85.4\approx85}.
$$

**The stated measurements do not reproduce gold's [atomic number](../../../atomic-number.md) 79 in this model.** The values and units above agree with the original PDF. Substituting $Z=79$ instead would predict $f\simeq3.17\times10^{-7}$ with the other inputs unchanged, rather than $3.7\times10^{-7}$. No stated correction accounts for that discrepancy; forcing the answer to 79 would require changing the data or adding an experimental correction not specified in the problem.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2017](../../2017-split.md)
3. [Past exam of the advanced quantum physics course of the University of Cambridge](../../split.md)
4. [Advanced Quantum Physics course of the University of Cambridge](../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
