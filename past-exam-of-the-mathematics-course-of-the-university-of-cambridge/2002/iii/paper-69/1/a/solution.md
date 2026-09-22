<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $D=d-1$ for the membrane's internal dimension and assume $\sigma>0$. The small-slope expansion is

$$
\sqrt{1+|\nabla h|^2}=1+\tfrac12|\nabla h|^2+O(|\nabla h|^4).
$$

The zeroth-order term is the projected area and is independent of the height field. Discarding it changes only an overall normalization of the [partition function](../../../../../../canonical-partition-function.md). Thus the leading fluctuation energy and its statistical weight are

$$
H_2[h]=\frac\sigma2\int d^Dx\,|\nabla h|^2,\qquad
\boxed{\mathcal Z_2=\int\mathcal Dh\,\exp\left[-\frac{\beta\sigma}{2}\int d^Dx\,|\nabla h|^2\right].}
$$

One obtains this [Gaussian field theory](../../../../../../gaussian-field-theory.md) by discretizing the height field on a microscopic mesh, integrating every height with its Boltzmann weight, and then writing the continuum measure. A microscopic cutoff is retained for quantities dominated by short wavelengths. Quadratic order here really means small slopes: a large rigid height shift is still free because the energy has no dependence on $h$ itself.

The uniform height mode has zero energy. Fix its mean, impose a [boundary condition](../../../../../../boundary-condition.md), or divide out the integral over global translations to normalize the [partition function](../../../../../../canonical-partition-function.md). Height differences are independent of that choice. The approximation is the tension-only part of [small-slope elastic membrane energy](../../../../../../small-slope-elastic-membrane-energy.md); there is no bending rigidity or confining potential in this part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
