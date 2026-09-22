<h1 id="6/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Write the [curl](../../../../../curl.md) and [cross product](../../../../../cross-product.md) with the [Levi-Civita symbol](../../../../../levi-civita-symbol.md), then use its contraction identity:

$$
\begin{aligned}
[\nabla\times(A\times B)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{k\ell m}A_\ell B_m)\\
&=(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})\partial_j(A_\ell B_m)\\
&=\partial_j(A_iB_j-A_jB_i).
\end{aligned}
$$

Expanding with the [product rule](../../../../../product-rule.md) gives

$$
A_i\partial_jB_j+B_j\partial_jA_i-B_i\partial_jA_j-A_j\partial_jB_i.
$$

Recognize the [divergence](../../../../../divergence.md) in the first and third terms, and the [directional derivatives](../../../../../directional-derivative.md) in the other two. The [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity is therefore

$$
\boxed{\nabla\times(A\times B)=A(\nabla\cdot B)+(B\cdot\nabla)A-B(\nabla\cdot A)-(A\cdot\nabla)B.}
$$

The derivatives act on both vector fields. No assumption of vanishing divergence or spatially constant fields has been made.

## ↑ Ancestors (13)

1. [Vii](../vii.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
