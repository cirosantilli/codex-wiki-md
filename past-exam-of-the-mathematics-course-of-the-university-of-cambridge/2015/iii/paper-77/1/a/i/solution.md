<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $r=|\mathbf x|$, $n_i=x_i/r$, and let the source have size $\ell$. The [retarded acoustic Green function](../../../../../../../retarded-acoustic-green-function.md) gives the outgoing solution of [Lighthill acoustic analogy](../../../../../../../lighthill-acoustic-analogy.md) as

$$
\rho'(\mathbf x,t)=\frac1{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int\frac{T_{ij}(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{|\mathbf x-\mathbf y|}\,d^3y.
$$

This follows by integrating the source derivatives by parts in the retarded convolution. Assume the source is localized and the boundary terms vanish. In the [acoustic compact-source approximation](../../../../../../../acoustic-compact-source-approximation.md), $k_0\ell\ll1$, the retardation across the source can be neglected, while $r\gg\ell$ permits replacement of the denominator by $r$. The integral becomes $S_{ij}(t-r/c_0)/r$.

In the radiation region $k_0r\gg1$, derivatives of the retarded argument dominate derivatives of the spreading factor. Since $\partial_{x_i}(t-r/c_0)=-n_i/c_0$, the leading [acoustic quadrupole](../../../../../../../acoustic-quadrupole.md) field is

$$
\boxed{\rho'(\mathbf x,t)\sim\frac{n_in_j\ddot S_{ij}(t-r/c_0)}{4\pi c_0^4r}=\frac{x_ix_j\ddot S_{ij}(t-r/c_0)}{4\pi c_0^4r^3}.}
$$

The two negative retardation derivatives give a positive sign. This is a far-field approximation, with smaller near-field terms omitted.

For low-[Mach number](../../../../../../../mach-number.md) aerodynamic fluctuations of speed $U$ and advective time $\ell/U$, take $T_{ij}=O(\rho_0U^2)$, $S_{ij}=O(\rho_0U^2\ell^3)$, and two time derivatives of order $(U/\ell)^2$. Therefore

$$
\boxed{\frac{\rho'}{\rho_0}=O\left[\left(\frac U{c_0}\right)^4\frac\ell r\right]=O(m^4\ell/r).}
$$

The quoted fourth power is the [compact acoustic quadrupole Mach-number scaling](../../../../../../../compact-acoustic-quadrupole-mach-number-scaling.md), with geometric spreading shown explicitly. It assumes the source strength and time scale just stated; the source must be acoustically compact, and the observation point must remain in the radiation region.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 77](../../../../paper-77-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
