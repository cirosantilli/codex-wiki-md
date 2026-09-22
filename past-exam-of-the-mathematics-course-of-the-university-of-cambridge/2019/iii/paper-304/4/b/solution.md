<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The variation found above uses the [adjoint covariant derivative](../../../../../../adjoint-covariant-derivative.md):

$$
\delta A_\mu^a=\frac1g(D_\mu\alpha)^a,
\qquad
(D_\mu c)^a=\partial_\mu c^a+g f^{abc}A_\mu^b c^c.
$$

For the [Lorenz gauge](../../../../../../lorenz-gauge-condition.md) functional $G^a[A]=\partial^\mu A_\mu^a$,

$$
\frac{\delta G^a[A^\alpha](x)}{\delta\alpha^b(y)}
=\frac1g\partial^\mu D_\mu^{ab}\delta(x-y).
$$

The field-independent factor $1/g$ may be absorbed into normalization. The [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) exponentiates the [Faddeev-Popov determinant](../../../../../../faddeev-popov-determinant.md) with anticommuting [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md):

$$
\det(\partial^\mu D_\mu)
=\int\mathcal D\bar c\,\mathcal Dc\,
e^{-\int d^4x\,\bar c^a\partial^\mu(D_\mu c)^a}.
$$

A Gaussian average over the gauge condition supplies the covariant gauge-fixing term, so

$$
\boxed{S=S_g+\int d^4x\left[
\frac1{2\xi}(\partial^\mu A_\mu^a)^2
+\bar c^a\partial^\mu(D_\mu c)^a
\right],
\qquad
D_\mu^{ac}=\delta^{ac}\partial_\mu+g f^{abc}A_\mu^b.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
