<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the injective translationally invariant case, the [fundamental theorem of matrix product states](../../../../../../fundamental-theorem-of-matrix-product-states.md) states that two tensors $A=\{A^i\}$ and $B=\{B^i\}$ of the same minimal bond dimension generate the same periodic MPS for every sufficiently large length if and only if

$$
A^i=e^{i\theta}XB^iX^{-1}
$$

for every physical index $i$, with one invertible matrix $X$. Equality as normalized rays permits the phase $e^{i\theta}$; equality as vectors for all lengths restricts the resulting factor $e^{iN\theta}$ accordingly. The converse is immediate from cyclicity of the [matrix trace](../../../../../../matrix-trace.md):

$$
\operatorname{Tr}(A^{i_1}\cdots A^{i_N})
=e^{iN\theta}\operatorname{Tr}(B^{i_1}\cdots B^{i_N}).
$$

For the nontrivial direction, [block](../../../../../../blocking-a-matrix-product-state.md) enough sites that both tensors are injective and define

$$
\Gamma_A^L(X)
=\sum_{i_1,\ldots,i_L}
\operatorname{Tr}(XA^{i_1}\cdots A^{i_L})
|i_1\cdots i_L\rangle,
$$

with $\Gamma_B^L$ defined similarly. Injectivity means that $\Gamma_A^L$ and $\Gamma_B^L$ have trivial [kernels](../../../../../../kernel-of-a-linear-map.md). Equality of all sufficiently long periodic states implies equality of the local support spaces $\operatorname{im}\Gamma_A^L=\operatorname{im}\Gamma_B^L$, so there is an invertible linear map $F$ on the virtual matrix algebra satisfying

$$
\Gamma_A^L=\Gamma_B^L\circ F.
$$

Compare two adjacent blocks and contract arbitrary environments on their left and right. Because both block maps are injective, equality of the physical contractions forces

$$
F(XY)=F(X)F(Y),
\qquad
F(I)=I.
$$

Thus $F$ is a unital algebra automorphism of $M_\chi(\mathbb C)$. By [every automorphism of a full matrix algebra is inner](../../../../../../every-automorphism-of-a-full-matrix-algebra-is-inner.md), $F(X)=X_0XX_0^{-1}$ for an invertible $X_0$. Applying this relation to a block with one physical site exposed gives

$$
A^i=e^{i\theta}X_0B^iX_0^{-1}.
$$

This proves the theorem and identifies the freedom as the [gauge equivalence of injective matrix product state tensors](../../../../../../gauge-equivalence-of-injective-matrix-product-state-tensors.md). For noninjective tensors, their canonical forms first split into injective blocks; equality then permits a permutation of equivalent blocks together with a similarity transformation and phase on each block.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
