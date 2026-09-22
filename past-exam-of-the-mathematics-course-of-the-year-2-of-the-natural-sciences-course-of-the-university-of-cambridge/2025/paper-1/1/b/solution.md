<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [divergence theorem](../../../../../divergence-theorem.md) states that, for a continuously differentiable [vector field](../../../../../vector-field.md) $\mathbf H$ on a bounded region $V$ with piecewise smooth boundary $S$ and outward [unit normal](../../../../../unit-normal.md) $\hat{\mathbf n}$,

$$
\int_V\nabla\cdot\mathbf H\,dV=\int_S\mathbf H\cdot\hat{\mathbf n}\,dS.
$$

To apply it, first derive the [divergence of a cross product](../../../../../divergence-of-a-cross-product.md) using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and the [product rule](../../../../../product-rule.md):

$$
\begin{aligned}
\nabla\cdot(\mathbf F\times\mathbf G)
&=\epsilon_{ijk}\partial_i(F_jG_k)\\
&=\epsilon_{ijk}(\partial_iF_j)G_k+\epsilon_{ijk}F_j\partial_iG_k\\
&=\mathbf G\cdot(\nabla\times\mathbf F)-\mathbf F\cdot(\nabla\times\mathbf G).
\end{aligned}
$$

In the second term the minus sign comes from interchanging the first two indices of the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). The [divergence theorem](../../../../../divergence-theorem.md) with $\mathbf H=\mathbf F\times\mathbf G$ now yields

$$
\boxed{\int_V[\mathbf G\cdot(\nabla\times\mathbf F)-\mathbf F\cdot(\nabla\times\mathbf G)]\,dV=\int_S(\mathbf F\times\mathbf G)\cdot\hat{\mathbf n}\,dS.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
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
