<h1 id="3a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Einstein summation convention](../../../../../../einstein-notation.md), with [divergence](../../../../../../divergence.md) $\partial_iF_i$ and [curl](../../../../../../curl.md) $(\nabla\times\mathbf F)_i=\epsilon_{ijk}\partial_jF_k$, where $\epsilon_{ijk}$ is the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md). For the first [vector field](../../../../../../vector-field.md),

$$
\partial_jF_i=2x_jx_i+r^2\delta_{ij},\qquad
\boxed{\nabla\cdot\mathbf F=5r^2,\quad \nabla\times\mathbf F=\mathbf0.}
$$

The derivative matrix is symmetric, so its contraction with the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) vanishes. For the second [vector field](../../../../../../vector-field.md),

$$
\partial_jG_i=a_jx_i+(\mathbf a\cdot\mathbf x)\delta_{ij},\qquad
\boxed{\nabla\cdot\mathbf G=4\mathbf a\cdot\mathbf x,\quad \nabla\times\mathbf G=\mathbf a\times\mathbf x.}
$$

For the third [vector field](../../../../../../vector-field.md), $H_i=\epsilon_{ikl}a_kx_l/r$. Its [divergence](../../../../../../divergence.md) is zero because the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) contracts with symmetric products. For its [curl](../../../../../../curl.md), either contract two [Levi-Civita symbols](../../../../../../levi-civita-symbol.md) or use the [vector triple product](../../../../../../vector-triple-product.md):

$$
\nabla\times\left(\frac{\mathbf a\times\mathbf x}{r}\right)
=-\frac{\mathbf x}{r^3}\times(\mathbf a\times\mathbf x)+\frac{2\mathbf a}{r}
=\frac{\mathbf a}{r}+\frac{(\mathbf a\cdot\mathbf x)\mathbf x}{r^3}.
$$

Thus

$$
\boxed{\nabla\cdot\mathbf H=0,\qquad
\nabla\times\mathbf H=\frac{\mathbf a+(\mathbf a\cdot\widehat{\mathbf x})\widehat{\mathbf x}}r.}
$$

All formulas hold on $r>0$, the domain where the radial [unit vector](../../../../../../unit-vector.md) is defined.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3A](../../3a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
