<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a differentiable [vector field](../../../../../vector-field.md) in [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), the [divergence](../../../../../divergence.md) and [curl](../../../../../curl.md) are

$$
\nabla\cdot F=\partial_iF_i,\qquad(\nabla\times F)_i=\epsilon_{ijk}\partial_jF_k,
$$

with summation over repeated indices. In components the curl is $(\partial_yF_z-\partial_zF_y,\partial_zF_x-\partial_xF_z,\partial_xF_y-\partial_yF_x)$. The [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md) and the [product rule](../../../../../product-rule.md) give

$$
\begin{aligned}
[\nabla\times(F\times G)]_i
&=\epsilon_{ijk}\epsilon_{k\ell m}\partial_j(F_\ell G_m)\\
&=(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})\partial_j(F_\ell G_m)\\
&=G_j\partial_jF_i+F_i\partial_jG_j-G_i\partial_jF_j-F_j\partial_jG_i.
\end{aligned}
$$

Recognizing the [directional derivatives](../../../../../directional-derivative.md) gives the [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity

$$
\nabla\times(F\times G)=(G\cdot\nabla)F-G(\nabla\cdot F)-(F\cdot\nabla)G+F(\nabla\cdot G).
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
