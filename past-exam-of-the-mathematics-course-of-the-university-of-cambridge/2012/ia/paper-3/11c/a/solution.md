<h1 id="11c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Einstein summation convention](../../../../../../einstein-notation.md) and the [contraction of two Levi-Civita symbols](../../../../../../contraction-of-two-levi-civita-symbols.md). For the first [cross product](../../../../../../cross-product.md) term,

$$
\begin{aligned}
[F\times(\nabla\times G)]_i
&=\epsilon_{ijk}F_j\epsilon_{k\ell m}\partial_\ell G_m\\
&=(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})F_j\partial_\ell G_m\\
&=F_j\partial_iG_j-F_j\partial_jG_i.
\end{aligned}
$$

The last term cancels $(F\cdot\nabla)G_i$. Interchanging $F,G$ gives the analogous cancellation with $(G\cdot\nabla)F_i$. The surviving terms are $F_j\partial_iG_j+G_j\partial_iF_j=\partial_i(F_jG_j)$ by the [product rule](../../../../../../product-rule.md). This proves the [dot-product gradient identity](../../../../../../dot-product-gradient-identity.md)

$$
\boxed{\nabla(F\cdot G)=(F\cdot\nabla)G+(G\cdot\nabla)F+F\times(\nabla\times G)+G\times(\nabla\times F).}
$$

The proof only requires continuously differentiable [vector fields](../../../../../../vector-field.md); neither field needs to be an [irrotational vector field](../../../../../../irrotational-vector-field.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
