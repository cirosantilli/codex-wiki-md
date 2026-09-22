<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $q_{\alpha\beta}=g_{\alpha\beta}+n_\alpha n_\beta$ for the [induced metric](../../../../../../induced-metric.md). The [spatial covariant derivative](../../../../../../spatial-covariant-derivative.md) projects its derivative index and both tensor indices:

$$
D_\gamma q_{\alpha\beta}=P^\rho{}_\gamma P^\mu{}_\alpha P^\nu{}_\beta\nabla_\rho(g_{\mu\nu}+n_\mu n_\nu).
$$

Four-dimensional [metric compatibility](../../../../../../metric-compatibility.md) removes the derivative of $g$. Each remaining term contains an undifferentiated normal on a projected index and hence vanishes. Therefore

$$
\boxed{D_\gamma q_{\alpha\beta}=0.}
$$

This establishes [metric compatibility of the spatial covariant derivative](../../../../../../metric-compatibility-of-the-spatial-covariant-derivative.md) directly from its projected definition.

Differentiating the normal's normalization gives

$$
0=\nabla_\nu(n^\mu n_\mu)=2n^\mu\nabla_\nu n_\mu,
$$

so **$n^\mu\nabla_\nu n_\mu=0$**. Consequently the second projection in the [extrinsic curvature](../../../../../../extrinsic-curvature.md) definition is redundant:

$$
K_{\alpha\beta}=P^\mu{}_\alpha(\delta^\nu{}_\beta+n^\nu n_\beta)\nabla_\mu n_\nu
=P^\mu{}_\alpha\nabla_\mu n_\beta.
$$

Finally differentiate $P^\lambda{}_\nu=\delta^\lambda{}_\nu+n^\lambda n_\nu$ and project:

$$
P^\mu{}_\alpha P^\nu{}_\beta\nabla_\mu P^\lambda{}_\nu
=P^\mu{}_\alpha P^\nu{}_\beta[(\nabla_\mu n^\lambda)n_\nu+n^\lambda\nabla_\mu n_\nu]
=\boxed{K_{\alpha\beta}n^\lambda.}
$$

The first term vanishes by $P^\nu{}_\beta n_\nu=0$, and the second is precisely the defining curvature. The positive sign follows from the specified positive-expansion convention, rather than from an independent projector convention.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
