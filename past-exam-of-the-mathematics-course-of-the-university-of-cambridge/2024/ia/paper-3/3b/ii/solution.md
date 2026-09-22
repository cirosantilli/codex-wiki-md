<h1 id="3b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) and the product rule. First,

$$
\begin{aligned}
\nabla\cdot(F\times G)
+&=\partial_i(\epsilon_{ijk}F_jG_k)\\
+&=\epsilon_{ijk}(\partial_iF_j)G_k
++\epsilon_{ijk}F_j\partial_iG_k\\
+&=G\cdot(\nabla\times F)-F\cdot(\nabla\times G).
\end{aligned}
$$

For the second identity, the contraction

$$
\epsilon_{ijk}\epsilon_{klm}
+=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl}
$$

gives

$$
\begin{aligned}
+[\nabla\times(F\times G)]_i
+&=\epsilon_{ijk}\partial_j(\epsilon_{klm}F_lG_m)\\
+&=\partial_j(F_iG_j-F_jG_i)\\
+&=F_i\partial_jG_j-G_i\partial_jF_j
++G_j\partial_jF_i-F_j\partial_jG_i.
\end{aligned}
$$

In [vector](../../../../../../vector.md) notation this is

$$
\boxed{
+\nabla\times(F\times G)
+=F(\nabla\cdot G)-G(\nabla\cdot F)
++(G\cdot\nabla)F-(F\cdot\nabla)G}.
$$

These are the [divergence and curl of a cross product](../../../../../../divergence-and-curl-of-a-cross-product.md) identities.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3B](../../3b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
