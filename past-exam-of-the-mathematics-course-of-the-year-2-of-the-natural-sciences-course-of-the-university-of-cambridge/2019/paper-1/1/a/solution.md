<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md) in [Cartesian coordinates](../../../../../cartesian-coordinate-system.md). With repeated indices summed,

$$
\begin{aligned}
[\nabla\times(\mathbf A\times\mathbf B)]_i
&=\epsilon_{ijk}\epsilon_{klm}\partial_j(A_lB_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(A_lB_m)\\
&=\partial_j(A_iB_j)-\partial_j(A_jB_i)\\
&=B_j\partial_jA_i+A_i\partial_jB_j-B_i\partial_jA_j-A_j\partial_jB_i.
\end{aligned}
$$

The last line is the [product rule](../../../../../product-rule.md). Reading its four terms in vector notation proves the [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity:

$$
\boxed{\nabla\times(\mathbf A\times\mathbf B)=(\mathbf B\cdot\nabla)\mathbf A-\mathbf B(\nabla\cdot\mathbf A)-(\mathbf A\cdot\nabla)\mathbf B+\mathbf A(\nabla\cdot\mathbf B).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
