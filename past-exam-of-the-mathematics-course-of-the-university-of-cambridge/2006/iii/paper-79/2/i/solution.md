<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $A_{ij}=\partial_j u_i$ and use [incompressibility](../../../../../../incompressible-flow.md), $A_{ii}=0$. The displayed vector can be expressed as

$$
D_i=A_{ij}A_{jk}u_k-\frac12u_i\operatorname{tr}(A^2).
$$

On taking its [divergence](../../../../../../divergence.md), $\partial_iA_{ij}=0$. Commuting the remaining [partial derivatives](../../../../../../partial-derivative.md) gives

$$
A_{ij}(\partial_iA_{jk})u_k
=u_kA_{ij}\partial_kA_{ji}
=\frac12u_k\partial_k\operatorname{tr}(A^2),
$$

which cancels the derivative of the second term of $D_i$. The derivatives falling on $u_k$ leave

$$
\boxed{\partial_iD_i=A_{ij}A_{jk}A_{ki}=\operatorname{tr}(A^3)}.
$$

In [homogeneous turbulence](../../../../../../homogeneous-turbulence.md), averaging commutes with differentiation and $\langle D_i\rangle$ is position independent, provided these [moments](../../../../../../moment.md) exist. Consequently $\langle\operatorname{tr}(A^3)\rangle=0$.

Using the [strain-rate tensor](../../../../../../strain-rate-tensor.md) and [vorticity](../../../../../../vorticity.md) decomposition supplied in the question now gives the [Betchov relation](../../../../../../betchov-relation.md):

$$
\boxed{\langle S_{ij}S_{jk}S_{ki}\rangle=-\frac34\langle\omega_i\omega_jS_{ij}\rangle}.
$$

This uses homogeneity and [incompressibility](../../../../../../incompressible-flow.md); isotropy is unnecessary.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
