<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [uniform matrix product state](../../../../../../uniform-matrix-product-state.md) is specified by matrices $A^i\in M_D$ and, on a periodic chain, has amplitudes

$$
\langle i_1\cdots i_N|\Psi_N(A)\rangle
=\operatorname{Tr}(A^{i_1}\cdots A^{i_N}).
$$

It is injective when, after some blocking length $\ell$, the products $A^{i_1}\cdots A^{i_\ell}$ span $M_D$.

The [fundamental theorem of matrix product states](../../../../../../fundamental-theorem-of-matrix-product-states.md) says that two injective tensors generating the same states for all sufficiently large $N$ satisfy

$$
\boxed{A^i=e^{i\theta}XB^iX^{-1}}
$$

for one invertible matrix $X$; conversely this relation plainly gives the same periodic states up to the overall phase $e^{iN\theta}$.

For the proof, block enough sites that both tensors are injective. Injectivity gives left inverses from physical blocks to arbitrary virtual matrices. Equality of the states then implies that replacing one blocked tensor inside any sufficiently long network defines an invertible linear map on its two virtual boundary indices. Applying the replacement at two adjacent blocks in either order shows that this boundary map preserves multiplication: $\Phi(MN)=\Phi(M)\Phi(N)$. Every automorphism of the full matrix algebra is inner, so $\Phi(M)=XMX^{-1}$. Undoing the blocking gives $A^i=e^{i\theta}XB^iX^{-1}$, with only an $N$th-root phase left by periodic closure. Equality for consecutive sufficiently large lengths makes that phase independent of $N$ and completes the result.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
