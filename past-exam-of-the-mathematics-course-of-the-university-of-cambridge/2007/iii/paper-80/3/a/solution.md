<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use positive carrier [wavenumber](../../../../../../wavenumber.md) $k$ and retain waves traveling mainly in the positive $x$ direction. Factor out their rapid [wave phase](../../../../../../phase-waves.md) by writing $\psi=e^{ikx}E(x,z)$. Substitution into the [Helmholtz equation](../../../../../../helmholtz-equation.md) is exact and gives

$$
E_{xx}+2ikE_x+E_{zz}=0.
$$

For a transverse [Fourier mode](../../../../../../fourier-mode.md) $e^{i\nu z}$ at a small angle, $|\nu|/k\ll1$ and its forward longitudinal [wavenumber](../../../../../../wavenumber.md) is

$$
k_x=\sqrt{k^2-\nu^2}=k-\frac{\nu^2}{2k}+O(\nu^4/k^3).
$$

Thus the envelope varies along $x$ on scale $k/\nu^2$, much more slowly than the carrier wavelength, and $|E_{xx}|/|kE_x|=O(\nu^2/k^2)$. Dropping this smaller term derives the [parabolic wave equation](../../../../../../parabolic-wave-equation.md),

$$
\boxed{2ikE_x+E_{zz}=0,\qquad E_x=\frac{i}{2k}E_{zz}}.
$$

With transform $\widehat E(x,\nu)=\int E(x,z)e^{-i\nu z}dz$, its free propagation is

$$
\widehat E(x,\nu)=\widehat E(0,\nu)e^{-i\nu^2x/(2k)},\qquad
E(x,z)=\frac1{2\pi}\int\widehat E(0,\nu)e^{i\nu z-i\nu^2x/(2k)}d\nu.
$$

This is a one-way [paraxial approximation](../../../../../../paraxial-approximation.md), not a replacement for backward waves or large-angle Helmholtz components. Its [Fourier multiplier](../../../../../../fourier-multiplier.md) has unit [modulus](../../../../../../modulus.md) and therefore does not attenuate any admitted component.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
