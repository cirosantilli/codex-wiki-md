<h1 id="3c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) and sum over repeated indices. The [contraction of two Levi-Civita symbols](../../../../../../contraction-of-two-levi-civita-symbols.md) and the [product rule](../../../../../../product-rule.md) give

$$
\begin{aligned}
[\nabla\times(F\times G)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{k\ell m}F_\ell G_m)\\
&=\partial_j(F_iG_j-F_jG_i)\\
&=F_i\partial_jG_j-G_i\partial_jF_j+G_j\partial_jF_i-F_j\partial_jG_i.
\end{aligned}
$$

Reading the four terms as [divergence](../../../../../../divergence.md) and directional derivatives proves the [curl of a cross product](../../../../../../curl-of-a-cross-product.md) identity

$$
\boxed{\nabla\times(F\times G)=F(\nabla\cdot G)-G(\nabla\cdot F)+(G\cdot\nabla)F-(F\cdot\nabla)G.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3C](../../3c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
