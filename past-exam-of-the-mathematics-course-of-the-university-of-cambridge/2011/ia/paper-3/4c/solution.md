<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

In [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), independent coordinate variables satisfy

$$
\frac{\partial x_i}{\partial x_j}=\delta_{ij},\qquad
\frac{\partial r}{\partial x_j}=\frac{x_j}{r}\quad(r>0),
$$

where $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md). Applying the [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) to $u_i=r^\alpha x_i$ gives the [Jacobian matrix](../../../../../jacobian-matrix.md)

$$
\boxed{d_{ij}=r^\alpha\delta_{ij}+\alpha r^{\alpha-2}x_ix_j.}
$$

This [tensor](../../../../../tensor.md) is symmetric in $i,j$. Hence its contraction with the antisymmetric [Levi-Civita symbol](../../../../../levi-civita-symbol.md) vanishes:

$$
(\nabla\times\mathbf u)_i=\epsilon_{ijk}d_{kj}=0.
$$

Similarly, $v_i=\epsilon_{ijk}k_ju_k$ and the constancy of $\mathbf k$ give

$$
\nabla\cdot\mathbf v=\epsilon_{ijk}k_jd_{ki}=0.
$$

The trace of the [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
\nabla\cdot\mathbf u=(3+\alpha)r^\alpha,
$$

which vanishes for $\alpha=-3$. The [curl of a cross product](../../../../../curl-of-a-cross-product.md) identity, with $\mathbf k$ constant, now gives

$$
\nabla\times(\mathbf k\times\mathbf u)
=\mathbf k(\nabla\cdot\mathbf u)-(\mathbf k\cdot\nabla)\mathbf u.
$$

For $\alpha=-3$,

$$
(\mathbf k\cdot\nabla)\mathbf u=r^{-3}\mathbf k-3r^{-5}(\mathbf k\cdot\mathbf x)\mathbf x,
$$

so

$$
\boxed{\nabla\times\mathbf v=\frac{3(\mathbf k\cdot\mathbf x)\mathbf x-r^2\mathbf k}{r^5}.}
$$

All identities for this singular case hold on $r>0$. In particular, zero [divergence](../../../../../divergence.md) here is a pointwise assertion away from the origin, not an assertion that the flux through a sphere enclosing the singularity is zero.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
