<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $r_s^2=N^{-1}\int r^2n(r)\,dr$. The [effective droplet radius](../../../../cloud-droplet-effective-radius.md) and [shape factor](../../../../adiabatic-cloud-droplet-moments.md) give $r_e=r_v^3/r_s^2$ and $k^{1/3}=r_v/r_e$, so $r_s^2=k^{1/3}r_v^2$. If the [extinction](../../../../particle-extinction-coefficient.md) efficiency is approximately independent of [droplet](../../../../cloud-droplet.md) size over the distribution,

$$
\sigma_{\rm ext}=\pi Q_{\rm ext}Nr_s^2
=\pi Q_{\rm ext}k^{1/3}\left(\frac{3c_w}{4\pi\rho_w}\right)^{2/3}N^{1/3}h^{2/3}.
$$

For visible [wavelengths](../../../../wavelength.md) and [droplets](../../../../cloud-droplet.md) large compared with the [wavelength](../../../../wavelength.md), [geometrical optics](../../../../geometrical-optics-split.md) makes $Q_{\rm ext}\simeq2$ a useful approximation. Retaining it as the specified constant, and taking $N,k,c_w$ constant over the [cloud](../../../../cloud.md),

$$
\boxed{\tau_c=\int_0^H\sigma_{\rm ext}\,dh
=\frac35\pi Q_{\rm ext}k^{1/3}
\left(\frac{3c_w}{4\pi\rho_w}\right)^{2/3}N^{1/3}H^{5/3}.}
$$

The $3/5$ comes from integrating $h^{2/3}$; replacing the whole [cloud](../../../../cloud.md) by its cloud-top [extinction](../../../../particle-extinction-coefficient.md) would incorrectly omit it. The effective-radius relation treats the distribution shape through $k$, without assuming all [droplets](../../../../cloud-droplet.md) have the same size. Liquid phase, negligible vertical variation in that [shape factor](../../../../adiabatic-cloud-droplet-moments.md), and negligible departures from the adiabatic water profile are essential assumptions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
