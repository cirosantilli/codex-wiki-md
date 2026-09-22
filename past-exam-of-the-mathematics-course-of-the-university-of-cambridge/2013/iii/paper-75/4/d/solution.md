<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\rho=\rho_0+\delta\rho$ and retain quadratic fluctuations in the smooth zero-winding sector. The [quadratic density-phase action](../../../../../../quadratic-density-phase-action.md) is

$$
S_2=\int\left[\frac g2(\delta\rho)^2+i\delta\rho\,\partial_\tau\phi+\frac{|\nabla\delta\rho|^2}{8m\rho_0}+\frac{\rho_0}{2m}|\nabla\phi|^2\right].
$$

At wavelengths long compared with the [healing length](../../../../../../healing-length.md), drop the density-gradient term. Completing the square gives

$$
\frac g2(\delta\rho)^2+i\delta\rho\,\partial_\tau\phi
=\frac g2\left(\delta\rho+\frac{i\partial_\tau\phi}g\right)^2+\frac{(\partial_\tau\phi)^2}{2g}.
$$

The real Gaussian density integral, or its equivalent contour shift, contributes only a field-independent [determinant](../../../../../../determinant.md). Absorb that normalization and the uniform saddle action into $S_0$. To this quadratic long-wave accuracy,

$$
\boxed{Z\simeq e^{-S_0}\int\mathcal D\phi\,e^{-S_{\rm eff}},\qquad
S_{\rm eff}=\frac12\int_0^\beta d\tau\int d^dr\left[\frac1g(\partial_\tau\phi)^2+\frac{\rho_0}m|\nabla\phi|^2\right].}
$$

The Gaussian extension of $\delta\rho$ to the full real line is a fluctuation approximation around positive $\rho_0$; it is not an exact replacement of the global density constraint. The compact field's vortex/winding sectors also lie beyond this smooth-phonon integral.

The [Bose-gas phase-only action](../../../../../../bose-gas-phase-only-action.md) is a continuum harmonic chain with Euclidean inverse propagator $\omega_n^2/g+\rho_0k^2/m$. Continuing to real frequency gives

$$
\boxed{E_k\sim c_s|k|,\qquad c_s=\sqrt{g\rho_0/m}=\sqrt{\mu/m}.}
$$

Restoring $\hbar$ gives $E_k\sim\hbar c_s|k|$ for a [wavenumber](../../../../../../wavenumber.md) $k$. This is the [phonon](../../../../../../phonon.md) branch of the [Bogoliubov spectrum](../../../../../../bogoliubov-quasiparticle-dispersion.md). Keeping the omitted density-gradient term replaces $g$ by $g+k^2/(4m\rho_0)$ and yields $E_k^2=c_s^2k^2+k^4/(4m^2)$ in the adopted units, so the full quadratic spectrum is $\sqrt{\epsilon_k(\epsilon_k+2g\rho_0)}$ with $\epsilon_k=k^2/(2m)$.

The phase-only action also tests the condensate assumption. At zero temperature its equal-time phase variance has an infrared contribution $\int d^dk/|k|$, logarithmically divergent in one dimension; at positive temperature the zero Matsubara mode gives $\int d^dk/k^2$, divergent in dimensions at or below two. Thus this same low-energy theory exposes the regimes where the mean-field condensate cannot describe true thermodynamic long-range order. It permits a finite infrared fluctuation at zero temperature for $d\ge2$ and at positive temperature for $d>2$, within the remaining weak-coupling assumptions.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
