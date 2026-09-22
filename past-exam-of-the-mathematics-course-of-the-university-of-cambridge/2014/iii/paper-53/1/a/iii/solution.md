<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Differentiate the [spatial projection tensor](../../../../../../../spatial-projection-tensor.md) before making any contractions:

$$
\nabla_\nu P^\lambda{}_\mu=-(\nabla_\nu n^\lambda)n_\mu-n^\lambda\nabla_\nu n_\mu.
$$

For the [spatial projector derivative identity](../../../../../../../spatial-projector-derivative-identity.md), its first term vanishes after projection on $\mu$. The definition of the [extrinsic curvature of a spatial hypersurface](../../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md) then gives the stronger tensor identity

$$
\boxed{P^\mu{}_\rho P^\nu{}_\sigma\nabla_\nu P^\lambda{}_\mu=-n^\lambda K_{\sigma\rho}.}
$$

Here $\lambda$ remains a free index. For a normal to a genuine [foliation](../../../../../../../foliation.md), the [extrinsic curvature](../../../../../../../extrinsic-curvature.md) is symmetric: projecting $\nabla_{[\nu}n_{\mu]}$ gives zero because locally $n_\mu$ is a scalar multiple of a time gradient. This is [hypersurface orthogonality implies symmetric extrinsic curvature](../../../../../../../hypersurface-orthogonality-implies-symmetric-extrinsic-curvature.md).

Contract $\rho$ with $\lambda$ in the stronger identity to obtain exactly the contraction displayed in the PDF:

$$
P^\mu{}_\lambda P^\nu{}_\sigma\nabla_\nu P^\lambda{}_\mu
=-n^\lambda K_{\sigma\lambda}=-n^\lambda K_{\lambda\sigma}=\boxed{0}.
$$

The last equality follows from the transversality of the [extrinsic curvature](../../../../../../../extrinsic-curvature.md). Thus the literal printed identity is valid, although both its sides vanish; the uncontracted identity explains its geometric origin.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
