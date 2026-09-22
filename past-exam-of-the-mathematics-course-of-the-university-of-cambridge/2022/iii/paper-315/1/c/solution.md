<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Deep in an optically thick [grey atmosphere](../../../../../../grey-atmosphere.md), write $I_\nu=B_\nu+\delta I_\nu$ and retain the first spatial-gradient correction in the transfer equation:

$$
\delta I_\nu\simeq-\frac{\mu}{\kappa\rho}
\frac{dB_\nu}{dz}.
$$

Angular and frequency integration then gives the [radiative diffusion](../../../../../../radiative-diffusion.md) flux

$$
F=-\frac{16\sigma T^3}{3\kappa\rho}\frac{dT}{dz}.
$$

For a thin [plane-parallel atmosphere](../../../../../../plane-parallel-atmosphere.md), constant [Rosseland mean opacity](../../../../../../rosseland-mean-opacity.md) $\kappa$, negligible external irradiation, and radius nearly equal to $R$, radiative equilibrium gives $F=L/(4\pi R^2)$. Therefore

$$
\boxed{\frac{dT}{dz}
=-\frac{3\kappa\rho L}{64\pi\sigma R^2T^3}}.
$$

With hydrostatic balance $dP/dz=-\rho g$, the equivalent pressure form is

$$
\boxed{\frac{dT}{dP}=\frac{3\kappa L}{64\pi\sigma GM\,T^3}},
$$

where $g=GM/R^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
