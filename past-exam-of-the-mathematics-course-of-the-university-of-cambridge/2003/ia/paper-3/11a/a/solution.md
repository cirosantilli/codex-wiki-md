<h1 id="11a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [suffix notation](../../../../../../einstein-notation.md), summing repeated indices. The [contraction of two Levi-Civita symbols](../../../../../../contraction-of-two-levi-civita-symbols.md) gives

$$
[F\times(\nabla\times G)]_i=\epsilon_{ijk}F_j\epsilon_{k\ell m}\partial_\ell G_m=F_j\partial_iG_j-F_j\partial_jG_i.
$$

Adding the [directional derivative](../../../../../../directional-derivative.md) $(F\cdot\nabla)G_i=F_j\partial_jG_i$ cancels the second term. Interchanging $F,G$ gives another pair whose sum is $G_j\partial_iF_j$. The total right-hand side is therefore

$$
F_j\partial_iG_j+G_j\partial_iF_j=\partial_i(F_jG_j),
$$

the $i$th component of the [gradient](../../../../../../gradient.md) of the [dot product](../../../../../../dot-product.md). Since this holds for each component, the [dot-product gradient identity](../../../../../../dot-product-gradient-identity.md) is proved:

$$
\boxed{\nabla(F\cdot G)=(F\cdot\nabla)G+(G\cdot\nabla)F+F\times(\nabla\times G)+G\times(\nabla\times F)}.
$$

It holds for any continuously differentiable [vector fields](../../../../../../vector-field.md); no irrotationality assumption is used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
