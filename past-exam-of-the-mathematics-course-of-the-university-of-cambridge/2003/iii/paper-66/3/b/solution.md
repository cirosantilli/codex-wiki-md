<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\delta(\mathbf x)=\int\frac{d^3k}{(2\pi)^3}\delta_{\mathbf k}e^{-i\mathbf k\cdot\mathbf x},
\qquad
\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta_D^{(3)}(\mathbf k-\mathbf k')P(k).
$$

[Statistical homogeneity](../../../../../../statistical-homogeneity.md) makes the Fourier covariance diagonal, and isotropy makes the [matter power spectrum](../../../../../../matter-power-spectrum.md) depend only on $k=|\mathbf k|$. The [two-point correlation function](../../../../../../two-point-correlation-function.md) $\xi(r)=\langle\delta(\mathbf x)\delta(\mathbf x+\mathbf r)\rangle$ follows by inserting the transform and using this covariance:

$$
\xi(r)=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
$$

Integrating the polar angle relative to $\mathbf r$ gives $\int d\Omega_k\,e^{ikr\cos\theta}=4\pi\sin(kr)/(kr)$. Hence

$$
\boxed{\xi(r)=\frac1{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin(kr)}{kr}\,dk.}
$$

The inverse isotropic transform is $P(k)=4\pi\int_0^\infty r^2\xi(r)\sin(kr)/(kr)\,dr$ whenever these transforms exist, with distributions or regularization otherwise.

For a spherical average of comoving radius $R$, the [spherical top-hat window function](../../../../../../spherical-top-hat-window-function.md) is

$$
W(kR)=\frac{3[\sin(kR)-kR\cos(kR)]}{(kR)^3}.
$$

At a fixed epoch let $P(k)=Ak^n$. The [scale-free smoothed density variance](../../../../../../scale-free-smoothed-density-variance.md) is

$$
\sigma_\delta^2(R)=\frac{A}{2\pi^2}\int_0^\infty k^{n+2}W(kR)^2dk
=\frac{A R^{-(n+3)}}{2\pi^2}\int_0^\infty y^{n+2}W(y)^2dy.
$$

Thus the RMS fractional mass fluctuation scales as $R^{-(n+3)/2}$; the RMS mass fluctuation itself scales as $\bar\rho R^3\sigma_\delta\propto R^{(3-n)/2}$ at fixed epoch.

The comoving [Poisson equation](../../../../../../poisson-equation.md) gives $\Phi_{\mathbf k}=-4\pi G a^2\bar\rho\,\delta_{\mathbf k}/k^2$. For the growing irrotational mode the [linearized cosmological continuity equation](../../../../../../linearized-cosmological-continuity-equation.md) gives $\mathbf v_{\mathbf k}=-iaHf\,\mathbf k\delta_{\mathbf k}/k^2$, where $f=d\log D_+/d\log a$. The averaged-potential and bulk-velocity variances are therefore

$$
\sigma_\Phi^2=\frac{A(4\pi Ga^2\bar\rho)^2}{2\pi^2}\int_0^\infty k^{n-2}W(kR)^2dk,
\qquad
\langle|\mathbf V_R|^2\rangle=\frac{A(aHf)^2}{2\pi^2}\int_0^\infty k^nW(kR)^2dk.
$$

For a single Cartesian component of the isotropic bulk velocity, divide its variance by three. Rescaling $kR$ gives

$$
\boxed{\sigma_\delta\propto R^{-(n+3)/2},\qquad
\sigma_\Phi\propto R^{(1-n)/2},\qquad
\sigma_V\propto R^{-(n+1)/2}.}
$$

These are dimensional scaling laws, with an important convergence qualification. Since $W(y)\to1$ at small $y$ and has large-$y$ envelope $O(y^{-2})$, the density average converges for $-3<n<1$, the absolute potential average for $1<n<5$, and the bulk velocity for $-1<n<3$. No one unbroken power law makes all three absolute averages finite on the entire range $0<k<\infty$. In particular, long-wavelength modes can dominate the potential. Physical infrared/ultraviolet cutoffs, potential differences, or fluctuation amplitudes in a band around $k\sim R^{-1}$ resolve the relevant divergences; with cutoffs the simple powers need not describe the full integrated variance. The [scale-free potential and bulk-flow variance](../../../../../../scale-free-potential-and-bulk-flow-variance.md) laws should be understood with these conditions, not as a claim that divergent RMS integrals are finite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
