<h1 id="36e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $Q=F\cdot x$. Differentiate the given [Stokeslet](../../../../../../stokeslet.md) velocity:

$$
\partial_ju_i=\frac1{8\pi\mu}\left[-\frac{F_ix_j}{r^3}+\frac{F_jx_i+Q\delta_{ij}}{r^3}-\frac{3Qx_ix_j}{r^5}\right].
$$

Symmetrizing and subtracting the pressure term cancels the diagonal terms, leaving the [Cauchy stress tensor](../../../../../../cauchy-stress-tensor.md)

$$
\sigma_{ij}=-\frac{3Qx_ix_j}{4\pi r^5}.
$$

On the radius-$R$ surface with outward sphere normal $n=x/R$, the force exerted by the exterior fluid on the sphere is the [traction](../../../../../../traction.md)

$$
t_i=\sigma_{ij}n_j=-\frac3{4\pi R^2}(F\cdot n)n_i.
$$

Use $dS=R^2d\Omega$ and $\int_{S^2}n_in_jd\Omega=(4\pi/3)\delta_{ij}$ to find

$$
\boxed{G_i=-\frac3{4\pi}F_j\int n_in_jd\Omega=-F_i}.
$$

The $R^2$ factors cancel, proving independence of radius. This calculation uses the printed far-field [Stokeslet](../../../../../../stokeslet.md); higher multipoles of the exact sphere flow have zero net force through enclosing surfaces.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [36E](../../36e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
