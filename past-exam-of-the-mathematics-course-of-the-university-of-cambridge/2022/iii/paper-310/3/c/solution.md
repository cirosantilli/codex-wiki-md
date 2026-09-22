<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The Fourier-space [cosmological Poisson equation](../../../../../../cosmological-poisson-equation.md) gives

$$
\phi(\mathbf k,\tau)
=-\frac{4\pi Ga^2\bar\rho_m}{k^2}\delta_m
=-\frac{3\Omega_{m,0}H_0^2}{2ak^2}\delta_m.
$$

Insert this into the line-of-sight expression for the [CMB lensing potential](../../../../../../cmb-lensing-potential.md), Fourier transform $\delta_m$, and use the [Rayleigh plane-wave expansion](../../../../../../rayleigh-plane-wave-expansion.md). Projection onto $Y_{lm}$ and spherical-harmonic orthogonality give

$$
\boxed{
a_{lm}^\psi=12\pi\Omega_{m,0}H_0^2i^{-l}
\int_0^{\chi_e}d\chi
\int\frac{d^3k}{(2\pi)^3}
\frac1{k^2}\frac{\chi_e-\chi}{\chi\chi_e}
\frac{\delta_m(\mathbf k,\tau)}{a(\tau)}
j_l(k\chi)Y_{lm}^*(\widehat{\mathbf k})}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
