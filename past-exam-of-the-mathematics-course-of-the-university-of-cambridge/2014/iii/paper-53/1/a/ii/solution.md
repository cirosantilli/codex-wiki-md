<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the $+---$ signature and $n^2=1$, direct expansion of the two [spatial projection tensors](../../../../../../../spatial-projection-tensor.md) gives

$$
q_{\alpha\beta}=P^\mu{}_\alpha P^\nu{}_\beta g_{\mu\nu}
=g_{\alpha\beta}-n_\alpha n_\beta.
$$

This restriction is negative definite on spatial vectors. The positive spatial [induced metric](../../../../../../../induced-metric.md) is instead $h_{\alpha\beta}=n_\alpha n_\beta-g_{\alpha\beta}=-q_{\alpha\beta}$, whose pullback to a time slice is the $h_{ij}$ used in the line element. The [spatial metric sign for a unit timelike normal](../../../../../../../spatial-metric-sign-for-a-unit-timelike-normal.md) is important here: the plus sign in the PDF's claimed equality is incompatible with its normal normalization: $g_{\alpha\beta}+n_\alpha n_\beta$ is not even transverse to $n^\alpha$.

The [spatial covariant derivative](../../../../../../../spatial-covariant-derivative.md) of a spatial tensor projects every index, including its derivative index. Projection only on the derivative index is sufficient for a scalar but not for a general tensor. Using [metric compatibility](../../../../../../../metric-compatibility.md) of the spacetime [Levi-Civita connection](../../../../../../../levi-civita-connection.md), we obtain

$$
D_\alpha h_{\beta\gamma}=P^\rho{}_\alpha P^\sigma{}_\beta P^\lambda{}_\gamma\nabla_\rho h_{\sigma\lambda}
=P^\rho{}_\alpha P^\sigma{}_\beta P^\lambda{}_\gamma
\left[(\nabla_\rho n_\sigma)n_\lambda+n_\sigma\nabla_\rho n_\lambda\right]=0.
$$

Each term contains a normal contracted with its [spatial projection tensor](../../../../../../../spatial-projection-tensor.md). Consequently $\boxed{D_i h_{jk}=0}$, and the negative spatial restriction also satisfies $D_iq_{jk}=0$. This proves the requested [metric compatibility of the spatial covariant derivative](../../../../../../../metric-compatibility-of-the-spatial-covariant-derivative.md) after correcting the source's metric sign. Contracting indices gives the particular expression written in the question.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
