# Radial curl of angular gradient fields

↑ **Parent:** [Surface gradient](surface-gradient.md)

Let $\nabla_{\!\tan}F=\nabla F-\mathbf e_r\partial_rF$ be the tangential [surface gradient](surface-gradient.md) on a [sphere](sphere.md) of [radius](radius.md) $r>0$. For smooth scalar fields, set $\mathbf f=R\mathbf e_r+\nabla_{\!\tan}G+\mathbf e_r\times\nabla_{\!\tan}F$. Its radial [curl](curl.md) detects only $F$:

$$
(\nabla\times\mathbf f)\cdot\mathbf e_r=\frac1{r^2}\Delta_{S^2}F,\qquad\Delta_{S^2}=\frac1{\sin\theta}\partial_\theta(\sin\theta\,\partial_\theta)+\frac1{\sin^2\theta}\partial_\phi^2.
$$

To prove this, use the radial [curl](curl.md) formula $(r\sin\theta)^{-1}[\partial_\theta(\sin\theta f_\phi)-\partial_\phi f_\theta]$. The radial component $R$ never enters it. The $G$ terms cancel as $G_{\phi\theta}-G_{\theta\phi}=0$ by [symmetry of second derivatives](symmetry-of-second-derivatives.md), while the $F$ terms give the unit-sphere [Laplace-Beltrami operator](laplace-beltrami-operator.md). Taking the [dot product](dot-product.md) with the position [vector](vector.md) $\mathbf r=r\mathbf e_r$ gives the displayed $r^{-1}$ version. This tangential gradient decomposition does not assert that the whole [vector field](vector-field.md) is [solenoidal](solenoidal-vector-field.md).

## ↑ Ancestors (9)

1. [Surface gradient](surface-gradient.md)
2. [Surface covariant derivative](surface-covariant-derivative.md)
3. [Geodesic](geodesic.md)
4. [Riemannian geometry](riemannian-geometry-split.md)
5. [Differential geometry](differential-geometry-split.md)
6. [Geometry and topology](geometry-and-topology-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/1/ii/solution.md)
