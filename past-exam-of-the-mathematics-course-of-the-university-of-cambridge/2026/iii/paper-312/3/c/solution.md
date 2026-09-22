<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On wavelengths much larger than halos, all matter is partitioned among halos. The mass-weighted halo overdensity must therefore equal the matter overdensity. Since $\delta_h(M)=b(M)\delta_m$, [mass conservation](../../../../../../mass-conservation.md) requires

$$
\int_0^\infty dM\,\frac{dn}{dM}\frac{M}{\bar\rho}b(M)=1.
$$

For the [Press-Schechter formalism](../../../../../../press-schechter-formalism.md), the mass-fraction measure becomes

$$
f(\nu)d\nu=\sqrt{\frac2\pi}e^{-\nu^2/2}d\nu,
\qquad \nu\geq0.
$$

It is normalized and is a half-normal distribution, so

$$
\int_0^\infty f(\nu)d\nu=1,
\qquad
\int_0^\infty\nu^2f(\nu)d\nu=1.
$$

Using the [linear Eulerian halo bias](../../../../../../linear-eulerian-halo-bias.md)

$$
b=1+b_L=1+\frac{\nu^2-1}{\delta_c}
$$

therefore gives

$$
\int_0^\infty f(\nu)b(\nu)d\nu
=1+\frac{1-1}{\delta_c}=1,
$$

which verifies the consistency relation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
