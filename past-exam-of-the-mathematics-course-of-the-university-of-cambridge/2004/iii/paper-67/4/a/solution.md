<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define neutral-hydrogen [column density](../../../../../../column-density.md) along a ray by $N=\int n_{\rm HI}\,d\ell$, in atoms per unit area. The [neutral-hydrogen column-density distribution](../../../../../../neutral-hydrogen-column-density-distribution.md) per redshift is

$$
f_z(N,z)=\frac{\partial^2\mathcal N}{\partial N\,\partial z},
$$

so $f_z\,dN\,dz$ is the expected number of absorbers in those intervals along one sightline. A logarithmic column bin instead has distribution $N\ln(10)f_z$; the bin convention must be specified.

Let $n_c$ be a constant [comoving number density](../../../../../../comoving-number-density.md) and $\sigma_p$ a constant physical interception area. The corresponding physical [number density](../../../../../../number-density.md) is $n_p=n_c(1+z)^3$. Proper light-path length satisfies $d\ell=c|dt|=c\,dz/[(1+z)H(z)]$. The expected intersection count, or first-order probability in infinitesimal $dz$, is therefore

$$
\frac{d\mathcal N}{dz}=n_p\sigma_p\frac{d\ell}{dz}
=\frac{c n_c\sigma_p(1+z)^2}{H(z)}.
$$

The [Friedmann equation](../../../../../../friedmann-equations.md), the [constant-equation-of-state density scaling](../../../../../../constant-equation-of-state-density-scaling.md) for [pressureless matter](../../../../../../pressureless-matter.md), and the present [cosmological density parameters](../../../../../../cosmological-density-parameter.md) give

$$
H^2(z)=H_0^2\left[\Omega_m(1+z)^3+\Omega_\Lambda+\Omega_K(1+z)^2\right],
\qquad\Omega_m+\Omega_\Lambda+\Omega_K=1.
$$

Combining them yields the [absorber incidence and comoving number density](../../../../../../absorber-incidence-and-comoving-number-density.md) relation

$$
\boxed{\frac{d\mathcal N}{dz}\propto
\frac{(1+z)^2}{\sqrt{\Omega_m(1+z)^3+\Omega_\Lambda+\Omega_K(1+z)^2}}.}
$$

Here the constant cross-section is physical, as required for this result; a fixed comoving cross-section would instead decrease in physical area as $(1+z)^{-2}$. It is convenient to define [absorption distance](../../../../../../absorption-distance.md) by $dX/dz=(H_0/H(z))(1+z)^2$ and $f_X=f_z/(dX/dz)$, so a population with these non-evolution assumptions has constant incidence per $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
