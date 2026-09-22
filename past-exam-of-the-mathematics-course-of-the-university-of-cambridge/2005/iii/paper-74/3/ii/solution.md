<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [statistical homogeneity](../../../../../../statistical-homogeneity.md) and [statistical isotropy](../../../../../../statistical-isotropy.md), with the paper's finite-volume Fourier normalization,

$$
\xi(r)=\frac{V}{(2\pi)^3}\int d^3k\,P(k)e^{i\mathbf k\cdot\mathbf r}
=\frac{V}{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin kr}{kr}\,dk.
$$

The angular integral is $4\pi\sin(kr)/(kr)$. In particular $\xi(r)=\int\Delta^2(k)\sin(kr)/(kr)\,d\ln k$, confirming the stated [dimensionless power spectrum](../../../../../../dimensionless-cosmological-power-spectrum.md) normalization.

For the [scale-free matter power spectrum](../../../../../../scale-free-matter-power-spectrum.md) $P(k)=Ck^n$, set $u=kr$ to obtain

$$
\xi(r)=\frac{VC}{2\pi^2}r^{-n-3}I_n,
\qquad I_n=\int_0^\infty u^{n+1}\sin u\,du.
$$

At zero the integrand behaves as $u^{n+2}$, requiring $n>-3$; at infinity its oscillatory integral converges for $n<-1$. Thus in the ordinary convergent range $-3<n<-1$, the [scale-free density correlation transform](../../../../../../scale-free-density-correlation-transform.md) has

$$
I_n=\Gamma(n+2)\sin\frac{\pi(n+2)}2>0,
\qquad I_{-2}=\frac\pi2,
\qquad
\boxed{\gamma=n+3,\quad r_0^{\gamma}=\frac{VCI_n}{2\pi^2}.}
$$

The [gamma function](../../../../../../gamma-function.md) expression follows by introducing $e^{-\epsilon u}$, evaluating the complex Laplace integral where it converges absolutely at zero, and continuing within the convergent oscillatory range; its removable singularity at $n=-2$ is handled by the limit. Absolute convergence of the original correlation integral requires the smaller range $-3<n<-2$.

The exponent relation is a useful scaling statement beyond that interval, but a pure primordial $n\simeq1$ spectrum over all wavenumbers has no ordinary unsmoothed Fourier correlation integral. Physical transfer functions, cutoffs or smoothing must be specified, and a distributional extension need not yield a positive $r_0$ power law. Even within the convergent interval, the point variance is ultraviolet divergent without smoothing; the finite result here is at nonzero separation.

For a representative present-day ordinary galaxy sample over roughly $0.1$–$10\,h^{-1}\,\mathrm{Mpc}$, the familiar approximate fit is

$$
\boxed{r_0\simeq5\,h^{-1}\,\mathrm{Mpc},\qquad\gamma\simeq1.8,}
$$

where $H_0=100h\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$. These are empirical galaxy clustering parameters, not universal matter-spectrum constants; luminosity, color, selection and scale change the fit, as shown in [the galaxy correlation measurements](https://arxiv.org/abs/astro-ph/0408569). A formal power law of that slope corresponds to $n\simeq-1.2$ on those scales, not to the nearly scale-invariant primordial spectral index.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
