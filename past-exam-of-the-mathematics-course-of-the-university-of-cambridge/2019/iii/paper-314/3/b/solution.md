<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The remaining [magnetic field](../../../../../../magnetic-field.md) has $\mathbf B=B_\phi(R)\mathbf e_\phi+B_z(R)\mathbf e_z$. The radial [Lorentz force density](../../../../../../lorentz-force-density.md) separates into a [magnetic pressure](../../../../../../magnetic-pressure.md) gradient and inward [magnetic tension](../../../../../../magnetic-tension.md):

$$
\frac1{4\pi}[(\nabla\times\mathbf B)\times\mathbf B]_R
=-\frac1{8\pi}\frac{d(B_z^2+B_\phi^2)}{dR}-\frac{B_\phi^2}{4\pi R}.
$$

Here $(\mathbf B\cdot\nabla)\mathbf B$ has radial component $-B_\phi^2/R$ because $\partial_\phi\mathbf e_\phi=-\mathbf e_R$. Thus [magnetostatic equilibrium](../../../../../../magnetostatic-equilibrium.md) gives

$$
\frac d{dR}\left(p+\frac{B_z^2+B_\phi^2}{8\pi}\right)+\frac{B_\phi^2}{4\pi R}=0.
$$

Integrating the axial component of the magnetostatic [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) gives $I(R)=cRB_\phi/2$, since regularity removes the integration constant. Substituting $B_\phi=2I/(cR)$ combines the toroidal terms into

$$
\boxed{\frac d{dR}\left(p+\frac{B_z^2}{8\pi}\right)
+\frac1{2\pi c^2R^2}\frac{dI^2}{dR}=0.}
$$

This is the [cylindrical magnetostatic pressure balance](../../../../../../cylindrical-magnetostatic-pressure-balance.md) equation in terms of enclosed [electric current](../../../../../../electric-current.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
