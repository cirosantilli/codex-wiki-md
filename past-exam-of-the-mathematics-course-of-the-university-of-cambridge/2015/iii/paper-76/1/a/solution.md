<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [time-harmonic wave](../../../../../../time-harmonic-wave.md) convention $\operatorname{Re}(\psi e^{-i\omega t})$, with a positive background [wavenumber](../../../../../../wavenumber.md) $k$. The scalar [Helmholtz equation](../../../../../../helmholtz-equation.md) for a constant-density acoustic model is

$$
 \psi_{xx}+\psi_{zz}+k^2n^2\psi=0.
$$

Writing $\psi=e^{ikx}E$ gives the exact envelope equation

$$
 E_{xx}+2ikE_x+E_{zz}+k^2(n^2-1)E=0.
$$

The [paraxial approximation](../../../../../../paraxial-approximation.md) neglects $E_{xx}$ relative to $2ikE_x$, giving the [parabolic wave equation](../../../../../../parabolic-wave-equation.md)

$$
\boxed{2ikE_x+E_{zz}+k^2(n^2-1)E=0,\qquad
E_x=\frac{i}{2k}E_{zz}+\frac{ik}{2}(n^2-1)E.}
$$

The choice of carrier and the direction of propagation matter: this is a forward, slowly varying envelope approximation. Sufficient scale conditions are $|E_{xx}|\ll2k|E_x|$, transverse spectral components $|p|\ll k$, and medium/envelope variation on longitudinal scales large compared with $1/k$. With the carrier fixed at the background $k$, small $|n-1|$ makes the refractive phase vary slowly too. Large-angle propagation, appreciable backscattering, or rapid longitudinal variation violates the approximation. Acoustic models with variable [mass density](../../../../../../density.md) can have additional gradient terms, so the scalar [Helmholtz equation](../../../../../../helmholtz-equation.md) itself is a model assumption. For the [Gaussian beam](../../../../../../gaussian-beam.md) in part (b), useful initial conditions are $kD\gg1$ and $D/|F|\ll1$, with the second condition absent for an initially uncurved beam. A narrow angular spectrum, rather than merely the label “Gaussian”, justifies the [paraxial approximation](../../../../../../paraxial-approximation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
