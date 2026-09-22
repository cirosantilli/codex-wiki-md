<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [conservation of energy](../../../../../../conservation-of-energy.md) to use here is the total [kinetic energy](../../../../../../kinetic-energy.md) plus [internal energy](../../../../../../internal-energy.md) inside the shock, not just the internal energy of a uniform-pressure core. With no radiative loss and negligible initial ambient energy,

$$
\dot Et=4\pi\int_0^{R(t)}\left(\frac12\rho u^2+\frac{p}{\gamma-1}\right)r^2\,dr.
$$

Substitute the [adiabatic superbubble similarity solution](../../../../../../adiabatic-superbubble-similarity-solution.md) and define the finite positive dimensionless integral

$$
I=\int_0^1\left(\frac12f(\eta)h(\eta)^2+\frac{g(\eta)}{\gamma-1}\right)\eta^2\,d\eta.
$$

Then $\dot Et=4\pi\rho_1\dot R^2R^3I$. Since $\dot R=3R/(5t)$ and $R^5=\alpha^5(\dot E/\rho_1)t^3$,

$$
\dot Et=\frac{36\pi}{25}\alpha^5\dot Et\,I,
\qquad\boxed{\alpha=\left(\frac{25}{36\pi I}\right)^{1/5}.}
$$

This is the [energy normalization of a continuously driven spherical shock](../../../../../../energy-normalization-of-a-continuously-driven-spherical-shock.md). It fixes $\alpha$ once the similarity profiles are determined. If the profiles describe only the shocked ambient layer, the energy of the interior hot bubble must also be included before using this normalization. A radiatively cooled shell has a different energy budget; its familiar numerical coefficient should not be substituted into this loss-free model.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
