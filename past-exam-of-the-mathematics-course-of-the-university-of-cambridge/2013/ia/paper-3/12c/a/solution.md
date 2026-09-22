<h1 id="12c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) and summation over repeated indices. Contracting the two symbols gives

$$
\begin{aligned}
[\nabla\times(\mathbf F\times\mathbf G)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{klm}F_lG_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(F_lG_m)\\
&=\partial_j(F_iG_j-F_jG_i)\\
&=F_i\partial_jG_j-G_i\partial_jF_j+G_j\partial_jF_i-F_j\partial_jG_i.
\end{aligned}
$$

Thus the [curl of a cross product](../../../../../../curl-of-a-cross-product.md) is

$$
\boxed{\nabla\times(\mathbf F\times\mathbf G)
=\mathbf F\nabla\cdot\mathbf G-\mathbf G\nabla\cdot\mathbf F
+(\mathbf G\cdot\nabla)\mathbf F-(\mathbf F\cdot\nabla)\mathbf G.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
