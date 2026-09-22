<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $K>0$ and a positive central [mass density](../../../../../../density.md). For this [polytrope of index one](../../../../../../polytrope-of-index-one.md), the spherical [hydrostatic pressure support equation](../../../../../../hydrostatic-pressure-support-equation.md) becomes

$$
2K\rho\frac{d\rho}{dr}=-\frac{Gm\rho}{r^2},\qquad
r^2\frac{d\rho}{dr}=-\frac{Gm}{2K}.
$$

Differentiate the second equation and use mass conservation. With $k^2=2\pi G/K$, this gives

$$
\frac1{r^2}\frac{d}{dr}\left(r^2\frac{d\rho}{dr}\right)+k^2\rho=0.
$$

The regular central solution, with $\rho(0)=\rho_c$ and $\rho'(0)=0$, is

$$
\rho(r)=\rho_c\frac{\sin kr}{kr}.
$$

This is also the index-one solution of the [Lane-Emden equation](../../../../../../lane-emden-equation.md). The [mass density](../../../../../../density.md) remains positive up to its first zero, so the free surface is at $kR=\pi$, giving

$$
\boxed{R=\frac\pi k=\left(\frac{\pi K}{2G}\right)^{1/2}.}
$$

Taking a later zero would include a region of negative [mass density](../../../../../../density.md) and would not describe a physical star.

Integrating the mass gives

$$
M=\frac{4\pi\rho_c}{k^3}\int_0^\pi \xi\sin\xi\,d\xi
=\frac{4\pi^2\rho_c}{k^3}.
$$

Consequently

$$
\boxed{\frac{\overline\rho}{\rho_c}=\frac{3M}{4\pi R^3\rho_c}=\frac3{\pi^2}.}
$$

The radius is independent of the central [mass density](../../../../../../density.md), whereas the mass is proportional to it; this is the special [polytropic mass-radius relation](../../../../../../polytropic-mass-radius-relation.md) at index one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
