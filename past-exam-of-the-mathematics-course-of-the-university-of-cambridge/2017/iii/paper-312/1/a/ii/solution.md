<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the normalization of the timelike [unit normal](../../../../../../../unit-normal.md) with the metric-compatible [covariant derivative](../../../../../../../covariant-derivative.md):

$$
0=\nabla_\nu(n^\mu n_\mu)=2n^\mu\nabla_\nu n_\mu.
$$

Thus the [derivative](../../../../../../../derivative.md) of the normal is already orthogonal to the normal in its second index. Expanding the second [spatial projection tensor](../../../../../../../spatial-projection-tensor.md) in the definition of the [extrinsic curvature of a spatial hypersurface](../../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md) gives

$$
K_{\mu\nu}=-P^\alpha{}_\mu(\delta^\beta{}_\nu+n^\beta n_\nu)\nabla_\alpha n_\beta=-P^\alpha{}_\mu\nabla_\alpha n_\nu.
$$

To prove symmetry using [Frobenius theorem](../../../../../../../frobenius-theorem.md), set $F_{\alpha\beta}=\nabla_\alpha n_\beta-\nabla_\beta n_\alpha$. [Hypersurface orthogonality](../../../../../../../hypersurface-orthogonality.md) is equivalent to

$$
n_\alpha F_{\beta\lambda}+n_\beta F_{\lambda\alpha}+n_\lambda F_{\alpha\beta}=0.
$$

Contract this with $n^\alpha P^\beta{}_\mu P^\lambda{}_\nu$. The last two terms vanish because a projected normal vanishes, while $n^\alpha n_\alpha=-1$ in the first term. Hence

$$
P^\alpha{}_\mu P^\beta{}_\nu F_{\alpha\beta}=0.
$$

The antisymmetric part of the doubly projected [covariant derivative](../../../../../../../covariant-derivative.md) of $n$ is therefore zero. This proves that [hypersurface orthogonality implies symmetric extrinsic curvature](../../../../../../../hypersurface-orthogonality-implies-symmetric-extrinsic-curvature.md):

$$
\boxed{n^\mu\nabla_\nu n_\mu=0,\quad K_{\mu\nu}=-P^\alpha{}_\mu\nabla_\alpha n_\nu,\quad K_{\mu\nu}=K_{\nu\mu}.}
$$

No geodesic assumption for the normal congruence is needed; its [normal acceleration](../../../../../../../normal-acceleration.md) may be nonzero.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
