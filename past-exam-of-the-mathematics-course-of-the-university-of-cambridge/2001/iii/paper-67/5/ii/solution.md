<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $q=\mathbf k\cdot\widehat{\mathbf n}$ and retain the negative-spatial-perturbation convention of the preceding part. Since $h=h_S$, the isotropic pieces of the supplied [Fourier mode](../../../../../../fourier-mode.md) contraction cancel:

$$
\left[\frac13h'\delta_{ij}
+\left(\widehat k_i\widehat k_j-\frac13\delta_{ij}\right)h'_S\right]
\widehat n_i\widehat n_j
=\frac{q^2}{k^2}h'.
$$

For $h=A(\mathbf k)\tau^2k^2$, the factor $1/2$ in the line-of-sight integral cancels the derivative's factor two. Thus

$$
\frac{\delta T}{T}
=\sum_{\mathbf k}A(\mathbf k)q^2
\int_{\tau_{\rm dec}}^{\tau_0}\tau e^{iq\tau}d\tau.
$$

An antiderivative convenient even at $q=0$ is

$$
\frac{d}{d\tau}\left[(1-iq\tau)e^{iq\tau}\right]
=q^2\tau e^{iq\tau}.
$$

It follows directly, or by two [integrations by parts](../../../../../../integration-by-parts.md), that

$$
\boxed{\frac{\delta T}{T}
=-\left[\sum_{\mathbf k}i(\mathbf k\cdot\widehat{\mathbf n})
A(\mathbf k)\tau e^{i\mathbf k\cdot\widehat{\mathbf n}\tau}
\right]_{\tau_{\rm dec}}^{\tau_0}
+\left[\sum_{\mathbf k}A(\mathbf k)
e^{i\mathbf k\cdot\widehat{\mathbf n}\tau}
\right]_{\tau_{\rm dec}}^{\tau_0}.}
$$

The source sign and both endpoint coefficients are fixed by the metric convention; no division by $q$ is needed.

To interpret the large-angle [Cosmic microwave background anisotropy](../../../../../../cosmic-microwave-background-anisotropy-split.md), restore the observer-centered propagation phase $e^{-iq\tau_0}$, which can equivalently be absorbed into the definition of each [Fourier mode](../../../../../../fourier-mode.md) amplitude. Put $D=\tau_0-\tau_{\rm dec}$. One mode contributes

$$
\Theta_{\mathbf k}(\widehat{\mathbf n})
=A(1-iq\tau_0)-A(1-iq\tau_{\rm dec})e^{-iqD}.
$$

The first term is a local angular monopole plus a dipole, so it is removed when discussing observed angular multipoles $\ell\ge2$. For modes outside the horizon at decoupling, $k\tau_{\rm dec}\ll1$, the higher-multipole emission signal is dominated by

$$
\boxed{\Theta_{\mathbf k,\ell\ge2}\simeq
-A(\mathbf k)e^{-i\mathbf k\cdot\widehat{\mathbf n}D}.}
$$

Its transfer amplitude has no leading positive power of $k$: the two explicit powers in $h$ have canceled in the integral. Projection onto the sky supplies [Spherical Bessel functions](../../../../../../spherical-bessel-function.md) $j_\ell(kD)$, with modes of order $kD\sim\ell$ contributing to each angular scale. This is the large-angle [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md); the emission velocity-like correction is relatively of order $k\tau_{\rm dec}$. For wavelengths much larger than the entire observed region, $kD\ll1$, removing the monopole and dipole leaves a signal starting at order $A(kD)^2$, rather than a finite observable anisotropy from a spatially uniform mode.

The stochastic scale dependence of $A(\mathbf k)$ is not specified by the deterministic metric solution. If one additionally assumes a scale-invariant primordial spectrum, $k^3P_A(k)=\text{constant}$, then

$$
C_\ell\ \propto\ \int_0^\infty\frac{dk}{k}\,j_\ell(kD)^2
=\frac1{2\ell(\ell+1)}
$$

for $\ell\ge1$, giving the familiar large-angle [Sachs-Wolfe plateau](../../../../../../sachs-wolfe-plateau.md), $\ell(\ell+1)C_\ell\simeq\text{constant}$, for the measured $\ell\ge2$ multipoles. A tilted primordial spectrum changes that trend. The full numerical temperature transfer also includes intrinsic last-scattering and Doppler terms, omitted from the stipulated metric-only integral.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
