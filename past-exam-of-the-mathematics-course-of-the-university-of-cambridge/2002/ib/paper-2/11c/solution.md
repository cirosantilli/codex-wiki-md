<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Under a Cartesian frame change $B'_i=R_{ik}B_k$, where $R$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md). Orthogonality gives $B'_kB'_k=B_kB_k$ and $R_{ik}R_{j\ell}\delta_{k\ell}=\delta_{ij}$. Therefore

$$
\alpha B'_iB'_j+\beta|\mathbf B'|^2\delta_{ij}=R_{ik}R_{j\ell}T_{k\ell},
$$

which is the [tensor component transformation law](../../../../../tensor-component-transformation-law.md). Also $T_{ij}=T_{ji}$ directly, proving that it is a symmetric [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) for every choice of the two scalars.

For $\mathbf B\ne0$, the direction of $\mathbf B$ is an [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) $(\alpha+\beta)|\mathbf B|^2$. Every vector perpendicular to $\mathbf B$ is an [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) $\beta|\mathbf B|^2$, a two-dimensional [eigenspace](../../../../../eigenspace.md). If $\alpha=0$, these eigenvalues coincide and every nonzero vector is an eigenvector. If $\mathbf B=0$, the [tensor](../../../../../tensor.md) is zero and again every nonzero vector is an eigenvector, now with eigenvalue zero.

For the position-dependent field with zero [divergence](../../../../../divergence.md), the [product rule](../../../../../product-rule.md) gives

$$
\partial_jT_{ij}=\alpha B_j\partial_jB_i+2\beta B_k\partial_iB_k.
$$

Contraction of the two [Levi-Civita symbols](../../../../../levi-civita-symbol.md) in the [curl](../../../../../curl.md) and [cross product](../../../../../cross-product.md) gives

$$
[(\nabla\times\mathbf B)\times\mathbf B]_i=B_j\partial_jB_i-B_k\partial_iB_k.
$$

Consequently

$$
\boxed{\alpha=1,\qquad\beta=-\frac12},\qquad T_{ij}=B_iB_j-\frac12|\mathbf B|^2\delta_{ij}.
$$

These constants give the magnetic part of the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md), with its physical prefactor suppressed. They are forced if the identity is to hold for every divergence-free field: $\mathbf B=(y,0,0)$ forces $2\beta=-1$; at the origin $\mathbf B=(y,1,0)$ then forces $\alpha=1$.

Apply the [divergence theorem](../../../../../divergence-theorem.md) separately to each component:

$$
\int_V[(\nabla\times\mathbf B)\times\mathbf B]_i\,dV=\int_S T_{ij}n_j\,dS.
$$

Since the whole vector field vanishes on $S$, all components of $T$ vanish there, and hence **the vector volume integral is zero**. The argument assumes a differentiable field and a boundary for which the [divergence theorem](../../../../../divergence-theorem.md) applies.

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
