<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An open-boundary [matrix product state](../../../../../../matrix-product-state.md) with physical dimension $q$ and bond dimension $\chi$ is

$$
|\Psi_N\rangle
=\sum_{i_1,\ldots,i_N=1}^q
\langle \ell|A^{i_1}A^{i_2}\cdots A^{i_N}|r\rangle
|i_1i_2\cdots i_N\rangle,
$$

where the $A^i$ are $\chi\times\chi$ matrices and $|\ell\rangle,|r\rangle$ are boundary vectors. For periodic boundary conditions, replace the boundary contraction by the [matrix trace](../../../../../../matrix-trace.md) $\operatorname{Tr}(A^{i_1}\cdots A^{i_N})$.

The same matrices define the [matrix product state transfer map](../../../../../../matrix-product-state-transfer-map.md)

$$
\mathcal E(X)=\sum_iA^iX(A^i)^\dagger.
$$

When $\sum_i(A^i)^\dagger A^i=I$, the [Stinespring dilation](../../../../../../stinespring-dilation.md)

$$
V|\psi\rangle=\sum_i|i\rangle\otimes A^i|\psi\rangle
$$

is an [isometry](../../../../../../isometry.md). Repeatedly applying $V$ stores each Kraus label in a fresh physical register:

$$
V_N\cdots V_1|r\rangle
=\sum_{i_1,\ldots,i_N}|i_1\cdots i_N\rangle
\otimes A^{i_N}\cdots A^{i_1}|r\rangle.
$$

Contracting the remaining virtual system with $\langle\ell|$ gives an MPS, while tracing over all recorded labels gives repeated application of the [completely positive map](../../../../../../completely-positive-map.md) $\mathcal E$. The MPS is therefore a coherent [unravelling](../../../../../../matrix-product-state-as-an-unravelling-of-a-completely-positive-map.md) of the channel. Equivalently, retaining the Kraus-label registers realizes a [purification](../../../../../../purification-of-a-density-operator.md) of its output. A non-normalized MPS tensor gives the same construction with a general completely positive map; an appropriate canonical gauge normalizes the transfer map on its support.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
