<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [product rule](../../../../../product-rule.md) in [Einstein notation](../../../../../einstein-notation.md), using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) to express the [cross product](../../../../../cross-product.md):

$$
\begin{aligned}
\nabla\cdot(\mathbf a\times\mathbf b)
&=\partial_i(\epsilon_{ijk}a_jb_k)\\
&=\epsilon_{ijk}(\partial_i a_j)b_k+\epsilon_{ijk}a_j\partial_i b_k\\
&=b_k\epsilon_{kij}\partial_i a_j-a_j\epsilon_{jik}\partial_i b_k\\
&=\mathbf b\cdot(\nabla\times\mathbf a)-\mathbf a\cdot(\nabla\times\mathbf b).
\end{aligned}
$$

The third line uses a cyclic permutation of indices in the first term and an interchange of two indices in the second. Rearranging proves the [divergence of a cross product](../../../../../divergence-of-a-cross-product.md) identity:

$$
\boxed{\mathbf a\cdot(\nabla\times\mathbf b)
=\mathbf b\cdot(\nabla\times\mathbf a)-\nabla\cdot(\mathbf a\times\mathbf b)}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
