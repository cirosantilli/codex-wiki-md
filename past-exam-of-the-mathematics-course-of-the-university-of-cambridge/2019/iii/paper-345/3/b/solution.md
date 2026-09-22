<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the kinematic fluxes $q=Q/(\pi\rho_0)$, $m=M/(\pi\rho_0)$ and $f_0=F_0/(\pi\rho_0)$. In the steady [Boussinesq approximation](../../../../../../boussinesq-approximation.md), the [non-Boussinesq top-hat plume equations](../../../../../../non-boussinesq-top-hat-plume-equations.md) reduce to

$$
q'=2\alpha\sqrt m,\qquad m'=\frac{f_0q}{m},\qquad f=f_0.
$$

Eliminating $z$ gives $m^{5/2}=5f_0q^2/(8\alpha)$, where the integration constant vanishes for a [pure plume](../../../../../../pure-plume.md) from a point source. Write $b=az$ and $w=Kz^{-1/3}$. The two balances give $a=6\alpha/5$ and $K^3=3f_0/(4a^2)=25f_0/(48\alpha^2)$. The [Boussinesq point-source plume](../../../../../../boussinesq-point-source-plume.md) is therefore

$$
\boxed{b(z)=\frac{6\alpha}{5}z,\qquad
w(z)=\left(\frac{25f_0}{48\alpha^2z}\right)^{1/3},\qquad
 g'(z)=\frac43K^2z^{-5/3},\qquad
\rho(z)=\rho_0\left(1-\frac{g'(z)}g\right).}
$$

Here $q=a^2Kz^{5/3}$ and $m=a^2K^2z^{4/3}$ tend to zero at the source, while $f_0$ remains positive. The plume [Froude number](../../../../../../froude-number.md) is independent of height:

$$
\boxed{C_p^2=\frac{w^2}{g'b}=\frac5{8\alpha}.}
$$

The ideal point source is a far-field similarity idealization. Since $g'\propto z^{-5/3}$, the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) fails near $z=0$ and is valid only when $g'/g\ll1$. In terms of $K$, this requires $z\gg[4K^2/(3g)]^{3/5}$; the density formula must not be extrapolated into its unphysical negative-density region.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
