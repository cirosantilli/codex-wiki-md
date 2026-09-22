<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a homologous star, [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), [mass conservation](../../../../../mass-conservation.md), and the [ideal gas](../../../../../ideal-gas.md) equation give the central scalings

$$
\rho_c\propto\frac M{R^3},
\qquad
P_c\propto\frac{GM^2}{R^4},
\qquad
T_c\propto\frac{\mu M}{R},
$$

where $\mu$ is the [mean molecular weight](../../../../../mean-molecular-weight.md). Integrating the nuclear energy-generation law over a fixed homologous profile gives

$$
L_{\rm nuc}\propto X\rho_cT_c^{13}M
\propto X\mu^{13}\frac{M^{15}}{R^{16}}.
$$

[Radiative stellar structure](../../../../../radiative-stellar-structure.md) gives independently

$$
L_{\rm rad}\propto\frac{R T_c^4}{\kappa\rho_c}
\propto\frac{\mu^4M^3}{\kappa}.
$$

Equating the two luminosities yields

$$
R^{16}\propto\kappa X\mu^9M^{12}.
$$

At fixed zero-age composition, the stars are therefore homologous with

$$
\boxed{R\propto M^{3/4}},
\qquad
\boxed{L\propto M^3}.
$$

The [effective temperature](../../../../../effective-temperature.md) satisfies $L=4\pi R^2\sigma T_e^4$, so $T_e\propto M^{3/8}$. The [zero-age main sequence](../../../../../zero-age-main-sequence.md) consequently has

$$
\boxed{\frac{d\log L}{d\log T_e}=8}.
$$

It is a steep line rising toward high luminosity and high temperature on a [Hertzsprung-Russell diagram](../../../../../hertzsprung-russell-diagram.md).

For fully ionized hydrogen and helium with $Y=1-X$,

$$
\frac1\mu=2X+\frac34Y=\frac{3+5X}{4},
$$

while $\kappa\propto1+X$. At fixed mass,

$$
\boxed{L\propto(1+X)^{-1}(3+5X)^{-4}},
$$

and the corresponding radius relation is

$$
\boxed{R\propto[X(1+X)]^{1/16}(3+5X)^{-9/16}}.
$$

At the pure-hydrogen zero-age point $X=1$,

$$
\frac{d\log L}{dX}=-\frac1{1+X}-\frac{20}{3+5X}=-3,
$$

whereas

$$
\frac{d\log R}{dX}=\frac1{16}\left(\frac1X+\frac1{1+X}-\frac{45}{3+5X}\right)=-\frac{33}{128}.
$$

Hence

$$
\frac{d\log T_e}{dX}
=\frac14\left(\frac{d\log L}{dX}-2\frac{d\log R}{dX}\right)
=-\frac{159}{256},
$$

and

$$
\boxed{\frac{d\log L}{d\log T_e}=\frac{256}{53}\simeq4.83}.
$$

As hydrogen is consumed, $X$ falls, so both $L$ and $T_e$ rise. In the usual diagram with temperature increasing leftward, the evolutionary track initially moves upward and leftward from the zero-age main sequence.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
