<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret the requested scale-dependent rms as the contribution from a logarithmic band of wavelengths, or equivalently a band centered at $k\sim R^{-1}$. A global uncut rms is not finite for this scale-free spectrum. The dimensionless density power per logarithmic wavenumber is

$$
\Delta_\delta^2(k)=\frac{k^3P(k)}{2\pi^2}=\frac{A}{2\pi^2}k^{n+3}.
$$

The [cosmological Poisson equation](../../../../../../cosmological-poisson-equation.md) gives $\varphi_{\mathbf k}=-(4\pi Ga^2\bar\rho)\delta_{\mathbf k}/k^2$. Therefore

$$
\boxed{\Delta_\varphi^2(k)=\frac{k^3P_\varphi(k)}{2\pi^2}
=\frac{A}{2\pi^2}(4\pi Ga^2\bar\rho)^2k^{n-1},\qquad
\varphi_{\rm rms}(R)\propto R^{(1-n)/2}.}
$$

This is the [potential fluctuations per logarithmic wavenumber](../../../../../../potential-fluctuations-per-logarithmic-wavenumber.md) scaling. A simple dimensional argument gives the same answer: the density amplitude on scale $R$ is proportional to $R^{-(n+3)/2}$, and its potential amplitude is of order $G\bar\rho(aR)^2\delta_R$, supplying two additional powers of $R$.

For $n=1$, the [Harrison-Zeldovich spectrum](../../../../../../harrison-peebles-zeldovich-spectrum.md) has scale-independent potential amplitude per logarithmic interval. If the density-spectrum amplitude grows as $A(t)=b^2(t)A_{\rm in}$, then $4\pi Ga^2\bar\rho=C/a$, so the potential amplitude evolves as $b/a$. It is constant in the pure growing matter mode of an [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md), where $b=a$.

A literal total variance would be proportional to $\int_0^\infty k^{n-2}\,dk$. Infrared convergence requires $n>1$ and ultraviolet convergence requires $n<1$, so no index makes both ends finite. At $n=1$ both divergences are logarithmic. Thus cutoffs or a band specification are essential for a numerical rms; the boxed statement describes the intended scale-local fluctuations rather than claiming a finite unsmoothed potential variance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
