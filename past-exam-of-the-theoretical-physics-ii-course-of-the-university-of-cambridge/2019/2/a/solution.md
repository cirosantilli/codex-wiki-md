<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a real, central, short-range potential and elastic [quantum scattering](../../../../quantum-scattering-split.md). At large [radius](../../../../radius.md), normalize the stationary [wavefunction](../../../../wave-function-split.md) as

$$
\psi(\mathbf r)\sim e^{ikz}+f(\theta)\frac{e^{ikr}}r,
$$

where $k=\sqrt{2mE}/\hbar$ and $\theta$ is the [scattering angle](../../../../scattering-angle.md). Equal incoming and outgoing speeds give the [differential scattering cross-section](../../../../differential-scattering-cross-section.md) $d\sigma/d\Omega=|f(\theta)|^2$.

The [partial-wave scattering](../../../../partial-wave-scattering.md) expansion separates the [spherical harmonics](../../../../spherical-harmonic.md). The incident [plane wave](../../../../plane-wave.md) has expansion $\sum_{\ell\ge0}i^\ell(2\ell+1)j_\ell(kr)P_\ell(\cos\theta)$, with [Spherical Bessel functions](../../../../spherical-bessel-function.md) $j_\ell$ and [Legendre polynomials](../../../../legendre-polynomial.md) $P_\ell$. The regular radial solution outside the potential has asymptotic form $u_\ell\propto\sin(kr-\ell\pi/2+\delta_\ell)$. Its real [scattering phase shift](../../../../scattering-phase-shift.md) $\delta_\ell$ changes the ratio of outgoing to incoming waves to the [Partial-wave S-matrix](../../../../partial-wave-s-matrix.md) $S_\ell=e^{2i\delta_\ell}$. Matching outgoing coefficients yields

$$
\boxed{f(\theta)=\frac1{2ik}\sum_{\ell=0}^{\infty}(2\ell+1)(S_\ell-1)P_\ell(\cos\theta)
=\frac1k\sum_{\ell=0}^{\infty}(2\ell+1)e^{i\delta_\ell}\sin\delta_\ell P_\ell(\cos\theta).}
$$

Here $\ell$ labels the [orbital angular momentum](../../../../orbital-angular-momentum.md), with squared magnitude $\hbar^2\ell(\ell+1)$. The assumption of purely elastic scattering is what makes every $S_\ell$ have unit [modulus](../../../../modulus.md).

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
