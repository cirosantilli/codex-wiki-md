<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), use the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and the [Einstein summation convention](../../../../../einstein-notation.md) to expand

$$
\begin{aligned}
[\mathbf u\times(\nabla\times\mathbf u)]_i
&=\epsilon_{ijk}\epsilon_{klm}u_j\partial_lu_m\\
&=u_j\partial_i u_j-u_j\partial_j u_i\\
&=\frac12\partial_i(u_ju_j)-[(\mathbf u\cdot\nabla)\mathbf u]_i.
\end{aligned}
$$

The contraction of the two symbols uses the [Kronecker delta](../../../../../kronecker-delta.md), and the final step is the [product rule](../../../../../product-rule.md). Thus the [convective acceleration](../../../../../convective-acceleration.md) identity is

$$
\boxed{(\mathbf u\cdot\nabla)\mathbf u=\frac12\nabla|\mathbf u|^2-\mathbf u\times(\nabla\times\mathbf u).}
$$

Put $\boldsymbol\omega=\nabla\times\mathbf u$. The [curl of a gradient](../../../../../curl-of-a-gradient.md) vanishes, and the [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity gives

$$
\nabla\times(\mathbf u\times\boldsymbol\omega)=\mathbf u\,\nabla\cdot\boldsymbol\omega-\boldsymbol\omega\,\nabla\cdot\mathbf u+(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega.
$$

Since the [divergence of a curl is zero](../../../../../divergence-of-a-curl-is-zero.md), taking the [curl](../../../../../curl.md) of the first identity yields

$$
\boxed{\nabla\times[(\mathbf u\cdot\nabla)\mathbf u]=(\nabla\cdot\mathbf u)\boldsymbol\omega+(\mathbf u\cdot\nabla)\boldsymbol\omega-(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

Twice continuous differentiability suffices for the mixed-derivative identities used here.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
