<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Plane-parallel [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) gives $dP/dz=-\rho g$, while $d\tau=-\kappa\rho dz$. Hence

$$
\frac{dP}{d\tau}=\frac g\kappa.
$$

For $\kappa=\kappa_0P^{\alpha-1}T^{4-4\beta}$,

$$
\frac{d(P^\alpha)}{d\tau}
=\frac{\alpha g}{\kappa_0}T^{4\beta-4}.
$$

The grey-atmosphere relation from part (ii) can be written

$$
T^4=T_0^4\left(1+\frac32\tau\right),
\qquad
d\tau=\frac{2,d(T^4)}{3T_0^4}.
$$

Integrating from the zero-pressure top, where $T=T_0$, gives

$$
\boxed{P^\alpha=
\frac{2\alpha g}{3\kappa_0\beta T_0^4}
\left(T^{4\beta}-T_0^{4\beta}\right)}.
$$

The natural matching point to the stellar interior is the [photosphere](../../../../../../photosphere.md) $\tau=2/3$, where $T=T_e$ and $T_e^4=2T_0^4$. Multiplying the preceding expression by $\kappa_0T^{4-4\beta}/g$ then yields the [stellar surface boundary condition](../../../../../../stellar-surface-boundary-condition.md)

$$
\boxed{\frac{P\kappa}{g}
=\frac{4\alpha}{3\beta}\left(1-2^{-\beta}\right)}.
$$

The local relation $L_r=4\pi r^2\sigma T^4$ identifies this matching temperature with the local effective temperature.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
