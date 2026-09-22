<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Einstein summation convention](../../../../../einstein-notation.md), writing $\partial_j=\partial/\partial x_j$. The [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md) gives

$$
\begin{aligned}
[\nabla\times(\mathbf a\times\mathbf b)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{klm}a_lb_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(a_lb_m)\\
&=\partial_j(a_ib_j-a_jb_i)\\
&=a_i\partial_jb_j-b_i\partial_ja_j+b_j\partial_ja_i-a_j\partial_jb_i.
\end{aligned}
$$

The last equality is the [product rule](../../../../../product-rule.md). Recognizing the [divergences](../../../../../divergence.md) and [directional derivatives](../../../../../directional-derivative.md) proves the [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity:

$$
\boxed{\nabla\times(\mathbf a\times\mathbf b)=\mathbf a(\nabla\cdot\mathbf b)-\mathbf b(\nabla\cdot\mathbf a)+(\mathbf b\cdot\nabla)\mathbf a-(\mathbf a\cdot\nabla)\mathbf b.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
