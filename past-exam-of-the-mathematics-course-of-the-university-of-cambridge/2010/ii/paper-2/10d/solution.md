<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

The [photon number density](../../../../../photon-number-density.md) is obtained by integrating the [Planck photon distribution](../../../../../planck-photon-distribution.md). With $x=h\nu/(kT)$,

$$
n=\frac{8\pi}{c^3}\int_0^\infty\frac{\nu^2\,d\nu}{e^{h\nu/(kT)}-1}
=\underbrace{\frac{8\pi k^3}{c^3h^3}\int_0^\infty\frac{x^2}{e^x-1}\,dx}_{\alpha}\,T^3.
$$

The integral converges, since its integrand is of order $x$ near zero and decays exponentially at infinity. Hence **$n=\alpha T^3$**, with $\alpha$ independent of temperature.

For equilibrium radiation undergoing [adiabatic expansion](../../../../../adiabatic-expansion.md), the total [entropy](../../../../../entropy.md) in a comoving volume is constant. Since the [entropy density](../../../../../entropy-density.md) is $\beta T^3$, this means $\beta T^3V$ is constant. A comoving volume scales as the cube of the [scale factor](../../../../../scale-factor-cosmology.md), so

$$
\boxed{T\propto V^{-1/3}\propto a^{-1}}.
$$

This agrees with the [cosmological redshift](../../../../../cosmological-redshift.md) of each photon frequency. The conclusion uses entropy conservation during the expansion.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
