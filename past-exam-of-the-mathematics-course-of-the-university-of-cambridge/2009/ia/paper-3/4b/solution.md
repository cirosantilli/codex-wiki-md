<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

For Cartesian components, $\partial_jx_i=\delta_{ij}$, the [Kronecker delta](../../../../../kronecker-delta.md). Differentiating $r^2=x_ix_i$ gives

$$
\boxed{\partial_jr=\frac{x_j}{r}\quad(r>0).}
$$

Put $s=k_\ell x_\ell$. Using the product rule and $\partial_j r^{-q}=-q x_jr^{-q-2}$ gives the [velocity gradient](../../../../../velocity-gradient.md)

$$
\boxed{d_{ij}=-\frac{k_ix_j}{r^3}+\frac{k_jx_i}{r^3}
+\frac{s\delta_{ij}}{r^3}-\frac{3s x_ix_j}{r^5}.}
$$

This is the [rate of strain and vorticity of a Stokeslet](../../../../../rate-of-strain-and-vorticity-of-a-stokeslet.md), apart from the overall physical normalization. Its [symmetric and antisymmetric parts of a matrix](../../../../../symmetric-and-antisymmetric-parts-of-a-matrix.md) are

$$
E_{ij}=\frac{d_{ij}+d_{ji}}2=\frac{s\delta_{ij}}{r^3}-\frac{3s x_ix_j}{r^5},\qquad
W_{ij}=\frac{d_{ij}-d_{ji}}2=\frac{k_jx_i-k_ix_j}{r^3}.
$$

Here $E_{ji}=E_{ij}$ and $W_{ji}=-W_{ij}$, and $d=E+W$. Taking the [trace](../../../../../matrix-trace.md) gives the [divergence](../../../../../divergence.md)

$$
\boxed{\nabla\cdot\mathbf u=d_{ii}=\frac{3s}{r^3}-\frac{3sr^2}{r^5}=0.}
$$

For the [curl](../../../../../curl.md), use the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). Because $d_{kj}=\partial_ju_k$, the symmetric part makes no contribution, and

$$
(\nabla\times\mathbf u)_i=\epsilon_{ijk}d_{kj}
=\frac{\epsilon_{ijk}(k_jx_k-k_kx_j)}{r^3}
=\boxed{\frac{2\epsilon_{ijk}k_jx_k}{r^3}}.
$$

Thus $\nabla\times\mathbf u=2\mathbf k\times\mathbf x/r^3$. All derivative identities hold away from the singular origin.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
