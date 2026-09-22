<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [radial action](../../../../../../radial-action.md) is

$$
J_r=\frac1\pi\int_{r_-}^{r_+}
\sqrt{2[E-\Phi(r)]-\frac{L^2}{r^2}}\,dr.
$$

With the variable $x$ from part b this becomes

$$
J_r=\frac{b\sqrt{-2E}}{2\pi}
\int_{x_-}^{x_+}
\left(\frac1x+\frac1{x-2}\right)
\sqrt{(x-x_-)(x_+-x)}\,dx.
$$

Applying the supplied integral twice, with $c=0$ and $c=2$, and using the root sum and products from parts b and c gives

$$
\boxed{
J_r=\frac{GM}{\sqrt{-2E}}
-\frac12\left(L+\sqrt{L^2+4GMb}\right)}.
$$

This is the [radial action of the spherical isochrone model](../../../../../../radial-action-of-the-spherical-isochrone-model.md). Rearranging,

$$
\frac{2GM}{\sqrt{-2E}}
=2J_r+L+\sqrt{L^2+4GMb},
$$

and squaring yields the [Hamiltonian](../../../../../../hamiltonian.md) in [action-angle variables](../../../../../../action-angle-variables.md):

$$
\boxed{
H(J_r,L)
=-\frac{2(GM)^2}
{\left(2J_r+L+\sqrt{L^2+4GMb}\right)^2}}.
$$

As a check, differentiating this Hamiltonian gives $\Omega_r=(-2E)^{3/2}/(GM)$ and the frequency ratio found in part c.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
