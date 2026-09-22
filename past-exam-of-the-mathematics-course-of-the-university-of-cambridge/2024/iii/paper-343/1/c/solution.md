<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the stated [Pauli matrices](../../../../../../pauli-matrices.md) as

$$
A^x=\frac{\sigma_x}{\sqrt3},
\qquad
A^y=\frac{\sigma_y}{\sqrt3},
\qquad
A^z=\frac{\sigma_z}{\sqrt3}.
$$

The factor $3^{-1/2}$ changes only the overall normalization at fixed $N$. In the [spin-one Cartesian basis](../../../../../../spin-one-cartesian-basis.md), the associated periodic [uniform matrix product state](../../../../../../uniform-matrix-product-state.md) is

$$
|\Psi_N\rangle
=\sum_{i_1,\ldots,i_N\in\{x,y,z\}}
\operatorname{Tr}(A^{i_1}\cdots A^{i_N})
|i_1\cdots i_N\rangle.
$$

This is the [Pauli-matrix representation of the Affleck--Kennedy--Lieb--Tasaki state](../../../../../../pauli-matrix-representation-of-the-affleck-kennedy-lieb-tasaki-state.md).

The [Pauli matrix multiplication law](../../../../../../pauli-matrix-multiplication-law.md)

$$
\sigma_i\sigma_j=\delta_{ij}I+i\varepsilon_{ijk}\sigma_k
$$

shows that products on two neighboring sites span all of $M_2(\mathbb C)$, so the tensor is an [injective matrix product state](../../../../../../injective-matrix-product-state.md) after [blocking](../../../../../../blocking-a-matrix-product-state.md) two sites. More geometrically, its two-site image is the scalar plus antisymmetric subspace of $3\otimes3$, namely the total-spin $J=0$ and $J=1$ sectors. By the [Two-site support of the Pauli-matrix Affleck--Kennedy--Lieb--Tasaki tensor](../../../../../../two-site-support-of-the-pauli-matrix-affleck-kennedy-lieb-tasaki-tensor.md), the missing subspace is the five-dimensional symmetric traceless $J=2$ sector.

Let $P^{(2)}_{n,n+1}$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto that $J=2$ sector. The [parent Hamiltonian of a matrix product state](../../../../../../parent-hamiltonian-of-a-matrix-product-state.md) is

$$
H=\sum_nP^{(2)}_{n,n+1}.
$$

Each term annihilates $|\Psi_N\rangle$, so this is a [frustration-free quantum Hamiltonian](../../../../../../frustration-free-quantum-hamiltonian.md) and the MPS is a ground state. Writing $x=\mathbf S_n\mathbin\cdot\mathbf S_{n+1}$ and using the [eigenvalues](../../../../../../spin-dot-product-eigenvalue.md) $-2,-1,1$ in the three [total-spin sectors](../../../../../../total-spin-sector.md) gives the explicit projector

$$
P^{(2)}_{n,n+1}
=\frac{(x+2)(x+1)}6.
$$

This is the [Affleck--Kennedy--Lieb--Tasaki parent Hamiltonian](../../../../../../affleck-kennedy-lieb-tasaki-parent-hamiltonian.md). Injectivity implies that its periodic ground state is unique for every sufficiently long chain.

## ↑ Ancestors (11)

1. [C](../c.md)
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
